
![](geral//Capa.png)


# Projeto TODO

<h1 align="center"> 
🚧 Projeto em construção 🚧
</h1>

# Índice 

  - [Descrição do projeto](#descrição-do-projeto)
  - [Tecnologias utilizadas](#️tecnologias-utilizadas) 
  - [Funcionalidades do projeto](#funcionalidades-do-projeto)  
  - [Benefícios do Projeto](#benefícios-do-projeto)
  - [Acesso ao projeto](#acesso-ao-projeto)
  - [Desenvolvedores](#desenvolvedores)


## Descrição do projeto 

<p align="justify">
Projeto de um Sistema de Gerenciamento de Tarefas, desenvolvido junto com o TreinaWeb. O sistema oferece uma solução para organizar e acompanhar atividades diárias.
</p>

- `Tarefa concluida`: Permite ao usuario, ao marcar uma tarefa como concluída, a data de conclusão automática para a tarefa deve ser registrada como a data atual, fornecendo um registro preciso do momento em que a tarefa foi finalizada. Além de permitir uma ordenação por data de entrega.
<img width="100%" height="200" src="./geral/Ordenado_por_data-entrega.png"></img>

- `Botões Inativos (Editar e Concluir)`: Inativar os botões "Editar" e "Concluir" após a marcação de uma tarefa como concluída impede a realização de ações inconsistentes ou desnecessárias. Isso contribui para a consistência do sistema e evita que os usuários tentem editar ou concluir novamente uma tarefa que já foi finalizada. A inativação dos botões reflete o estado atual da tarefa, proporcionando uma experiência de usuário mais intuitiva e evitando possíveis confusões.
<img width="100%" height="200" src="./geral/Desabilitar_botoes_apos_concuido.png"></img>

- `Herança de template`: Permite criar um template base com funcionalidades comuns e, em seguida, estender ou especializar esse template para criar novos componentes. Reduz a duplicação de código, uma vez que as partes comuns são definidas no template base e compartilhadas por todas as classes derivadas.
<img width="100%" height="200" src="./geral/Herança_templates_List-Base.png"></img>

- `Validação de Campos`: Ajuda a garantir a integridade dos dados, evitando a entrada de valores inválidos ou inconsistentes. Isso é crucial para manter a precisão e confiabilidade das informações manipuladas pelo software.
<img width="100%" height="200" src="./geral/Validação_dos_campos..png"></img>

- `H2 database - Configurações`: 

``conexão com Banco de Dados`` => spring.datasource.url=jdbc:h2:file:./h2-database <br>
  - tipo de banco => *jdbc:h2*
  - tipo que o h2 vai funcionar será em arquivos => *:file*
  - local do arquivo gerado (raiz do projeto) => *./h2-database*

``usuario para acessar o banco`` => spring.datasource.username=sa
  - padrão => *sa*

``senha para acessar o banco`` => spring.datasource.password=
  - vazio pois ainda estar em desenvolvimento

``Configurações para a JPA`` => spring.jpa.hibernate.ddl-auto=update
  - estrategia que o hibernate, implementação da JPA, vai utilizar para criar as tabelas no banco de dados.
  - update => verifica as entidades e atualiza o banco de acordo com as entidades

``exibição no terminal`` => spring.jpa.show-sql=true
- true => Sempre que executar uma operação no banco de dados, as SQL será apresentada no terminal (log)

``console do H2`` => spring.h2.console.enabled=true
- true => Ter acesso a uma interface do H2

==> Print de como deve ficar as configurações:
<img width="100%" height="350" src="./geral/H2_database-config.png"></img>
==> Print do console do H2:
no navegador: http://localhost:8080/h2-console
<img width="100%" height="350" src="./geral/H2_database.png"></img>



## Tecnologias utilizadas

<a href="https://www.java.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a>  <a href="https://code.visualstudio.com/" target="_blank"> <img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Visual_Studio_Code_1.35_icon.svg" alt="androidStudio" width="40" height="30"/> </a> <a href="https://www.thymeleaf.org/" target="_blank"> <img src="https://www.thymeleaf.org/images/thymeleaf.png" alt="firebase" width="40" height="40"/> </a> 
<a href="https://getbootstrap.com/docs/5.0/getting-started/introduction/" target="_blank"> <img src="https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/themes/3067767/settings_images/omx3KZGSamzipD0jXUwg_file.jpg" alt="firebase" width="50" height="40"/> </a> 
<a href="https://maven.apache.org/" target="_blank"> <img src="https://cdn.icon-icons.com/icons2/2107/PNG/512/file_type_maven_icon_130397.png" alt="firebase" width="40" height="40"/> </a> <a href="https://spring.io/projects/spring-data-jpa/" target="_blank"> <img src="https://devcolibri.com/wp-content/uploads/2017/11/dfdfds.png" alt="firebase" width="40" height="40"/> </a> <a href="https://spring.io/projects/spring-boot/" target="_blank"> <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR5gJvZf4YCHHKfc4X3DsufIko_fRqeXsxCDuefw7QVkQ&s" alt="firebase" width="40" height="40"/> </a> <a href="https://www.h2database.com/html/main.html" target="_blank"> <img src="https://www.h2database.com/html/images/h2-logo-2.png" alt="firebase" width="50" height="40"/> </a>


- `Java 17`: Utilizando a versão mais recente do Java, o projeto se beneficia das últimas melhorias de desempenho, segurança e funcionalidades da linguagem.
- `Spring Boot`: O framework Spring Boot proporciona uma arquitetura simplificada e pronta para uso, agilizando o desenvolvimento e facilitando a manutenção do sistema.
- `VS Code`: A escolha do Visual Studio Code como ambiente de desenvolvimento ressalta o foco na produtividade e na facilidade de integração com as tecnologias utilizadas.
- `H2 Database`: O banco de dados H2 oferece uma solução leve e eficiente para armazenar dados, sendo ideal para desenvolvimento e testes.
- `Thymeleaf`: O Thymeleaf é utilizado para a criação de templates dinâmicos, permitindo uma apresentação elegante e interativa das informações no frontend.
- `Data-JPA`: O uso do módulo Data-JPA do Spring simplifica a interação com o banco de dados, proporcionando uma camada de abstração que facilita a manipulação dos dados.
- `Maven`: O sistema de gerenciamento de dependências Maven simplifica o processo de construção, distribuição e documentação do projeto.
- `Spring Web`: A implementação do Spring Web viabiliza o desenvolvimento de endpoints RESTful, proporcionando uma comunicação eficiente entre o frontend e o backend.



## Funcionalidades do projeto

- `Cadastro de Tarefas`: Os usuários podem inserir novas tarefas, especificando detalhes como `Título` e `Data entrega`. Essa funcionalidade fornece uma entrada rápida e fácil para todas as atividades planejadas. O sistema também grava a data em que a tarefa foi cadastrada no sistema.
<img width="100%" height="250" src="./geral/Cadastrar_tarefa.png"></img>

- `Excluir Tarefas`: A possibilidade de excluir tarefas oferece flexibilidade aos usuários para remover itens que não são mais relevantes ou necessários. Isso mantém a lista de tarefas organizada e focada nas atividades atuais. Além de aparecer uma notificação para confirmar se realmente deseja realizar a exclusão da tarefa, evitando assim um retrabalho.
<img width="100%" height="300" src="./geral/Excluir_tarefa.png"></img>

- `Editar Tarefas`: A capacidade de editar tarefas permite aos usuários realizar ajustes ou adicionar informações adicionais conforme necessário. Essa funcionalidade é crucial para manter as informações atualizadas e refletir qualquer mudança nos requisitos ou prazos.
<img width="100%" height="300" src="./geral/Editar_tarefa.png"></img>

- `Listar de Tarefas`: A visualização clara e organizada de todas as tarefas é essencial para o gerenciamento eficiente. A funcionalidade de listagem permite que os usuários vejam suas tarefas em uma interface fácil de entender, proporcionando uma visão global das responsabilidades.
<img width="100%" height="300" src="./geral/Listar_tarefas.png"></img>


## Benefícios do Projeto

- `Organização Eficiente`: Permite a criação, edição e exclusão de tarefas, possibilitando uma gestão eficaz do tempo e das atividades diárias.

- `Interface Intuitiva`: A interface desenvolvida com Thymeleaf oferece uma experiência amigável ao usuário, com recursos interativos para facilitar a interação com o sistema.

- `Segurança e Confiabilidade`: A integração do Spring Boot e a utilização do H2 Database garantem a segurança e confiabilidade na manipulação e armazenamento dos dados.

- `Facilidade de Extensão`: A estrutura modular do projeto, aliada ao uso do Maven, facilita a adição de novas funcionalidades e a manutenção do sistema ao longo do tempo. 


## Acesso ao projeto

É possível acessar o projeto através do [Link](https://github.com/Thamyresmya/TODO)

Neste repositório você tem acesso a todo o material desenvolvido.


## Desenvolvedores

| [<img src="https://github.com/Thamyresmya.png" width=115><br><sub>Thamyres Cavalcante</sub>](https://github.com/Thamyresmya) |   |
| :---: | :---: 



## Me siga nas redes sociais

- [Linkedin](https://www.linkedin.com/in/thamyrescavalcante/)
- [Instagran](https://www.instagram.com/thamyres__cavalcante/)

<br>

---

### Feito com 💜 by Thamyres Cavalcante.




