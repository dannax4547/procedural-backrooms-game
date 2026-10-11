# Prompt 1 — Planejar e migrar de Unity para Unreal Engine 5

Atue como engenheiro responsável por planejar e executar a migração do jogo procedural de Backrooms deste repositório, hoje configurado em Unity 6.0.6f1 (confirme a versão real em ProjectSettings/ProjectVersion.txt), para Unreal Engine 5. Não comece convertendo arquivos em massa. Primeiro faça inventário verificável de cenas, prefabs, scripts, materiais, shaders, texturas, modelos, animações, áudio, UI, input, física, navegação, geração procedural, plugins, configurações e licenças.

## Regras de migração

- Preserve o checkout Unity e todo conteúdo original. Não apague nem substitua Assets, cenas, ProjectSettings, Packages ou metadados Unity; a migração deve ficar isolada em uma pasta/branch claramente definida e reversível.
- Leia o projeto real e identifique versão/recursos de Unity e pacotes utilizados. Para o destino, confirme a versão de UE5 instalada e compatível antes de fixar API ou formato.
- Classifique cada item: migrável diretamente, conversão assistida, reconstrução manual, substituível, fora de escopo ou bloqueado. Registre origem, destino, dependências, proprietário, risco e método de validação.
- Não presuma equivalência entre C# e C++, componentes Unity e Actors/Components, URP e renderer UE, prefabs e Blueprints, NavMesh, input, física ou pipelines de assets. Reprojete contratos para o modelo do Unreal em vez de portar nomes mecanicamente.
- Defina primeiro uma fatia vertical pequena: abrir um mapa, mover o jogador, carregar um ambiente e provar uma interação representativa. Estabeleça critérios visuais, funcionais, de performance e de build antes de migrar o restante.
- Preserve IDs, escalas, coordenadas, colisões, materiais e comportamento somente quando houver evidência. Verifique unidades, eixos, pivôs, orientação, importação, LOD e compressão.
- Faça backup/branch antes de operações de conversão em massa. Nunca sobrescreva o único original. Não baixe plugins, publique builds, altere custos ou envie conteúdo para serviços externos sem autorização.

Use a documentação oficial da versão efetiva do Unreal para decisões que dependam de versão. Faça um relatório de inventário, mapa de equivalência, decisões pendentes, protótipo vertical e validações executadas. Marque itens não migrados como pendentes; não declare a migração concluída por ter importado os assets.
