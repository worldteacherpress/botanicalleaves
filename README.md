# Botanical Leaves — World Teacher Press

Site estático educativo complementar ao livro. Inclui 52 fichas, pesquisa, filtros, navegação entre plantas e links individuais para os QR codes. Interface em inglês, em coerência com o livro.

## Publicar no GitHub Pages

1. Abra o repositório `botanical-leaves` da organização.
2. Escolha **Add file → Upload files**.
3. Carregue **o conteúdo desta pasta**: `index.html`, `style.css`, `plants.js`, `app.js`, `.nojekyll` e a pasta `assets`. O `index.html` deve ficar na raiz do repositório, não dentro de uma pasta `site`.
4. Confirme em **Commit changes**.
5. Em **Settings → Pages**, escolha **Deploy from a branch**, branch **main**, pasta **/(root)** e **Save**.
6. Aguarde a publicação e abra o endereço apresentado pelo GitHub.

Exemplo se a organização se chamar worldteacherpress:

`https://worldteacherpress.github.io/botanical-leaves/`

Uma ficha tem um endereço como:

`https://worldteacherpress.github.io/botanical-leaves/#plant/ginkgo-tree`

O fragmento `#plant/...` funciona diretamente no GitHub Pages sem configuração de rotas. Use o botão **Copy this plant’s link** depois da publicação. Gere os QR codes a partir do domínio real publicado. Não use endereços localhost nos QR impressos. Mantenha os identificadores das plantas, o nome da organização e do repositório após imprimir.

## Ver localmente

Na pasta `site`, execute `node serve.mjs` e abra http://localhost:4173 . Também é possível abrir o index.html diretamente para consultar a coleção.

## Conteúdo editorial

Os textos são introduções curtas à observação das folhas, não um guia de identificação conclusiva. As imagens são as ilustrações do livro, não fotografias de exemplares reais. Os rótulos genéricos permanecem ao nível do género ou grupo: não se assume que um nome comum identifica uma espécie exata. Antes da edição final, rever os desenhos e os nomes do livro em conjunto, sobretudo Aralia, Birch, Bird of Paradise, Caladium, Elephant Ear Philodendron, Fan Palm, Fern, Hawthorn, Oak, Plane Tree e Silver Dollar Eucalyptus.

Referências: [Kew Plants of the World Online](https://powo.science.kew.org/) e [Woodland Trust — observação de árvores](https://www.woodlandtrust.org.uk/trees-woods-and-wildlife/british-trees/how-to-identify-trees/). As ligações de cada ficha abrem uma pesquisa no Kew; não representam uma validação individual de todas as espécies ou ilustrações. A areca usa o nome aceite Chrysalidocarpus lutescens, com o sinónimo Dypsis lutescens explicado na ficha.

Os ficheiros do livro permanecem na pasta original; `assets` contém cópias reduzidas para o site. Para regenerar: `powershell -ExecutionPolicy Bypass -File prepare-assets.ps1`. As fontes Google são opcionais; existe alternativa local em Georgia/Arial. O site não precisa de conta de visitante, base de dados ou chave de API.
