# Análise Comparativa de Arquiteturas

## 1. MVC (Model-View-Controller)
- **View:** Interface do usuário.
- **Controller:** Orquestra o fluxo.
- **Model:** Regras de negócio e persistência.
*Observação: O Controller decide qual View exibir.*

## 2. MVP (Model-View-Presenter)
- O **Presenter** atua como intermediário direto. A View é mais "passiva" e repassa eventos para o Presenter.

## 3. MVVM (Model-View-ViewModel)
- Utiliza **Data Binding**. A View reage a mudanças na **ViewModel** de forma automática (notificarMudanca).