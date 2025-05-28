---
title: "Self-Attention AI Model for Practical Sensor Networking: Demodulation of Long-Period Fiber Grating Sensor Cascaded with FBG Sensor Array"
collection: publications
permalink: /publication/2025-05-23-Self-Attention-AI-Model-for-Practical-Sensor-Networking
category: manuscripts
date: 2025-05-23
venue: 'IEEE Transactions on Instrumentation and Measurement'
citation: ' Felipe Barino,  Alexandre Santos, &quot;Self-Attention AI Model for Practical Sensor Networking: Demodulation of Long-Period Fiber Grating Sensor Cascaded with FBG Sensor Array.&quot; IEEE Transactions on Instrumentation and Measurement, 2025.'
---


[Acesse o artigo](https://doi.org/10.1109/TIM.2025.3573014){:target="_blank"}


## O problema

As grades de fibra de período longo (LPFGs) são sensores ópticos com grande potencial devido à sua alta sensibilidade e versatilidade em diversas aplicações. No entanto, sua adoção em larga escala, especialmente em campo, é dificultada por alguns desafios importantes.  A interpretação dos sinais de LPFGs (um processo chamado interrogação) geralmente requer equipamentos volumosos e caros, pois seus espectros de transmissão são largos e complexos, diferentemente das grades de Bragg em fibra (FBGs), que possuem picos de reflexão bem definidos e soluções comerciais de interrogação já estabelecidas.

Além disso, a largura espectral das LPFGs limita a quantidade de sensores que podem ser monitorados simultaneamente em um mesmo cabo óptico (multiplexação), o que encarece sistemas que necessitam de muitos pontos de medição.  Apesar de serem mais fáceis de fabricar e capazes de medir uma gama maior de parâmetros que as FBGs (especialmente devido à sua sensibilidade ao índice de refração, útil em biossensores, na indústria alimentícia e no monitoramento de estruturas), esses desafios de interrogação e multiplexação precisam ser superados para que as LPFGs se tornem sensores práticos e amplamente utilizados fora do ambiente de laboratório. 

## Abordagem utilizada

Para enfrentar esses desafios, este trabalho propõe uma solução inovadora e de baixo custo para a interrogação de sensores LPFG, integrando-os a uma rede de sensores ópticos.  A ideia central é utilizar um conjunto de sensores FBG, já bem estabelecidos e com interrogadores comerciais disponíveis, de uma maneira nova: o espectro de reflexão das FBGs é modulado (alterado) pelo espectro de transmissão da LPFG.  Ou seja, a LPFG "filtra" a luz refletida pelas FBGs.

Para decodificar essa modulação espectral e extrair o comprimento de onda ressonante da LPFG (a informação chave do sensor), foi desenvolvido um modelo de Inteligência Artificial (IA) baseado em "autoatenção" (self-attention).  Esse modelo de IA consegue analisar dinamicamente os espectros de reflexão das FBGs e focar apenas nas características mais relevantes para a demodulação da LPFG, filtrando informações desnecessárias ou ruído. 

Uma característica importante desta abordagem é que o modelo de IA foi treinado inteiramente com dados sintéticos, ou seja, dados gerados por simulação computadorizada que imitam o comportamento dos sensores.  Isso elimina a necessidade de um processo demorado e custoso de coleta de uma grande quantidade de dados experimentais para treinar modelos complexos de IA.  A validação do sistema, no entanto, foi realizada com espectros de LPFGs reais.  O sistema óptico consiste na LPFG em série com um array de 13 sensores FBG, e um interrogador FBG comercial é usado para capturar o espectro de reflexão modulado.  Para evitar perdas excessivas de sinal, circuladores ópticos foram implementados para garantir que a luz interaja com a LPFG apenas após ser refletida pelas FBGs. 

## Resultados

O sistema proposto demonstrou uma capacidade de demodulação com resolução subnanométrica.  Nos testes com um conjunto de 73 espectros de LPFGs reais e 100 configurações diferentes de FBGs para cada um (totalizando 7300 amostras de teste), o sistema alcançou um erro quadrático médio (RMSE) de 0.75 nm e um erro percentual absoluto médio (MAPE) de 0.0335%.  A resolução estimada do sistema foi de 0.687 nm.  Esses resultados são comparáveis aos obtidos anteriormente com redes neurais treinadas com dados reais de LPFGs e FBGs estáticas, validando a eficácia da abordagem de treinamento com dados sintéticos e aprendizado por transferência para dados reais. 

O mecanismo de autoatenção do modelo de IA mostrou-se eficaz em focar nas características espectrais relevantes da LPFG, adaptando-se a deslocamentos no comprimento de onda ressonante da LPFG e sendo robusto a distorções no espectro e a pequenas variações na posição das FBGs.  O modelo também demonstrou ser insensível à largura e profundidade da depressão espectral da LPFG, o que o torna adequado para uma ampla variedade de sensores LPFG. 

Em uma demonstração prática, utilizando um sensor LPFG de índice de refração (RI) para medir diferentes concentrações de misturas de água e glicerol, o sistema apresentou um erro relativo inferior a 1% na estimativa do RI.  O sistema também foi capaz de identificar corretamente a posição da LPFG mesmo quando as FBGs próximas sofriam deslocamentos (simulando o uso das FBGs também como sensores), com coeficientes de correlação muito baixos entre os deslocamentos das FBGs e a posição estimada da LPFG (variando de -0.064 a 0.11), demonstrando a robustez da rede de sensores. 

## Perspectivas

Esta abordagem, que combina um array de sensores FBG com um modelo de IA de autoatenção treinado sinteticamente, oferece um caminho promissor para a interrogação de LPFGs de forma mais prática e com melhor custo-benefício em redes multissensores.  Ao simplificar a interrogação e alavancar o poder da IA e dos dados sintéticos, este trabalho abre portas para uma utilização mais ampla das LPFGs em diversas aplicações de sensoriamento, superando um dos principais obstáculos para sua adoção em campo. 

A capacidade de usar um interrogador FBG comercial e permitir que as próprias FBGs atuem como sensores (por exemplo, para medir deformação e temperatura, enquanto a LPFG mede outros parâmetros como índice de refração) aumenta significativamente a versatilidade e a economicidade dos sistemas de sensoriamento óptico.  O sucesso do treinamento com dados sintéticos também facilita o desenvolvimento de modelos de IA ainda mais robustos e complexos (como redes convolucionais ou transformers) para aprimorar ainda mais o paradigma de interrogação de LPFGs. 


## Material suplementar

Material suplementar, com funções usadas para gerar dados, modelos desenvolvidos, medições e resultados podem ser vistos no repósitório [lpfg_demodulation_supplementar](https://github.com/felipebarino/lpfg_demodulation_supplementary). Favor citar o reporitório e o trabalho, com seus respectivos DOIs.