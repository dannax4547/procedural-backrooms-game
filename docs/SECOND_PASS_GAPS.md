# Second Pass Gaps — Levels 0–99

Data-base: 2026-10-02.

## Problemas confirmados nesta rodada
- Levels 37–40 estavam em formato antigo sem o schema obrigatório.
- Level 12 não possuía Entidades, Recursos e Mídia.
- Level 91 possuía checkbox [ ] que o validador interpretava como pendência.
- Levels 02 e 03 tinham lacunas explícitas de pesquisa nos próprios arquivos; ambos foram reestruturados.

## Gap estrutural de sub-seções
O snapshot oficial de 0–99 lista 58 sub-seções/localizações. A branch possui 28 arquivos dedicados e 30 ainda ausentes.

O inventário está em docs/SUBLEVEL_REGISTRY.md.

## Pendências prioritárias
- Manila Room, Red Rooms, The Torment.
- 1.3.
- Traders Vault.
- 2.1.
- 3.5.
- The Office Market.
- 5.1, 5.2, 5.3.
- 6.1, 6.2, 6.3, 6.31.
- 7.6, 7.7, 7.8, The Hadal Zone.
- 8.1, The Sanctum Subterraneous.
- 9.2, 9.3, 9.5, 9.9.
- 10.1, 10.2.
- AFTER HOURS, The Headquarters.
- Vultures In The Paper Oasis.
- Ground 48.1 — Noctilucent Ground.

## Catálogo transversal

- `docs/ENTITY_BASE_CATALOG_0_99.md`: concluído para os 100 níveis principais e 28 sub-seções já documentadas.
- Permanecem apenas as 30 sub-seções sem arquivo dedicado no registro oficial.

## Mídia
Os catálogos existentes não equivalem a licença individual fechada. Ainda é necessário:
- identificar autor e origem;
- registrar licença;
- marcar material não reutilizável;
- substituir referências bloqueadas quando possível.

## Conectividade
Ainda faltam:
- proveniência por aresta;
- confiança;
- arestas externas a 0–99;
- confirmação de bidirecionalidade;
- reconciliação de rotas de subníveis;
- atualização após rewrites.

## Verificação de ferramenta

- O código Rust foi revisado e o bug de classificação dos arquivos principais no inventário foi corrigido.
- `rustc` não está disponível no ambiente desta sessão; a compilação local não pôde ser realizada.
- `.github/workflows/backrooms-validation.yml` foi configurado como mecanismo de validação global.
- Não declarar “CI verde” sem um run disponível.

## Critério de conclusão real
A documentação só deve ser considerada completa quando níveis e sub-seções documentadas possuírem schema, desconhecidos explícitos, entidades, bases/instalações, entradas, saídas, mídia, estado editorial e validação Rust, além de reconciliação com o índice oficial.
