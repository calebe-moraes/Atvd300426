# Atividade: Arquitetura de Software e Diagramas de Sequência

Este projeto demonstra a implementação prática de uma arquitetura em camadas (MVC).

## 📊 Diagrama de Sequência

```mermaid
sequenceDiagram
    actor Usuario
    participant View
    participant Controller
    participant Service
    participant Repository

    Usuario ->> View: solicita consulta(id)
    View ->> Controller: request_consulta(id)
    Controller ->> Service: consultar_usuario(id)
    Service ->> Repository: buscar_por_id(id)
    Repository -->> Service: dados_usuario
    Service -->> Controller: usuario
    Controller -->> View: resposta(usuario)
    View -->> Usuario: exibe dados
