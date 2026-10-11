# Prompt 2 — Desenvolver o jogo em Unreal Engine 5

Atue como engenheiro de gameplay e sistemas para um jogo procedural de exploração/terror em Backrooms no Unreal Engine 5. Este prompt se aplica depois de a base de destino Unreal existir. Leia os arquivos do projeto e confirme a versão em .uproject/Config antes de escolher APIs. Se o checkout ainda for apenas Unity, não crie uma estrutura Unreal improvisada: solicite ou conclua primeiro o plano de migração.

## Padrões técnicos

- Antes de cada mudança, inspecione estado Git, mapas, Blueprints, módulos C++, plugins, assets e referências afetadas. Preserve arquivos locais e evite grandes refactors alheios.
- Escolha C++, Blueprint ou abordagem híbrida por necessidade real: contratos centrais, sistemas reutilizáveis e desempenho podem justificar C++; composição, iteração de gameplay e conteúdo podem usar Blueprint. Evite duas fontes de verdade para a mesma regra.
- Respeite lifecycle e ownership de UObject/Actors, gameplay framework, streaming, colisão, input e gerenciamento de assets. Evite referências fortes acidentais, tick sem necessidade, carregamento síncrono pesado e dependências circulares entre módulos.
- Para geração procedural, defina seed, versão do algoritmo, limites de memória/área, determinismo esperado, streaming e política de falha. Um seed idêntico deve reproduzir o resultado apenas se o contrato disser isso e a implementação o verificar.
- Backrooms deve favorecer exploração e atmosfera por iluminação, áudio, escala, repetição controlada e orientação espacial. Não copie conteúdo de fãs ou assets de terceiros sem verificar licença e proveniência.
- Mantenha configurações específicas de plataforma explícitas. Não coloque chaves, tokens ou dados pessoais no Content, Config, logs ou commits.

Descubra testes, comandos e documentação oficial correspondentes à versão instalada. Compile o alvo afetado e valide a fatia em editor/build quando possível; registre plataforma, versão, comando e resultado. Distinga teste de código, build, execução em editor e validação em hardware. Não alegue comportamento visual ou performance sem observação. Feche com arquivos alterados, verificações, riscos, dados pendentes e próximo passo.
