# TERMO DE ABERTURA DO PROJETO (TAP)

## 1. Identificação

**Nome do Projeto:**  
Sistema de estimativa de probabilidade de inadimplência (PD)

---

## 2. Alinhamento Estratégico

Gestão de risco de crédito e otimização de capital.

---

## 3. Público-alvo

Empresas que concedem crédito, como bancos e fintechs.

---

## 4. Justificativa

Este projeto visa mitigar a ocorrência de inadimplência em instituições financeiras por meio de um modelo de Machine Learning que prediz a probabilidade de um indivíduo entrar em inadimplência grave (atraso superior a 90 dias). Quando os bancos sofrem inadimplência, eles perdem o dinheiro emprestado e os lucros que receberiam ao longo do contrato. Além disso, aumentam os gastos operacionais para acompanhamento do devedor, gestão do prejuízo e, em alguns casos, ações jurídicas.

Outro impacto relevante é a necessidade de utilizar provisões para devedores duvidosos, ou seja, dinheiro que poderia ser usado para conceder novos empréstimos e gerar receita passa a ser reservado para cobrir possíveis calotes. Quando a inadimplência é elevada, os bancos tendem a aumentar as taxas de juros de seus produtos de crédito para compensar as perdas. Com juros mais altos, empresas e pessoas físicas tomam menos empréstimos, investem menos, geram menos empregos e reduzem renda. Isso faz com que mais pessoas tenham dificuldade para pagar suas dívidas, elevando ainda mais a inadimplência.

Esse cenário gera um ciclo de contração de crédito e desaceleração econômica. Portanto, a inadimplência não é apenas um problema financeiro das instituições bancárias, mas também um problema econômico e social.

---

## 5. Escopo / Objetivos

Será utilizado um dataset público que simula dados reais de uma instituição financeira, contendo informações de diversos clientes, como histórico de pagamentos, renda, idade, entre outras variáveis. A partir desses dados, será treinado um modelo de Machine Learning com o objetivo de estimar a probabilidade de um indivíduo, em algum momento após a concessão do crédito, entrar em inadimplência grave (atraso superior a 90 dias).

O modelo será disponibilizado como um serviço (API) e implantado em um ambiente de produção simulado (deploy), permitindo que empresas que concedem crédito utilizem a estimativa de risco como apoio à tomada de decisão, visando reduzir a inadimplência e promover decisões de crédito mais sustentáveis e justas.

---

## 6. Exclusões / Não Escopo

Este projeto não tem como objetivo identificar fraude ou a intenção do indivíduo ao tomar o empréstimo. Casos em que o cliente já contrata o crédito com a intenção de não pagar caracterizam estelionato, mas a detecção desse tipo de comportamento não faz parte do escopo do sistema. O foco do projeto é exclusivamente o risco de inadimplência, independentemente da intenção do indivíduo.

---

## 7. Premissas

Assume-se que o dataset utilizado representa de forma razoável o comportamento real de clientes que tomam crédito. Considera-se que os padrões históricos de inadimplência ajudam a prever o risco de novos clientes no futuro. A definição de inadimplência grave como atraso superior a 90 dias é considerada válida e alinhada às práticas do mercado financeiro.

Parte-se do pressuposto de que as variáveis disponíveis, como dados cadastrais, histórico de crédito e comportamento anterior, possuem informação suficiente para explicar o risco de inadimplência. O modelo será utilizado como apoio à decisão, e não como o único critério para aprovação ou rejeição de crédito.

---

## 8. Restrições

O projeto utiliza um dataset público e anonimizado, que não contém todas as informações que um banco real teria acesso, como dados transacionais em tempo real, informações de open finance ou indicadores macroeconômicos. O modelo será treinado apenas com dados disponíveis no momento da concessão do crédito, caracterizando-o como um modelo de originação.

O escopo do projeto é restrito à estimativa da Probabilidade de Inadimplência (PD), não incluindo modelos de Loss Given Default (LGD) ou Exposure at Default (EAD). O ambiente de produção será uma simulação em cloud, sem integração com sistemas bancários reais.

---

## 9. Riscos

Os dados podem conter vieses históricos de concessão de crédito, o que pode influenciar o comportamento do modelo. Existe o risco de overfitting e de o modelo não generalizar bem para novos clientes. Mudanças no perfil dos clientes ou no cenário econômico podem causar degradação de desempenho ao longo do tempo.

Caso as probabilidades previstas não sejam bem calibradas, o sistema pode levar a decisões inadequadas, como conceder crédito a clientes muito arriscados ou rejeitar clientes com bom perfil. Além disso, modelos mais complexos podem dificultar a explicação das decisões, o que é um ponto crítico em aplicações de crédito.
