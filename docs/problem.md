# Problema

## Contexto

A inadimplência em operações de crédito representa um dos principais riscos enfrentados por instituições financeiras como bancos e fintechs. Quando um cliente deixa de honrar seus compromissos financeiros, especialmente em casos de inadimplência grave (atrasos superiores a 90 dias), o impacto vai além da perda direta do valor emprestado. Há aumento de custos operacionais com cobrança, necessidade de provisões financeiras para cobrir possíveis calotes e, em cenários mais críticos, prejuízos jurídicos.

Em larga escala, níveis elevados de inadimplência afetam a sustentabilidade do negócio. Para compensar perdas, as instituições tendem a elevar as taxas de juros, o que reduz a demanda por crédito, limita investimentos produtivos e pode gerar efeitos econômicos e sociais negativos. Portanto, a inadimplência não é apenas um problema financeiro interno das instituições, mas um fator relevante para a estabilidade econômica como um todo.

## Problema Central

As decisões de concessão de crédito ainda dependem, em muitos casos, de regras estáticas ou análises manuais que não conseguem capturar padrões complexos presentes em grandes volumes de dados históricos. Isso dificulta a identificação antecipada de clientes com maior risco de inadimplência grave, resultando em decisões subótimas, maior exposição ao risco e uso ineficiente de capital.

Além disso, mesmo quando modelos preditivos são utilizados, frequentemente há limitações relacionadas à falta de padronização do processo, baixa rastreabilidade das previsões, dificuldade de integração com sistemas existentes e ausência de mecanismos claros de monitoramento, versionamento e re-treinamento dos modelos.

## Proposta de Solução

Este projeto propõe o desenvolvimento de um sistema de Machine Learning capaz de estimar a probabilidade de inadimplência grave (+90 dias) de indivíduos a partir de dados históricos e cadastrais. O modelo será disponibilizado como um serviço (API), permitindo sua integração com sistemas de decisão de crédito de diferentes instituições financeiras.

O sistema receberá dados do cliente, realizará validações, transformações e aplicação de regras de negócio, e retornará uma probabilidade de inadimplência acompanhada de explicações sobre os fatores que influenciaram a previsão. As previsões serão persistidas de forma isolada por instituição, garantindo rastreabilidade, auditoria e uso futuro em ciclos de re-treinamento.

## Público-Alvo

O público-alvo do sistema são empresas que concedem crédito, como bancos tradicionais, fintechs e outras instituições financeiras, que necessitam de suporte analítico para reduzir riscos, melhorar a eficiência das decisões de crédito e manter a saúde financeira do negócio.

## Limites do Problema

O sistema não tem como objetivo identificar fraudes ou intenções deliberadas de não pagamento por parte dos indivíduos. Casos de estelionato ou fraude intencional fogem do escopo deste projeto. O foco está exclusivamente na previsão de risco de inadimplência com base em padrões históricos e comportamentais observáveis nos dados.

## Impacto Esperado

Com a adoção do sistema proposto, espera-se que as instituições consigam:

* Reduzir a taxa de inadimplência grave;
* Tomar decisões de crédito mais informadas e consistentes;
* Alocar capital de forma mais eficiente;
* Diminuir a necessidade de provisões excessivas;
* Manter taxas de juros mais equilibradas, contribuindo para um ambiente econômico mais saudável.

Do ponto de vista técnico, o projeto também demonstra a aplicação prática de conceitos de ML system design, como separação entre treino e inferência, persistência de previsões, versionamento de modelos e preparação para ciclos futuros de re-treinamento batch.
