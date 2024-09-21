# TerraçoTech CEu

Versão Base Atual: `1.3`

Branch Atual: `baseline`

---

Esta branch não possui nenhuma alteração do modpack oficial e se manterá atualizada conforme o modpack se atualizar.

Considere essa branch uma versão **"não-oficial"** de distribuição do modpack que gera um modpack idêntico¹ ao modpack providenciado pelo servidor.


> [!IMPORTANT]
> Esta branch minifica as configurações do jogo, mantendo apenas arquivos de config que foram modificados.
> Após o primeiro carregamento do jogo você obterá, se utilizar dessa branch, um modpack equivalente ao oficial.

> [!CAUTION]
> O modpack oficial tem um problema, a versão do mod "CC:C Bridge" é diferente da versão obtível pelo modrinth **ou** curseforge.
> A alteração que foi feita foi para diminuir a versão minima aceita do forge de `47.2.0` para `47.1.0`.
> Isso requer que ele seja embutido no modpack como um override, aumentando o tamanho do `mrpack` (Forge não tendo [Dependency Overrides](https://fabricmc.net/wiki/tutorial:dependency_overrides) fazendo com que esse tipo de maracutaia seja necessária denovo :( )

> [!TIP]
> A versão do modpack exportado usando o comando `packwiz mr export` é infinitamente menor que o modpack oficial (e é a que providenciamos pelos releases do github).
> Temos sempre a preferência de obter mods pelo modrinth, e quando não é possivel adicionamos o mod pelo curseforge.
> O que faz com que o mrpack (arquivo de modpack do modrinth) **só contenha arquivos de mods que foram adicionados pelo curseforge**.

> [!CAUTION]
> As versões (modificadas ou não) do CEu não possuem nenhum suporte aos jogadores. **Não importune a NotJustAnna por causa dessa "versão" do modpack**. Você está sozinho. Isso deve ser utilizado por usuários **muito avançados** ou aqueles que gostam de mecher em coisas e vê-las quebrarem.

---

Changeset:

`01-Remove-Clumps.patch` - Remove o mod "Clumps" do Client, visto que ele [**só é necessário no servidor**](https://modrinth.com/mod/clumps/).
`02-Replace-PingHud.patch` - Troca o mod "PingHud" pelo "Better Ping Display \[Forge\]". (Não sabo se vai dar bom, pq o mod tá com `BOTH` apesar de ser um single mixin mod em algo q claramente é client-sided. Q port mal feito pqp.)
`03-Remove-Terralith.patch` - Remove o mod "Terralith" do Client, visto que na real ele é um datapack, e não é necessário para entrar no servidor. (Se o forge deixar.)
`04-Remove-AcceleratedDecay.patch`- Remove o mod "Accelerated Decay", visto que em teoria ele não é necessário para entrar no servidor. (Se o gorge deixar.)
`05-Replace-Farsight.patch` - Troca o mod "farsight" pelo "Distant Horizons"


Ideias:
---

- Pegar absolutamente **todo mod feito por "someaddon"** e encontrar algum replacement open source. Eu não duvido q a vida desse cara é fazer repackage de mod open source. Não tem como alguem manter tanto mod e todos serem ARR.
