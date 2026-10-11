# Dossiê de pesquisa — Backrooms para o procedural-backrooms-game

**Snapshot de pesquisa:** 11/10/2026.  
**Fonte de referência:** [The Backrooms Wiki (Wikidot)](https://backrooms-wiki.wikidot.com/).  
**Uso:** pesquisa e design de jogo procedural; não é um cânone universal nem uma especificação jurídica.

## 1. Como ler este dossiê

A Wikidot declara que é um projeto de ficção colaborativa, aberto a contribuições e focado em interpretações variadas do cenário. Ela própria aponta a Fandom como outra perspectiva. Portanto, “conteúdo Backrooms” não significa que todas as páginas pertençam à mesma continuidade. Este jogo deve guardar a procedência e a continuidade de cada ideia, em vez de fundir tudo silenciosamente. [Página inicial e apresentação do projeto](https://backrooms-wiki.wikidot.com/)

Neste documento:

- **Wikidot** significa uma página publicada na comunidade `backrooms-wiki.wikidot.com`; não significa fato compartilhado por todas as comunidades.
- **Fandom** significa material da comunidade `backrooms.fandom.com`; é outra interpretação independente.
- **Kane Pixels/YouTube, 4chan, Reddit e outros autores** são origens/criações próprias, mesmo quando conceitos são adaptados por uma wiki.
- **Interpretação para jogo** é uma sugestão de design derivada da leitura, não uma regra canônica da fonte.
- **Não confirmado**, **relato**, **histórico**, **página em reescrita**, **arquivo** e **placeholder** devem continuar estados distintos. Não converter automaticamente rumores editoriais em monstros ou fatos do mundo.

O site muda com frequência. Os índices e páginas foram consultados no snapshot acima; antes de qualquer publicação ou implementação, confirmar novamente o status e a página-fonte.

## 2. Mapa do material da Wikidot

A biblioteca oficial separa tipos de conteúdo que podem ser entidades de dados distintas no jogo:

| Tipo | O que a wiki organiza | Possível uso procedural |
|---|---|---|
| [Levels](https://backrooms-wiki.wikidot.com/normal-levels-i) e [unnumbered levels](https://backrooms-wiki.wikidot.com/unnumbered-levels) | Espaços, regras, entradas/saídas e condições | Biomas/blueprints, regras locais e grafo de transição |
| [Entities](https://backrooms-wiki.wikidot.com/entities) e entidades não numeradas | Seres vivos com habitats, necessidades e comportamentos | Agentes, encontros, sinais, ecologia e perigo |
| [Objects](https://backrooms-wiki.wikidot.com/objects) | Ferramentas, armas, consumíveis, artefatos e objetos comuns alterados | Loot, crafting, risco de identificação e recursos |
| [Phenomena](https://backrooms-wiki.wikidot.com/phenomena) | Ocorrências anômalas que distorcem espaço, tempo, matéria ou percepção | Eventos sistêmicos locais, gatilhos e exceções temporárias |
| [Persons of Interest](https://backrooms-wiki.wikidot.com/poi-s) | Indivíduos marcantes, humanos ou não; importantes para a história | NPCs nomeados, registros, missões e memória do mundo |
| Groups | Comunidades, organizações e bases; diretório no menu da wiki | Fações, reputação, comércio, postos seguros e conflitos |
| [Tales](https://backrooms-wiki.wikidot.com/tales) | Narrativas | Logs, eventos roteirizados e contexto ambiental |
| [Canons](https://backrooms-wiki.wikidot.com/canons) e [series/subclusters](https://backrooms-wiki.wikidot.com/series-and-subclusters-hub) | Continuidades e conjuntos de páginas relacionados | Pacotes de conteúdo coerentes selecionáveis pelo jogador |
| [Joke entries, archived, trimmed e alternative pages](https://backrooms-wiki.wikidot.com/) | Estados editoriais e páginas alternativas | Não incorporar ao modo principal sem decisão explícita |

As categorias são importantes: a própria wiki diferencia “entidade” (ser vivo) de “objeto” (não vivo), e explica que entidades variam de habitantes amistosos a animais irracionais e seres incompreensíveis. Fenômenos são ocorrências, não criaturas. POIs são indivíduos documentados com impacto histórico. [Entities](https://backrooms-wiki.wikidot.com/entities), [Objects](https://backrooms-wiki.wikidot.com/objects), [Phenomena](https://backrooms-wiki.wikidot.com/phenomena), [POIs](https://backrooms-wiki.wikidot.com/poi-s)

## 3. Princípios narrativos que funcionam bem proceduralmente

### 3.1 Espaço familiar com regras quebradas

O Level 0 atual parte de escritórios/áreas comerciais comuns, mas torna a repetição, a escala e a continuidade espacial ameaçadoras. A descrição fala de corredores que se rearranjam quando não observados, isolamento entre pessoas, sons que parecem vir de lugares móveis e perigos de sobrevivência sem exigir combate. [Level 0 — “Threshold”](https://backrooms-wiki.wikidot.com/level-0)

**Tradução de design:** a tensão pode vir de navegação e percepção. Alterar a topologia com limites legíveis; usar áudio para orientar e também confundir; colocar marcos raros que ajudam o jogador a comparar o mapa; fazer as mudanças obedecerem a condições registradas em vez de aleatoriedade sem explicação.

### 3.2 O que o jogador sabe pode ser incompleto

A página de Level 0 diz que entidades ali não estão confirmadas: há relatos de figuras, mas nenhuma observação conclusiva. Isso é diferente de “spawnar uma criatura padrão”. A dúvida pode ser construída com silhuetas, ruídos, inconsistências de registro e ausência de confirmação. [Level 0](https://backrooms-wiki.wikidot.com/level-0)

### 3.3 Sobrevivência e exploração devem se cruzar

A página descreve desidratação e fome, carpetes úmidos e riscos ambientais. Já Level 4 apresenta água de amêndoa em bebedouros, máquinas e fontes, além de ser um lugar de encontro e reabastecimento, relativamente fácil de acessar e deixar. [Level 0](https://backrooms-wiki.wikidot.com/level-0), [Level 4 — “Abandoned Office”](https://backrooms-wiki.wikidot.com/level-4)

**Tradução de design:** construir uma curva de tensão por recursos: longos trechos incertos, sinais de possível abrigo, custo de desvio, pontos de reabastecimento e decisões sobre continuar ou voltar. Um recurso conhecido não precisa ser sempre seguro; cada nível descreve suas próprias condições.

### 3.4 Geometria deve variar por nível, não por um único gerador

Level 0 usa maze mutável e salas/variações arquitetônicas; Level 2 descreve túneis industriais estreitos, com cotovelos de 45 graus e comprimentos aproximados múltiplos de cinco metros; Level 3 é uma instalação elétrica com salas e corredores apertados, recursos valiosos e perigo alto; Level 4 é espaço de escritório e ponto de encontro. [Level 0](https://backrooms-wiki.wikidot.com/level-0), [Level 2](https://backrooms-wiki.wikidot.com/level-2), [Level 3](https://backrooms-wiki.wikidot.com/level-3), [Level 4](https://backrooms-wiki.wikidot.com/level-4)

**Tradução de design:** separar `LevelProfile` (materiais, módulos, regras, iluminação, áudio, perigos, recursos, conectividade) do gerador de salas. Usar geradores/modificadores diferentes para maze liminar, túnel utilitário, instalação elétrica e escritório. Os números e restrições geométricas acima são pistas específicas da página de Level 2, não leis de toda a Backrooms.

### 3.5 O mapa pode ser confiável só em certas zonas

No Level 0, salas de arcos são descritas como relativamente estáveis, enquanto salas de pilares podem confundir orientação e caminhos mudam. Trechos escuros alteram visibilidade e podem encher de líquido; salas vermelhas são descritas como desconectadas e quase impossíveis de abandonar. [Level 0](https://backrooms-wiki.wikidot.com/level-0)

**Tradução de design:** regras espaciais são atributos de região: `stability`, `visibility`, `landmark_density`, `route_mutation`, `hazard`, `escape_probability`. Elas podem orientar o gerador e a IA sem expor números ao jogador.

## 4. Sobrevivência, risco e dificuldade

A Wikidot possui um Survival Difficulty Class opcional; o próprio guia diz que o sistema não é obrigatório. Ele serve como metadado editorial, não como balanceamento pronto para videogame. Os níveis listam segurança, proteção contra ameaças e presença/certeza de entidades (ou campos equivalentes conforme a versão do guia). Confira o guia e o template atual antes de ingerir. [Survival Difficulty Class Guide](https://backrooms-wiki.wikidot.com/sd-class-guide)

Recomendação de dados para jogo (campos nossos, não da wiki):

- `hazards`: riscos ambientais e suas condições;
- `resource_pressure`: água, comida, descanso, luz, ferramentas;
- `entity_presence`: `confirmed | reported | unknown | absent | historical`;
- `human_presence`: sem presença, encontros raros, comunidades ou bases;
- `navigation_instability`: estático, variantes locais ou mutação dinâmica;
- `exit_visibility` e `exit_conditions`: saída observável, condicional, rara ou incerta;
- `source_confidence`: afirmação direta, relato interno, inferência de gameplay;
- `continuity_id`: continuidade/pacote editorial selecionado.

Não faça um único `difficulty` achatar tudo. Um nível pode ser fisicamente seguro, difícil de mapear e possuir entidades desconhecidas. Separe os eixos para que o jogo possa gerar experiências variadas sem contradições.

## 5. Conteúdo útil por subsistema

### Níveis e conectividade

O índice de níveis oferece níveis numerados, não numerados e subníveis; o repositório já inclui um grafo de conectividade e registro de subníveis. Trate cada ligação como direcionada e condicional: entrar em A a partir de B não prova que se possa voltar por qualquer rota. Registre método, condição, direção, status da página e certeza. [Índice de níveis](https://backrooms-wiki.wikidot.com/normal-levels-i), [níveis não numerados](https://backrooms-wiki.wikidot.com/unnumbered-levels)

### Entidades

Cada entidade deve ter habitat(s), comportamento, necessidades, sinais observáveis, resposta ao jogador e fonte. Não distribuir por toda parte: a página de um nível pode confirmar presença localizada, histórica ou contestada. O catálogo global é índice, não autorização para incluir toda criatura em todos os níveis. [Entities](https://backrooms-wiki.wikidot.com/entities)

### Objetos e recursos

Objetos podem ser banais, alterados, construídos por pessoas, úteis, perigosos ou semelhantes a outros objetos. A wiki destaca que a identificação importa porque existem falsificações/semelhantes. Para gameplay, isso dá suporte a inspeção, risco/recompensa e recursos com estado. Marcar individualmente objeto anômalo, consumível e recurso normal. [Objects](https://backrooms-wiki.wikidot.com/objects)

### Fenômenos

Fenômenos podem mudar geometria, física, tempo, percepção e propriedades de objetos. Modele-os como sistemas ou eventos com escopo, gatilho, duração, sinais prévios, contra-medidas e efeito persistente, não como item de loot ou inimigo por padrão. [Phenomena](https://backrooms-wiki.wikidot.com/phenomena)

### Fações, comunidades e POIs

Bases podem funcionar como áreas seguras, mercados, pontos de informação ou locais de conflito. Grupos e indivíduos nomeados são dependentes de continuidade; se houver sistemas de facção, a configuração do mundo deve definir quais entradas coexistem. Um POI não é automaticamente uma classe de inimigo. [Groups list](https://backrooms-wiki.wikidot.com/groups-list), [POIs](https://backrooms-wiki.wikidot.com/poi-s)

### Canons e series

A wiki abriga canons distintos e series de páginas conectadas; série é descrita como páginas que formam uma história contínua. Use um `content pack`/`continuity profile` para selecionar conjuntos compatíveis. No modo misto, deixe explícito que o jogo está combinando interpretações. [Canons](https://backrooms-wiki.wikidot.com/canons), [Series & Subclusters](https://backrooms-wiki.wikidot.com/series-and-subclusters-hub)

## 6. Fandom e outras criações — eixo separado

A Wikidot chama a Fandom de “different perspective”, não de continuação subordinada. As páginas da Fandom não devem ser tratadas como confirmação de uma página Wikidot. A URL traduzida indicada pelo usuário e páginas canônicas Fandom foram bloqueadas para leitura direta automatizada durante esta pesquisa (restrição/erro do servidor); por isso, esta versão **não** afirma ter feito comparação integral linha a linha.

**Leads secundários para pesquisa manual posterior (Fandom, não Wikidot):**

- [Fandom — Level 0](https://backrooms.fandom.com/wiki/Level_0): o resultado indexado descreve uma versão chamada “The Lobby” e lista suas próprias propriedades/saídas. Trate como artigo Fandom e confira autoria/histórico na página antes de adotar; não substituir Level 0 Wikidot “Threshold”.
- [Fandom — Entity List](https://backrooms.fandom.com/wiki/Entity_List): diretório próprio de entidades/categorias. Nomes que coincidam com a Wikidot não garantem mesma origem autoral, descrição ou continuidade.
- [Fandom — Groups](https://backrooms.fandom.com/wiki/Groups): diretório próprio de grupos; não importar nomes ou relações para o conjunto Wikidot sem uma fonte correspondente.
- **Kane Pixels** é outra criação/autoria audiovisual. Se o projeto quiser níveis, criaturas ou eventos inspirados nessa série, devem ser catalogados como `KanePixels`/`creator-universe`, não rebatizados como Wikidot/Fandom. Confirmar fontes primárias do criador e direitos antes de uso.

Status de procedência sugerido no jogo:

| Código | Significado |
|---|---|
| `wikidot:<slug>` | página primária da Backrooms Wiki Wikidot |
| `fandom:<slug>` | página da comunidade Backrooms Fandom |
| `creator:<name>/<work>` | obra independente identificada por criador |
| `community:<site>/<page>` | conteúdo de outra comunidade |
| `original:procedural-backrooms-game` | conteúdo original do jogo |
| `inference:<source-id>` | interpretação de design criada pela equipe, ligada à fonte que motivou a ideia |

## 7. Licença, atribuição e imagens

A Wikidot informa que, salvo aviso diferente, o conteúdo da página é CC BY-SA 3.0; cada página também traz autoria/citação e arquivos de imagem podem ter licenças próprias. A página de Level 0, por exemplo, indica autores da revisão e licenças individuais para diferentes imagens. Isso demonstra que licença de texto não concede automaticamente licença de imagem. [Licensing Guide](https://backrooms-wiki.wikidot.com/licensing-guide), [Image Use Guide](https://backrooms-wiki.wikidot.com/image-use-policy), [Level 0 credit block](https://backrooms-wiki.wikidot.com/level-0)

Para o jogo:

1. Não baixar nem incorporar uma imagem só porque aparece na wiki ou no Fandom.
2. Registrar cada asset com URL original, autor, licença específica, prova da licença, transformações e atribuição requerida.
3. Tratar texto CC BY-SA 3.0 com atribuição e obrigações share-alike aplicáveis; consultar orientação jurídica antes de misturar material adaptado à distribuição comercial/proprietária.
4. Criar arte original ou usar assets com licença comercial compatível sempre que houver dúvida. Gerar uma imagem por IA tampouco elimina a necessidade de revisar ferramentas, direitos de referência e política interna do projeto.
5. Manter lore em forma de resumo factual e links, evitando copiar trechos longos das páginas.

A política de imagem da wiki disciplina contribuições para a própria comunidade; para uso externo, o que manda é a licença real do asset e a lei aplicável. Nunca presumir que a permissão para publicar na wiki equivale a permissão ampla para usar no jogo.

## 8. Esquema mínimo para o banco de conteúdo

```yaml
id: wikidot:level-0
source:
  site: backrooms-wiki.wikidot.com
  url: https://backrooms-wiki.wikidot.com/level-0
  accessed: 2026-10-11
  authors: [DivineAtlas, DrAkimoto, RobertGoerman]
  license_text: CC-BY-SA-3.0
  license_assets: verify-per-asset
continuity: wikidot-main
editorial_status: current # current | rewrite | archived | trimmed | alternative | unknown
kind: level
claims:
  - claim: "Layout can change when not observed"
    status: described-in-page
    confidence: source-explicit
    gameplay: "Conditional topology mutation"
    inference: true
entities:
  - id: "example-entity"
    presence: unknown
exits: []
assets: []
```

Manter `claim` separado da interpretação de gameplay. O importador deve guardar URL de origem, revisão/data consultada, autores, estado editorial e licença; deve sinalizar alteração na página para revisão humana.

## 9. Inventário do repositório e próximos lotes de pesquisa

O repositório já contém arquivos `levels/` para níveis 0–99, `SUBLEVEL_REGISTRY.md`, `LEVEL_CONNECTIVITY_GRAPH.md`, `ENTITY_BASE_CATALOG_0_99.md`, matriz de status de cânone e catálogos de imagens. Esses arquivos são o material local existente; este dossiê não os substitui nem valida cada entrada individual.

Para ampliar a cobertura com rigor:

1. Auditar URLs, autoria, status editorial, revisão e citações de cada nível local (0–99 e subníveis).
2. Conferir separadamente páginas de entidades, objetos, fenômenos, grupos, POIs e contos citados pelos níveis.
3. Acrescentar níveis não numerados e canons/series como pacotes opcionais, com conexões e proveniência.
4. Fazer levantamento Fandom com navegação manual se a proteção anti-bot continuar bloqueando; manter comparação lado a lado e atribuição independente.
5. Criar catálogo próprio de licença de imagens/áudio, pois lore e arte têm direitos distintos.
6. Só depois escolher um escopo de continuidade para a primeira versão jogável; começar pequeno (por exemplo, uma rota curta entre níveis iniciais) e manter os demais conjuntos desativados até serem compatibilizados.

## 10. Segunda rodada — níveis 5–10, entidades e sobrevivência

Esta rodada reforça que os níveis têm identidade mecânica e editorial própria. Também encontrou páginas explicitamente marcadas como desatualizadas ou em reescrita; seu conteúdo pode servir como histórico/inspiração, mas não deve entrar no pacote atual sem revisão.

### Níveis 5–10

| Página | O que está descrito na Wikidot | Leitura para o jogo | Estado/alertas |
|---|---|---|---|
| [Level 5 — Terror Hotel](https://backrooms-wiki.wikidot.com/level-5) | Hotel aparentemente dos anos 1930, mobiliário antigo, limpeza inexplicável, jazz aleatório, três áreas (Main Hall, Beverly Room, Boiler Room), portas/elevadores com destinos incertos, áreas habitadas e colmeias de Deathmoths. | Um nível pode funcionar como hub social e ainda manter áreas de alto risco. Contrastar hospitalidade/serviço com ruídos, portas que mudam e salas com regras próprias. | Página atualizada; tem tag/canon `terror-hotel-canon`. O histórico de autoria credita originalmente uma pessoa usuária da Fandom, com reescrita atual da Wikidot: proveniência cruzada, versão corrente Wikidot. Imagens possuem licenças específicas listadas na página. |
| [Level 6 — Lights Out](https://backrooms-wiki.wikidot.com/level-6) | Escuridão total, fontes de luz não funcionam, navegação pelo tato em corredores estreitos. | Um segmento que troca visão por som, tato, memória espacial e recursos de orientação. Deve ser usado como experiência curta/opcional para evitar fadiga. | Banner explícito “outdated”; dificuldade pendente. Tratar como versão histórica/legada até a reescrita. Autoria de base inclui Reddit. |
| [Level 7 — Thalassophobia](https://backrooms-wiki.wikidot.com/level-7) | Oceano aparentemente infinito, pouca exploração, travessia exige preparação e é perigosa. | Muda a navegação para superfície/verticalidade, orientação por marcos distantes, gestão de fôlego e expedições preparadas. | Também marcada “outdated”. Não tratar o artigo atual como ficha definitiva do cânone Wikidot. |
| [Level 8 — Cave Systems](https://backrooms-wiki.wikidot.com/level-8) | Sistemas de cavernas em grande escala. | Usar módulos e conectividade próprios: bifurcações, gargalos, desníveis e acústica que comunica distância/direção. | Verificar status editorial e detalhes no artigo completo antes de parametrizar. |
| [Level 9 — The Suburbs](https://backrooms-wiki.wikidot.com/level-9) | Área suburbana infinita à meia-noite; casas diferentes, algumas vazias, itens úteis, aparelhos que exigem energia sem funcionar. | Exploração de interiores como microdungeons; separar silhueta da rua e conteúdo da casa; usar casas semelhantes como falsa familiaridade. | A página atual atribui origem a u/Bart0nius no Reddit e reescrita por Stretchsterz na Wikidot. Usar identidade `wikidot:level-9` e manter origem histórica separada. |
| [Level 10 — Bumper Crop](https://backrooms-wiki.wikidot.com/level-10) | Campos extensos de trigo/cevada, linhas de árvores, céu nublado constante, chuva/neblina raras e vento como quebra da uniformidade. A ficha exibe classificação por eixos (saída, ambiente, entidades). | Ameaça pode vir de horizonte e visibilidade, sem combate. Cultivos permitem ocultação e orientação por linhas, mas reduzem marcos verticais. | Página atual com Survival Difficulty Class 1 e métricas: saída 2/5, ambiente 1/5, entidades 0/5. A página credita a origem original a u/Hertz3241 no Reddit. |

#### Level 5 como aula de composição

Level 5 demonstra um padrão útil para proceduralidade: **um tema comum com subáreas de regras distintas**. O hotel tem salão principal, salão de baile/hub e sala de caldeiras; cada uma muda densidade de objetos, som, temperatura, aperto espacial, riscos e conexões. Entradas e saídas ligam outros níveis sob condições variadas. Em jogo, isso sugere gerar primeiro um grafo de zonas e depois construir cada zona com um perfil, em vez de escolher peças de sala aleatórias em um único saco.

#### Status editorial é dado de runtime/autoria

As páginas consultadas do Level 6 e Level 7 exibem aviso de desatualização. Portanto, o sistema de importação deve guardar `editorial_status` junto do conteúdo e permitir excluir páginas `outdated`, `under-rewrite`, `trimmed` ou `archived` do pacote padrão. Para modo “arquivo”, elas podem aparecer com rótulo e data próprios.

### Entidades que ensinam comportamento legível

[Entity 3 — Smilers](https://backrooms-wiki.wikidot.com/entity-3) e [Entity 8 — Hound](https://backrooms-wiki.wikidot.com/entity-8) demonstram que um encontro pode depender do comportamento do jogador, não só de HP e perseguição:

- O artigo atual dos Smilers descreve atração por luz e recomenda manter contato visual/afastar-se lentamente; ruído alto ou recuo em pânico podem precipitar ataque. Isso dá um ciclo de leitura de sinais → controlar luz/ruído → retirada cuidadosa.
- O artigo atual dos Hounds descreve uma criatura quadrúpede agressiva; contato visual pode intimidá-la por pouco tempo, enquanto rosnado indica que ficar à vista é perigoso. Isso cria uma escolha de risco: encarar para ganhar tempo ou esconder-se quando o aviso sonoro já surgiu.
- Ambas as fichas registram autor original associado à Fandom e reescrita na Wikidot. A versão consultada é a Wikidot atual; a procedência original deve ser preservada nos metadados. Não copiar suas artes sem conferir licença individual.

Para a IA, extrair **ações e observáveis**, não apenas “hostil”: `stimuli`, `warning_signals`, `escalation_conditions`, `deescalation_actions`, `pursuit_constraints`, `habitat`, `confidence`. Um comportamento interativo pode ficar injusto se o jogo não ensina seu gatilho; cada regra precisa de sinal visual/sonoro e chance razoável de resposta.

### Objeto: Almond Water

[Object 1 — Almond Water](https://backrooms-wiki.wikidot.com/object-1) aparece como termoses de líquido claro, um recurso muito procurado e amplamente encontrado. A ficha registra utilidade para sobrevivência; a origem da abundância aparece como desconhecida, e uma hipótese em textos antigos é expressamente tratada como possível lenda. A mesma página Level 0 observa que o líquido que contamina carpetes pode estar adulterado, então “Almond Water” em um recipiente conhecido e líquido no chão não são loot equivalente.

**Aplicação procedural:** modelar identidade/procedência do recipiente, estado (lacrado, aberto, contaminado), fonte de água e confiança do jogador. Evitar converter uma conjectura de origem em explicação narrativa definitiva.

### Fenômeno em reescrita: Directed Control

[Phenomenon 1 — Directed Control](https://backrooms-wiki.wikidot.com/phenomenon-1) está marcado como “being rewritten”. O próprio texto em andamento levanta dúvida se se trata de efeito sobrenatural ou resposta de autopreservação/trauma e pede crítica, destacando viés de confirmação. Isso é um exemplo excelente de **incerteza diegética**, mas não de regra estável pronta para o jogo. Guardar em quarentena de pesquisa até a página sair da reescrita.

### Narrativas como fonte de conteúdo, não catálogo de regras

O hub [Tales](https://backrooms-wiki.wikidot.com/tales) diz que os contos variam em formato, tema e gênero e podem aprofundar lore de níveis/grupos. Para o jogo, usar contos como fonte de fragmentos narrativos, logs, cronologia e ideias de missão; verificar se pertencem a uma série/canon particular e não assumir que cada acontecimento é universal.

## 11. Regras adicionais para o importador

Os achados desta rodada justificam acrescentar estes campos ao esquema sugerido:

```yaml
editorial_status_detail: current | outdated | under-rewrite | archived | trimmed
origin_community: wikidot | fandom | reddit | 4chan | creator | unknown
current_version_author: []
historical_original_author: []
continuity_tags: []
survival_profile:
  exit: null
  environment: null
  entities: null
mechanics:
  stimuli: []
  warnings: []
  counterplay: []
```

`origin_community` não substitui `source_site`: uma página pode ser uma reescrita Wikidot de uma ideia originalmente publicada por outra pessoa/comunidade. Armazenar ambos evita apagar a proveniência e evita confundir a versão atual com a origem histórica.

## 12. Terceira rodada — cidade-hub, censura e biomas (Levels 11–20)

### Level 11 — cidade como infraestrutura sistêmica

[Level 11 — The City That Never Sleeps](https://backrooms-wiki.wikidot.com/level-11) é apresentado como metrópole extensa, com blocos de ruas, bairros de densidade variável, escolas, shoppings, transporte, canais, túneis, pontes, edifícios acessíveis e estruturas que parecem fachadas intransponíveis. A página descreve sistemas autossuficientes de energia, água, produção e abastecimento; objetos e veículos podem mudar de lugar quando não observados. O nível é um hub informal, mas muitas saídas são discretas, direcionais e potencialmente sem retorno.

**Aplicação ao jogo:** é um candidato a hub de longo prazo, mas não deve ser uma “cidade aberta infinita” sem estrutura. Gerar distritos conectados por uma malha legível, com densidade e função urbana, rotas subterrâneas próprias, edifícios com regras de acesso e saída. O deslocamento de objetos quando não observados pode sustentar eventos de mundo e reposição de loot; a dificuldade de registrar saídas sustenta exploração e cartografia. Uma base humana pode estabilizar visualmente um trecho, dando uma pista narrativa de ocupação.

### Level 12 — pouca ameaça, pouca explicação

[Level 12 — Matrix](https://backrooms-wiki.wikidot.com/level-12) descreve um cômodo simples, branco e iluminado com mesa, cadeira e porta trancada; tentativas de registrar o local produzem imagem branca/ruído ou tela de teste. Pessoas relatam entrar e sair, mas o método costuma ser esquecido. A página classifica o nível como dificuldade 0 e não registra avistamentos de entidades.

**Aplicação:** uma sala curta de transição ou pausa que quebra a expectativa com um forte efeito de gravação. A impossibilidade de registrar pode ser simulada como regra local de câmera/log; nunca como falha genérica de gravação do próprio jogo. As saídas incertas precisam ser comunicadas como mistério intencional.

### Níveis 13–20: não importar apenas pelo título

O índice confirma uma grande variedade temática, mas título não basta para definir mecânica. As páginas iniciais consultadas indicam:

- [Level 13 — The Boiling Frogs](https://backrooms-wiki.wikidot.com/level-13): página com várias reescritas e autoria corrente Wikidot; inspecionar o corpo completo antes de codificar.
- [Level 14 — Paradise](https://backrooms-wiki.wikidot.com/level-14): tem autoria identificada e hub de obras do autor; contexto e continuidade devem ser lidos antes de combinar com outros níveis.
- [Level 15 — Futuristic Halls](https://backrooms-wiki.wikidot.com/level-15): marcado “being rewritten”. A página ainda traz uma restrição explícita sobre novas conexões; não inventar entradas/saídas no grafo do jogo.
- [Level 16 — Altered Topography](https://backrooms-wiki.wikidot.com/level-16): apresentado como ecossistema de floresta tropical com neblina e gravidade reduzida que afeta objetos vindos de fora, não organismos nativos; a página usa narrativa de arquivos/versões e deve ser interpretada junto ao texto completo.
- [Level 17 — The Carrier](https://backrooms-wiki.wikidot.com/level-17): o texto descreve “Plane #17”, uma embarcação/estrutura de passagens, com setores e compartimentos em operação temporal independente segundo relatos/evidências circunstanciais. Não reduzir esse conteúdo a “corredor genérico”.
- [Level 18 — Memories](https://backrooms-wiki.wikidot.com/level-18): marcado “outdated”; a versão consultada descreve espaços que lembram memórias de infância e vozes ligadas a arrependimentos, mas deve ficar em categoria histórica até reescrita.
- [Level 19 — Attic Floorboards](https://backrooms-wiki.wikidot.com/level-19): marcado “being rewritten”; manter em quarentena editorial.
- [Level 20 — Boreas Structure](https://backrooms-wiki.wikidot.com/level-20): a página apresenta duas seções (Waiting Halls e The Electric), avisos de perigo, efeitos auditivos/visuais relatados e substância gelatinosa de origem desconhecida; é importante distinguir observação, hipótese e informação confirmada.

### Padrão de evidência diegética

Essas páginas misturam bases de dados ficcionais, relatórios de exploradores, avisos editoriais e hipóteses. Para tornar isso jogável sem apagar a nuance:

1. Guardar a frase como **observação relatada**, não automaticamente como propriedade física universal.
2. Dar grau de confiança e número/qualidade de testemunhas quando a própria fonte oferece isso.
3. Permitir conteúdo procedural variar a ocorrência de eventos incertos sem mudar as regras confirmadas.
4. Fazer o jogador encontrar evidências contraditórias quando isso for intencional, e identificar a contradição como parte da história.
5. Nunca usar página em reescrita para uma regra fundamental do tutorial ou para bloquear a progressão principal.

### Mais exemplos de procedência entre comunidades

O Level 5 atual registra autor original da Fandom e reescrita atual na Wikidot. Smilers e Hounds também creditam a origem de seus artigos a usuário(s) da Fandom, embora as páginas consultadas sejam versões reescritas na Wikidot. Isso mostra que “quem originou a ideia”, “quem escreveu o texto atual” e “qual comunidade contém a página consultada” são campos separados. Para atribuição do jogo, conservar os três quando forem conhecidos; não chamar a versão atual de Fandom só porque a origem foi daquela comunidade.

## 13. Quarta rodada — rotas condicionais e escala de biomas (Levels 21–30)

### Level 21 — portas como grafo probabilístico (versão desatualizada)

[Level 21 — Numbered Doors](https://backrooms-wiki.wikidot.com/level-21) descreve quatro corredores longos que se encontram num centro com mesa/cadeiras. Portas numeradas e portas com características distintas podem apontar para níveis diferentes, subníveis ou rotas que retornam ao próprio Level 21; algumas levam a paredes. O artigo também descreve corredores mutáveis e entidades variáveis.

O artigo está explicitamente marcado como **outdated** e inclui recomendações diegéticas de cautela. Use-o como referência de um padrão procedural de alto valor — portas como arestas de grafo com destino, condições e probabilidade —, mas não como conteúdo estável do modo principal até nova versão.

### Levantamento por conceitos nas páginas 21–30

| Página | Evidência consultada | Ideia procedural | Estado que exige cuidado |
|---|---|---|---|
| [Level 21 — Numbered Doors](https://backrooms-wiki.wikidot.com/level-21) | Corredores mutáveis, portas variadas, saídas que podem retornar, destino desconhecido ou até parede. | Gerar uma rede de transições com rótulos, destino e direcionalidade; portas podem ser um puzzle de navegação. | `outdated`; não adotar o inventário de portas como atual. |
| [Level 22 — Ruins Left Behind](https://backrooms-wiki.wikidot.com/level-22) | Título aponta cenário de ruínas; precisa de leitura integral antes de derivar mecânicas. | Potencial para ruína, vestígios e narrativa ambiental. | A consulta desta rodada só confirmou título; tratar o conteúdo como não analisado. |
| [Level 23 — The Petrified Garden](https://backrooms-wiki.wikidot.com/level-23) | Superorganismo do tamanho aproximado de um planetoide, superfície de floresta densa e túneis/pockets de ar internos; fauna presente. A classificação aparece `4?` e inclui “overgrown”. | Construir ecologia vertical em duas camadas (dossel e interior subterrâneo), com entradas de luz, ar e fauna distribuída por habitat. | A classificação traz interrogação: não achatar a incerteza para um escore definitivo. |
| [Level 24 — The Moon](https://backrooms-wiki.wikidot.com/level-24) | Um modelo artificial em escala do sistema solar; a superfície lunar tem gravidade normal e eventos meteorológicos artificiais, incluindo névoa tóxica com propriedades específicas. | Ambiente surreal pode seguir uma regra física coerente e permitir decisões de equipamento/abrigo. | Página tem detalhes técnicos ficcionais; confirmar toda mecânica com o texto antes de implementar. |
| [Level 25 — The Quarter Hub](https://backrooms-wiki.wikidot.com/level-25) | O índice apresenta um nível hub e a página lista versões/autoria. | Hub pode organizar as transições da campanha. | Marcado “being rewritten”; colocar em quarentena. |
| [Level 26 — The SS Fun =)](https://backrooms-wiki.wikidot.com/level-26) | A página atual contém relato narrativo sobre navio de cruzeiro e referências a lenda de teletransporte/experimento; há autores e revisão identificados. | Introduzir cenário de embarcação, isolamento e documentos em formato testemunhal. | Separar fatos do narrador, folclore citado e regra do nível. |
| [Level 27 — The Bunker Springs](https://backrooms-wiki.wikidot.com/level-27) | Fonte termal pequena, água potável/mineral e relatos de maior clareza/energia; a descrição menciona uma passagem de drenagem pequena demais para exploração humana. | Um ponto de descanso pode oferecer benefício com limite, além de um mistério ambiental que não é rota viável. | Marcado `outdated`; a classificação 0 é da versão antiga. |
| [Level 28 — Final Virtue](https://backrooms-wiki.wikidot.com/level-28) | Página consultada usa componentes e navegação expansiva; resumo do topo não foi extraído com segurança nesta rodada. | Não derivar mecânica só do título. | Precisa de leitura integral dedicada. |
| [Level 29 — Hyperian](https://backrooms-wiki.wikidot.com/level-29) | Comunidade numa ilha, oceanos/áreas externas, círculo exterior e interior protegido por montanhas; água de Almond Water em rios. | Projetar mapa de escala macro com zonas aninhadas e passagem de ambiente exposto para refúgio protegido. | Marcado `being rewritten`; a ficha mostra classificação 4 e saída muito difícil/infestação hostil, mas tudo deve ser revalidado pós-rewrite. |
| [Level 30 — Shifted Beyond Reality](https://backrooms-wiki.wikidot.com/level-30) | Céu amplo com ilhas e entidades chamadas Memory Lurkers; contato pode alterar percepção/memórias/ambiente. | Distúrbio perceptivo atrelado a interação observável, com mundo alterado temporariamente e registros persistentes separados da verdade objetiva. | Marcado `outdated`; não tratar o mecanismo atual como versão final. |

### Rotas e regras como dados de primeira classe

As páginas do Level 5 e do Level 21 ajudam a refinar o grafo de conectividade: uma porta precisa de `source_zone`, `destination_level`, `destination_zone`, `direction`, `conditions`, `reliability`, `revisitability`, `editorial_status` e `source_url`. Uma rota narrada como rumor deve ser `reported`; uma rota observada mas de sentido único é `confirmed_one_way`; uma porta que pode voltar ao nível original não cria automaticamente saída garantida.

### Expansão de identidade visual e sonora

Com os níveis consultados até 30, já há uma gama de perfis distintos para organizar futuros módulos de geração: escritório amarelo; túneis utilitários; instalação elétrica; escritório-abrigável; hotel antigo; escuridão tátil; oceano; caverna; subúrbio noturno; campos; metrópole; quarto branco que censura gravações; espaço infantil/memorial (em versão outdated); portas numeradas; floresta-planetoide; lua artificial; nave/estrutura; ilha e céu-ilhas. Esses são nomes/temas de artigos Wikidot, cada qual com estado próprio. O jogo deve evitar um gerador único de “corredor Backrooms” e permitir perfis de nível realmente diferentes.

## Fontes de partida

- [Página inicial, escopo e interpretações da Wikidot](https://backrooms-wiki.wikidot.com/)
- [Índice de Levels](https://backrooms-wiki.wikidot.com/normal-levels-i) e [unnumbered levels](https://backrooms-wiki.wikidot.com/unnumbered-levels)
- [Entities](https://backrooms-wiki.wikidot.com/entities), [Objects](https://backrooms-wiki.wikidot.com/objects), [Phenomena](https://backrooms-wiki.wikidot.com/phenomena)
- [Groups](https://backrooms-wiki.wikidot.com/groups-list), [POIs](https://backrooms-wiki.wikidot.com/poi-s), [Tales](https://backrooms-wiki.wikidot.com/tales)
- [Canons](https://backrooms-wiki.wikidot.com/canons), [Series & Subclusters](https://backrooms-wiki.wikidot.com/series-and-subclusters-hub)
- [Survival Difficulty Class Guide](https://backrooms-wiki.wikidot.com/sd-class-guide)
- [Licensing Guide](https://backrooms-wiki.wikidot.com/licensing-guide), [Image Use Guide](https://backrooms-wiki.wikidot.com/image-use-policy)
- Exemplos de níveis: [0](https://backrooms-wiki.wikidot.com/level-0), [1](https://backrooms-wiki.wikidot.com/level-1), [2](https://backrooms-wiki.wikidot.com/level-2), [3](https://backrooms-wiki.wikidot.com/level-3), [4](https://backrooms-wiki.wikidot.com/level-4)
