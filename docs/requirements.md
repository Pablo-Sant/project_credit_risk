# Requisitos Funcionais e Não Funcionais

## Requisitos Funcionais

1. O sistema deve calcular a probabilidade de um cliente entrar em inadimplência grave (atraso superior a 90 dias).

2. O sistema deve ser capaz de exibir um histórico de previsões realizadas por cada usuário.

3. O sistema deve permitir a entrada de dados do cliente para realização da previsão.

4. O sistema deve possuir tela de cadastro para usuários autorizados.

5. O sistema deve possuir tela de login para autenticação dos usuários.

6. O sistema deve poder ser utilizado como um serviço, por meio de uma API.

7. O sistema deve ser capaz de tratar os dados de entrada, validando tipo, obrigatoriedade e conformidade, além de realizar transformações necessárias, como feature engineering, normalização e encoding.

8. O sistema deve atuar com transparência, expondo erros e exceções de forma clara em cada etapa do processo de previsão.

9. O sistema deve apresentar uma interface de usuário (UI) para interação com as funcionalidades disponíveis.

---

## Requisitos Não Funcionais

1. O sistema deve utilizar autenticação via token JWT para garantir que cada usuário tenha acesso apenas às informações que lhe pertencem.

2. O sistema deve validar os dados de entrada para garantir robustez e correto funcionamento.

3. O sistema deve possuir uma arquitetura com forte separação de responsabilidades, visando manutenibilidade, testabilidade, legibilidade do código e facilidade de evolução.

4. O sistema deve armazenar senhas utilizando hash, garantindo que dados sensíveis não sejam persistidos em texto puro.

5. O sistema deve suportar a experimentação de múltiplos algoritmos de Machine Learning, com validação cruzada e seleção do modelo com melhor capacidade de generalização.

6. As métricas de avaliação do modelo devem ser escolhidas considerando sua relevância para o contexto de negócio.

7. O sistema deve facilitar o re-treinamento, atualização e monitoramento do modelo em produção.

8. O sistema deve garantir anonimização dos dados e conformidade com a LGPD.

9. O sistema deve possuir disponibilidade mínima de 99,9% ao mês.

10. A UI/UX do sistema deve ser projetada para garantir boa usabilidade e experiência do usuário.

11. O sistema deve versionar os modelos de Machine Learning e permitir rollback em caso de falhas ou degradação de desempenho.

12. Cada previsão realizada deve estar associada ao modelo utilizado, à sua versão e aos dados empregados na inferência.

13. O sistema deve fornecer explicações para as previsões, por meio de técnicas como feature importance ou SHAP.
