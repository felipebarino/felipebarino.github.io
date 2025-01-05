---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Formação
---
* Ph.D em Engenharia Elétrica, Universidade Federal de Juiz de Fora, 2025 (em andamento)
* M.S. em Engenharia Elétrica, Universidade Federal de Juiz de Fora, 2021
* B.S. em Engenharia Elétrica, Universidade Federal de Juiz de Fora, 2019

Ensino
---
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Pesquisa e desenvolvimento
---
* 2023-Atual: Desenvolvimento e Aplicação de Metodologia para Segregação de Perdas de Cargas e Fenômenos Hidráulicos na Tomada d'água
  * Local: Laboratório de Instrumentação e Telemetria
  * Atividades: Metodologia, Validação, Calibração, Desenvolvimento de software, Infraestrutura de redes

* 2022-2024: Aferição dos sensores a fibra óptica desenvolvidos para a Ambev
  * Local: Laboratório de Instrumentação e Telemetria
  * Atividades: Metodologia, Validação, Desenvolvimento de software, Análise de dados

* 2021-2022: Identificação de Parâmetros na Cerveja, como Amargor, utilizando Sensores a Fibra Óptica
  * Local: Laboratório de Instrumentação e Telemetria
  * Atividades: Metodologia, Desenvolvimento de software, Análise de dados

* 2020-2023: Desenvolvimento de Sistemas Mecatrônicos Remotamente Operados para Limpeza e Inspeção do Batente e Soleira de Vedação dos StopLogs de Hidroelétricas
  * Local: Laboratório de Instrumentação e Telemetria
  * Atividades: Análise de dados

Patentes
---

* Dispositivo de Medição de Vórtice. Número do registro: BR1020190272473, Instituição de registro: INPI - Instituto Nacional da Propriedade Industrial. Depósito: 10/02/2020

* Sensor óptico a fibra para medição de cálcio em leite. Número do registro: BR10202300621, Instituição de registro: INPI - Instituto Nacional da Propriedade Industrial. Depósito: 03/04/2023

* Sensor óptico baseado em um interferômetro de Mach-Zehnder em fibra para monitoramento do processo de fermentação. Número do registro: BR10202300620, Instituição de registro: INPI - Instituto Nacional da Propriedade Industrial. Depósito: 03/04/2023 

Publicações
---
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% include archive-single-cv.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}
{% endif %}