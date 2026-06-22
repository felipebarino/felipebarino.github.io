---
title: "Optical tongue based on Mach–Zehnder interferometers and automated machine learning for spoilage microorganisms assessment in ricotta cheese"
collection: publications
permalink: /publication/2026-06-16-Optical-tongue-MZI
category: manuscripts
date: 2026-06-16
venue: 'IEEE Access'
citation: 'Renato Luiz Faraco Filho, Deivid Campos, Lizandra Rezende, Felipe Oliveira Barino, Marcus Vinicius Souza, Alexandre Bessa dos Santos, &quot; Optical tongue based on Mach–Zehnder interferometers and automated machine learning for spoilage microorganisms assessment in ricotta cheese.&quot; Sensors and Actuators A: Physical, 2026.'
---


[Acesse o artigo](https://doi.org/10.1016/j.sna.2026.118109){:target="_blank"}


### O Problema

O controle microbiológico de queijos frescos de alta umidade, como a ricota, representa um desafio crítico para a indústria de laticínios devido à vulnerabilidade desses produtos à rápida proliferação de microrganismos deteriorantes e patogênicos (como o *Staphylococcus spp.*). Métodos analíticos convencionais, que se baseiam em contagens em placas de cultura e ensaios bioquímicos, embora sejam confiáveis, são demorados, destrutivos e demandam uma infraestrutura especializada. Essa lentidão impede o monitoramento em tempo real ou em linha na cadeia de produção. Por outro lado, sensores eletrônicos comerciais (línguas e narizes eletrônicos) comumente aplicados na indústria sofrem com limitações severas, incluindo alta sensibilidade a interferências ambientais externas (como temperatura e umidade), ruído eletromagnético e a necessidade de protocolos rígidos de estabilização térmica e mecânica antes de cada medição.

### Abordagem Utilizada

Para solucionar essas limitações, a pesquisa propôs e desenvolveu um sistema integrado de monitoramento não destrutivo combinando sensores interferométricos de fibra óptica com um framework de Aprendizado de Máquina Automatizado (AutoML). A plataforma de detecção óptica funciona como uma "língua eletrônica". Ela foi construída utilizando um Interferômetro de Mach-Zehnder (MZI) constituído por duas redes de período longo micro-conificadas (MT-LPFGs) fabricadas em cascata em uma fibra monomodo padrão (SMF-28) via técnica de descarga de arco elétrico. O princípio operacional baseia-se em monitorar as flutuações no índice de refração do entorno do sensor; as alterações físico-químicas geradas pela atividade metabólica do *Staphylococcus spp.* modulam a fase interferométrica e alteram o perfil espectral de transmissão da luz na fibra. Para interpretar esses padrões espectrais não lineares e complexos e estimar a contaminação microbiológica ($log_{10} CFU/g$), utilizou-se o framework *AutoGluon* para otimizar e avaliar sistematicamente múltiplos algoritmos de regressão, aplicando também uma análise multicritério baseada na Fronteira de Pareto para balancear precisão e custo computacional.

### Resultados

Os experimentos laboratoriais validaram a alta capacidade do sistema em detectar e quantificar o gradiente de contaminação microbiológica na ricota, destacando-se pelos seguintes achados:

* **Desempenho Preditivo Superior:** O modelo baseado em redes neurais profundas (*NeuralNetTorch*) obteve a maior acurácia no conjunto de testes independentes, alcançando um coeficiente de correlação de Pearson ($R$) de 0,976 e um coeficiente de determinação ($R^2$) de 0,951, demonstrando excelente adaptação à estrutura não linear dos dados ópticos.


* **Banda Espectral Otimizada:** A análise de importância de variáveis identificou que as faixas de comprimento de onda entre 1480–1500 nm e 1510–1530 nm concentram a maior sensibilidade às variações bacterianas na matriz láctea, servindo como guia essencial para o design de futuros sensores ópticos dedicados.


* **Alto Limite de Detecção (LOD):** O sistema alcançou um limite de detecção multivariado analítico de 1,62 $log_{10} CFU/g$ (~42 CFU/g), valor significativamente inferior às concentrações iniciais testadas e confortavelmente abaixo dos limites regulatórios de segurança alimentar.


* **Eficiência Computacional via Pareto:** A análise multi-objetivo revelou que os modelos de conjunto baseados em árvores, especialmente o *ExtraTrees*, representam o melhor compromisso operacional para aplicações industriais práticas; eles mantiveram alta estabilidade e métricas de acurácia competitivas exigindo apenas uma fração minúscula ($10^3$ ciclos de CPU) do tempo de processamento consumido por redes neurais profundas.



### Perspectivas

Este trabalho estabelece uma base sólida para a transição tecnológica rumo ao controle de qualidade automatizado e digitalizado em laticínios (*Food Quality 4.0*). O sucesso da integração do sensor MT-LPFG com ferramentas de AutoML viabiliza o desenvolvimento de dispositivos compactos, robustos e imunes a ruídos para inspeção em tempo real e em linha. Os desdobramentos futuros das pesquisas estarão focados na expansão do banco de dados experimentais para englobar diferentes marcas de queijo, origens do leite, perfis de aditivos e variadas condições reais de armazenamento. Adicionalmente, planeja-se refinar as estratégias de calibração contínua e processamento de sinal para mitigar o envelhecimento natural dos componentes ópticos, além de otimizar os algoritmos mais eficientes (como o *ExtraTrees*) para embarque direto em sistemas de hardware de baixo custo (*edge deployment*) na linha de processamento industrial.