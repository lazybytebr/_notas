# _notas

```mermaid
usecaseDiagram

actor Cliente
actor Esteticista
actor Administrador

Cliente --> (Agendar Sessão)
Cliente --> (Cancelar Sessão)
Cliente --> (Avaliar Atendimento)

Esteticista --> (Visualizar Agenda)
Esteticista --> (Registrar Atendimento)
Esteticista --> (Preencher Anamnese)

Administrador --> (Gerenciar Usuários)
Administrador --> (Visualizar Relatórios)
Administrador --> (Configurar Sistema)
```
