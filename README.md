# Atividade: Arquitetura de Software e Diagramas de Sequência

Este projeto demonstra a implementação prática de uma arquitetura em camadas (MVC) utilizando Python, comparando uma interface de linha de comando (CLI) e uma interface Web (Flask).

## 📊 Diagrama de Sequência
O fluxo da aplicação segue o padrão abaixo, garantindo que a View nunca acesse o Repository diretamente:

![Diagrama de Sequência](https://www.planttext.com/api/plantuml/png/SoSmIImgL03ApaaiBbR8pY_Epo_DAr5GjLFGjVGrK_3CJSuioatDArAmid8pSd9mId9iS0fS2WfS2_iBAdCIyx9oIdBIn681In6Y0000)

## 🛠️ Tecnologias Utilizadas
- **Linguagem:** Python 3.x
- **Framework Web:** Flask
- **Modelagem:** PlantUML

## 📂 Organização das Camadas
1. **View:** Responsável pela interação com o usuário (Entrada/Saída).
2. **Controller:** Gerencia as requisições e trata exceções de fluxo.
3. **Service:** Onde residem as regras de negócio.
4. **Repository:** Responsável única e exclusivamente pelo acesso aos dados.

## 🚀 Como executar
Para a versão CLI:
`python src/main_cli.py`

Para a versão Web:
`python src/main_web.py`