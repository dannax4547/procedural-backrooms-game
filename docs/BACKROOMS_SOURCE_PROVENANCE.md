# Registro de comparação — Wikidot, Fandom e obras independentes

**Revisado em:** 11/10/2026  
**Objetivo:** impedir que o projeto trate comunidades e criações independentes como um único cânone.

## Regra de procedência

O projeto usa a [Backrooms Wiki Wikidot](https://backrooms-wiki.wikidot.com/) como fonte de referência principal, conforme decisão do usuário. A própria Wikidot descreve o site como ficção colaborativa com interpretações variadas e aponta a Fandom como outra perspectiva. Logo, Wikidot e Fandom são comunidades/continuidade distintas; nenhuma página Fandom é prova automática de uma afirmação Wikidot. [Declaração da Wikidot](https://backrooms-wiki.wikidot.com/)

## Limite desta consulta

O usuário forneceu [Backrooms Wiki Fandom via tradução](https://backrooms-fandom-com.translate.goog/wiki/Backrooms_Wiki). A consulta automatizada recebeu bloqueio/restrição ao abrir esse link e as páginas canônicas correspondentes; a página Groups também respondeu erro de acesso. Não foi possível ler integralmente conteúdo, histórico, autores e licenças nesta sessão. Os itens abaixo são pistas do índice de busca, não auditoria completa; precisam de conferência manual antes de entrar no jogo.

## Leads Fandom para verificar

| Página | Atribuição correta | Como tratar |
|---|---|---|
| [Level 0](https://backrooms.fandom.com/wiki/Level_0) | Artigo da comunidade Fandom | Resultado indexado usa o título “The Lobby”. Comparar estrutura, saídas, entidades e autores com o [Level 0 Wikidot “Threshold”](https://backrooms-wiki.wikidot.com/level-0). São duas versões; não fundir os detalhes. |
| [Entity List](https://backrooms.fandom.com/wiki/Entity_List) | Diretório de entidades da Fandom | Catálogo secundário próprio. Mesmos nomes em outra wiki podem ter histórias e regras diferentes. Associar cada ficha ao seu site/slug/autoria. |
| [Groups](https://backrooms.fandom.com/wiki/Groups) | Diretório de grupos da Fandom | Não importar facções para o conjunto Wikidot sem página-fonte independente na Wikidot. |

Os resultados encontrados mencionam entidades como Smilers, Deathmoths, Clumps, Dullers, Hounds, Facelings, Skin-Stealers e Wretches. Alguns desses nomes também aparecem no ecossistema Wikidot, mas a coincidência de nome não prova que descrição, autoria ou continuidade sejam iguais. Comparar as páginas individuais e registrar duas fichas se as regras diferirem.

## Obras de outros criadores

- **4chan / post original:** o artigo atual de Level 0 na Wikidot credita o conceito original a um post de 4chan e identifica adaptações e reescritas posteriores. Isso é proveniência histórica da ideia; o texto corrente do Level 0 é a versão da página Wikidot e tem seus próprios autores. [Créditos do Level 0](https://backrooms-wiki.wikidot.com/level-0)
- **Kane Pixels:** obra audiovisual independente; qualquer material extraído dela deve ser registrado como obra/criador próprio, não como “Wikidot” ou “Fandom”. Buscar a fonte oficial do criador para estabelecer origem, versão e autorização antes de usar personagens, cenas, imagens ou áudio.
- **Reddit e outros criadores:** uma wiki pode adaptar algo que nasceu em outra comunidade. Salvar tanto `source_page` quanto `original_creator/source` quando a página creditar outra origem.
- **Conteúdo original do jogo:** ideias geradas pela equipe ficam marcadas `original:procedural-backrooms-game`, com referências inspiradoras separadas. Não atribuir como oficial à comunidade.

## Campos de proveniência obrigatórios

```yaml
source_site: backrooms-wiki.wikidot.com # ou backrooms.fandom.com, criador/site
source_url: https://...
source_title: ...
source_author: []
source_original_creator: []
continuity: wikidot-main # fandom | kane-pixels | creator:<name> | original-game
editorial_status: current # archived | trimmed | rewrite | unknown
license_text: CC-BY-SA-3.0 # conferir página
license_assets: verify-per-asset
accessed: 2026-10-11
confidence: primary-page-read # search-snippet | inferred | user-provided
```

## Política de comparação para novos registros

1. Ler a página primária completa e o histórico quando disponível.
2. Registrar nomes, descrição, autor, revisão, URL, licença e estado editorial separadamente para cada site.
3. Comparar apenas características explicitamente citadas. “Parece a mesma criatura” entra como hipótese, não como fato.
4. Manter uma tabela `shared_name` quando houver nome igual, mas preservar IDs independentes (`wikidot:...`, `fandom:...`).
5. Marcar adaptações de uma página como derivadas e manter crédito/origem citada.
6. Não usar a palavra “canônico” sem completar a qualificação: canônico para qual comunidade, cânone ou obra?
7. Quando uma fonte estiver bloqueada ou removida, anotar a lacuna e não preencher com memória ou fanon.

## Referências primárias consultadas

- [Wikidot: escopo do site e link para a Fandom como perspectiva diferente](https://backrooms-wiki.wikidot.com/)
- [Wikidot: Level 0 e créditos de adaptação/autoria](https://backrooms-wiki.wikidot.com/level-0)
- [Wikidot: diretórios de entidades](https://backrooms-wiki.wikidot.com/entities), [objetos](https://backrooms-wiki.wikidot.com/objects), [grupos](https://backrooms-wiki.wikidot.com/groups-list), [POIs](https://backrooms-wiki.wikidot.com/poi-s)
- Fandom (acesso direto bloqueado nesta consulta): [Level 0](https://backrooms.fandom.com/wiki/Level_0), [Entity List](https://backrooms.fandom.com/wiki/Entity_List), [Groups](https://backrooms.fandom.com/wiki/Groups)
