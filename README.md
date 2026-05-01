Atividade: Arquitetura de Software e Diagramas de Sequência

Este projeto demonstra a implementação prática de uma arquitetura em camadas (MVC).

📊 Diagrama de Sequência

sequenceDiagram
    actor Usuario
    participant View
    participant Controller
    participant Service
    participant Repository

    Usuario->>View: solicita consulta(id)
    View->>Controller: request_consulta(id)
    Controller->>Service: consultar_usuario(id)
    Service->>Repository: buscar_por_id(id)
    Repository-->>Service: dados_usuario
    Service-->>Controller: usuario
    Controller-->>View: resposta(usuario)
    View-->>Usuario: exibe dados


🛠️ Tecnologias Utilizadas

Linguagem: Python 3.x

Framework Web: Flask

Modelagem: Mermaid

📂 Organização das Camadas

View: Responsável pela interação com o usuário.

Controller: Gerencia as requisições e trata exceções.

Service: Onde residem as regras de negócio.

Repository: Responsável pelo acesso aos dados.

🚀 Como executar

Para a versão CLI:
python src/main_cli.py

Para a versão Web:
python src/main_web.py
