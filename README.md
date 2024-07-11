O aplicativo Business Card é um aplicativo Android desenvolvido em Kotlin, que utiliza a arquitetura MVVM (Model-View-ViewModel) e o banco de dados Room para gerenciamento de informações de cartões de visita. Ele oferece funcionalidades de CRUD (Create, Read, Update, Delete) com uma interface interativa.

Estrutura do Projeto
Model: Define as entidades do banco de dados e as operações DAO (Data Access Object).
View: Contém as atividades e fragmentos que compõem a interface do usuário.
ViewModel: Gerencia os dados da interface e mantém o estado através do ciclo de vida das atividades e fragmentos.

Principais Tecnologias Utilizadas
Kotlin: Linguagem principal do aplicativo.
Room: Biblioteca de persistência que fornece uma camada de abstração sobre o SQLite.
LiveData: Utilizado para observar dados e atualizar a UI em resposta a mudanças nos dados.
ViewModel: Mantém os dados da UI em configurações de mudança de ciclo de vida.
RecyclerView: Exibe listas de cartões de visita de forma eficiente.
Data Binding: Liga componentes da UI aos dados do aplicativo de forma declarativa.

Funcionalidades Detalhadas
Adicionar Cartão: Implementado através de uma Activity com um formulário de entrada de dados e um ViewModel que insere os dados no banco de dados Room.
Editar e Excluir Cartões: Realizado através de um contexto de menu no RecyclerView, que permite editar ou excluir cartões selecionados. As operações são gerenciadas pelo ViewModel correspondente.
Seleção de Cor de Fundo: Implementada com um ColorPicker, armazenando a cor selecionada no banco de dados.

Estrutura do Banco de Dados
Entidades: Definidas na classe BusinessCard, com anotações do Room para mapear as colunas do banco de dados.
DAO: Interface BusinessCardDao define métodos para inserir, atualizar, excluir e consultar cartões.
Database: Classe AppDatabase que define o banco de dados Room e fornece instâncias do DAO.

O aplicativo Business Card é um exemplo de um aplicativo Android utilizando as práticas recomendadas de arquitetura e persistência de dados. A utilização do Kotlin, Room, LiveData e ViewModel proporciona uma aplicação bem estruturada, responsiva e fácil de manter.
