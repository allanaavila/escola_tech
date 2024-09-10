## Sistema de Gestão de Alunos, Turmas e Notas

## Descrição do Projeto

Este projeto é uma evolução da agenda de contatos desenvolvida no módulo anterior. Agora, a aplicação inclui a capacidade de gerenciar contatos, turmas e notas, com o objetivo de criar uma solução eficiente para o gerenciamento de dados acadêmicos em uma escola de tecnologia.

Utilizando princípios da programação orientada a objetos, o projeto adota uma estrutura de herança para organizar as classes. A classe **Contato** serve como base (classe pai), e as classes **Aluno** e **Professor** herdam suas funcionalidades e atributos, estendendo o comportamento para incluir dados específicos relacionados a cada tipo de usuário. Isso garante um código mais reutilizável e modular, facilitando a manutenção e a expansão futura do sistema.


## Link do Repositório:
[Repositório GitHub](https://github.com/allanaavila/escola_tech.git)

## Funcionalidades

### 1. **Gerenciamento de Contatos**
   - Adicionar, detalhar, editar e excluir contatos.
   - Contatos são usados como classe pai, proporcionando uma base para a herança de classes específicas, como Aluno e Professor.
   - Garantia de integridade dos dados com validação de duplicidade de números de telefone.

### 2. **Gerenciamento de Turmas**
   - Adição de turmas, permitindo associar um conjunto de alunos a cada turma.
   - Detalhamento de informações sobre turmas, incluindo alunos associados.
   - Modificação e exclusão de turmas, com tratamento de erros para dados inexistentes.

### 3. **Gerenciamento de Notas**
   - Atribuição de notas aos alunos de cada turma.
   - Visualização de médias e distribuição de notas por aluno ou turma.
   - Edição e remoção de notas, com validação para garantir a consistência das informações.

### 4. **Listagem de Dados**
   - Listagem completa de contatos, turmas e notas.
   - Tratamento de exceções quando não há dados a serem exibidos.


### Tecnologia Utilizada
- Java: Linguagem principal utilizada no desenvolvimento do sistema.
- Paradigma de Orientação a Objetos (POO): Implementado para gerenciar as entidades Aluno, Turma e Nota.
- Coleções Java: Utilização de List para armazenamento de alunos, turmas e notas.

  ### Estrutura do Projeto
```plaintext
├── src
│   ├── controller
│   │   ├── ControllerAluno.java
│   │   ├── ControllerTurma.java
│   │   ├── ControllerNota.java
│   ├── model
│   │   ├── Aluno.java
│   │   ├── Contato.java
│   │   ├── Turma.java
│   │   ├── Nota.java
│   ├── util
│   │   └── Validacoes.java
│   ├── Main.java
├── README.md 


### Execução do Projeto
## Clone o repositório:
 ```bash
git clone https://github.com/seu-usuario/sistema-gestao-escolar-java.git
```
   - Compile o projeto com o seu ambiente de desenvolvimento Java (Eclipse, IntelliJ, etc.).
   - Execute a classe Main.java para iniciar o sistema.


## Arquitetura do Projeto

Este projeto utiliza o conceito de herança da Programação Orientada a Objetos. A classe **Contato** serve como a classe base (pai), 
fornecendo atributos e métodos comuns como nome, telefone e e-mail. As classes **Aluno** e **Professor** herdam esses atributos e comportamentos, 
estendendo-os com informações específicas, como notas para os alunos e disciplinas lecionadas para os professores. Essa abordagem permite um design mais flexível e modular, 
facilitando o crescimento futuro do sistema.
