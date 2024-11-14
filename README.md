# RA3-rec
tarefa para a matéria de arquitetura de software

%% C4 Model - Level 1: Diagrama de Contexto

graph TD
    A[Usuário (Vendedor/ Caixa)] -->|Usa| B[Sistema PDV]
    B -->|Integra| C[API Gateway]
    B -->|Comunica| D[iFood]
    B -->|Integra| E[Serviço de Pagamentos]
    B -->|Integra| F[Sistemas Externos (ERP)]
    B -->|Integra| G[Serviço de Relatórios]
    B -->|Integra| H[Serviço de Notas Fiscais]
    C -->|Roteia requisições| I[Microserviço de Produtos]
    C -->|Roteia requisições| J[Microserviço de Vendas]
    C -->|Roteia requisições| K[Microserviço de Clientes]
    C -->|Roteia requisições| L[Microserviço de Pagamentos]
    C -->|Roteia requisições| M[Microserviço de Relatórios]
    C -->|Roteia requisições| N[Microserviço de Notas Fiscais]

