---
title: "Correlated Time-Series in Multi-Day-Ahead Streamflow Forecasting Using Convolutional Networks"
collection: publications
permalink: /publication/2020-01-01-Correlated-Time-Series-in-Multi-Day-Ahead-Streamflow-Forecasting-Using-Convolutional-Networks
category: manuscripts
date: 2020-01-01
venue: 'IEEE Access'
citation: ' Felipe Barino,  Vinicius Silva,  Andres Lopez-Barbero,  Leonardo Honorio,  Alexandre Santos, &quot;Correlated Time-Series in Multi-Day-Ahead Streamflow Forecasting Using Convolutional Networks.&quot; IEEE Access, 2020.'
---
[Acesse o artigo](https://doi.org/10.1109/ACCESS.2020.3040942){:target="_blank"}

<img src="/images/graphical_abstract_correlated_ts_cnn.png">

## O problema

A previsão da vazão dos rios é crucial para o planejamento da produção de energia hidrelétrica, especialmente para usinas hidrelétricas a fio d'água. No entanto, a vazão do rio é um reflexo de vários fatores hidrológicos, hidrogeológicos e meteorológicos, o que aumenta a dificuldade de modelagem direta e favorece o uso de métodos orientados por dados.

## Abordagem utilizada

Neste artigo, propomos o uso de redes neurais convolucionais unidimensionais (1d-CNN) para previsão de vazão de vários dias à frente e apresentamos um modelo de múltiplas entradas usando séries temporais de entrada correlacionadas. Observamos que a vazão e a turbidez do rio são altamente correlacionadas, mas deslocadas no tempo. 

## Resultados

O modelo proposto foi aplicado no Rio Madeira, o maior e mais importante afluente do Amazonas, próximo à Usina Hidrelétrica de Santo Antônio. Observamos que a vazão está 38 dias atrasada da vazão, logo a turbidez é uma boa informação sobre a vazão futura. Os resultados mostraram que o uso de séries temporais correlacionadas como entrada para um modelo 1d-CNN diminui o tamanho do modelo em 5 vezes, com melhorias na precisão.

## Perspectivas

Acreditamos que a abordagem proposta pode ser aplicada em outros rios e bacias hidrográficas, contribuindo para um planejamento mais eficiente e preciso da geração de energia hidrelétrica. Além disso, pretendemos investigar o uso de outras variáveis hidrológicas e meteorológicas como entrada para o modelo, visando melhorar ainda mais sua precisão e robustez.
