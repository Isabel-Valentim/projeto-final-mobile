# projeto-final-mobile

### ANA CLARA GUARIZI DE SOUZA E ISABEL PEREIRA MIRANDA VALENTIM

Este repositório contém a documentação e a pasta zipada do projeto no expo.

O Todo-Calendar é um aplicativo desenvolvido em React Native que permite aos usuários gerenciar suas tarefas e eventos em um único lugar. Ele combina funcionalidades de um calendário com uma lista de tarefas e eventos, permitindo que os usuários adicionem, excluam e visualizem. O app também está integrado a uma API (MockAPI) para persistência de dados.

## VÍDEO
link: https://www.youtube.com/watch?v=YUNUU-ZDydI&ab_channel=IsabelValentim

## DOCUMENTAÇÃO

Descrição dos Módulos e Componentes
1. App.js
Função: Configura a navegação principal do aplicativo.
Navegação:
React Navigation é usado para gerenciar navegação entre telas.
Usa o Stack Navigator e Material Top Tabs para uma navegação fluida.


2. Tela de Tarefas (HomeScreen.js)
Função: Gerencia as tarefas do usuário.
Principais Recursos:
Adicionar Tarefa:
O usuário insere um texto no input e clica no botão "Adicionar".
A tarefa é enviada para a API MockAPI e exibida na lista.
Excluir Tarefa:
Cada tarefa tem um botão "Excluir" para removê-la da API e da lista local.
Dependências:
FlatList: Para renderizar a lista de tarefas.
fetch: Para integrar com a API.
3. Tela de Eventos (CalendarScreen.js)
Função: Permite gerenciar eventos com um calendário interativo.
Principais Recursos:
Selecionar Data:
O usuário seleciona uma data no calendário.
Adicionar Evento:
Inclui campos para Nome, Local e Descrição do evento.
O evento é salvo na API MockAPI e exibido em uma lista abaixo do calendário.
Excluir Evento:
Cada evento possui um botão "Excluir" que remove o evento da lista e da API.
Dependências:
react-native-calendars: Para exibir o calendário.
fetch: Para interagir com a API.
6. Integração com MockAPI
Endereços de API:
Tarefas:
GET /tasks: Retorna todas as tarefas.
POST /tasks: Adiciona uma nova tarefa.
DELETE /tasks/{id}: Remove uma tarefa.
Eventos:
GET /events: Retorna todos os eventos.
POST /events: Adiciona um novo evento.
DELETE /events/{id}: Remove um evento.
Configuração:
URLs são armazenadas diretamente nos componentes (API_URL).
