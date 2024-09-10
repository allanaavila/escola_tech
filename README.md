## Sistema de Gestão de Alunos, Turmas e Notas

## Descrição do Projeto

Este projeto é uma evolução da agenda de contatos desenvolvida no módulo anterior. Agora, a aplicação inclui a capacidade de gerenciar contatos, turmas e notas, com o objetivo de criar uma solução eficiente para o gerenciamento de dados acadêmicos em uma escola de tecnologia.

Utilizando princípios da programação orientada a objetos, o projeto adota uma estrutura de herança para organizar as classes. A classe **Contato** serve como base (classe pai), e as classes **Aluno** e **Professor** herdam suas funcionalidades e atributos, estendendo o comportamento para incluir dados específicos relacionados a cada tipo de usuário. Isso garante um código mais reutilizável e modular, facilitando a manutenção e a expansão futura do sistema.


## Link do Repositório:
[Repositório GitHub](https://github.com/allanaavila/escola_tech.git)

## Funcionalidades

### Menu Geral da Escola Tech
     ```plaintext
      ╔══════════════════════════════╗
      ║       ESCOLA TECH            ║
      ╠══════════════════════════════╣
      ║  1 - Menu das Turmas         ║
      ║  2 - Menu dos Alunos         ║
      ║  3 - Lançar Notas            ║
      ║  4 - Buscar Nota do Aluno    ║
      ╠══════════════════════════════╣
      ║  0 - Sair                    ║
      ╚══════════════════════════════╝
     ```

### 1. **Gerenciamento de Alunos**
   - Adicionar, detalhar, editar e excluir alunos.
   - Contatos são usados como classe pai, proporcionando uma base para a herança de classes específicas, como Aluno e Professor.
   - Garantia de integridade dos dados com validação de duplicidade de números de telefone.
     ** Menu de Cadastro de Alunos
     ```plaintext
      ╔══════════════════════════════╗
      ║      CADASTRO DE ALUNOS      ║
      ╠══════════════════════════════╣
      ║  1 - Cadastrar Aluno         ║
      ║  2 - Detalhar Aluno          ║
      ║  3 - Alterar Aluno           ║
      ║  4 - Remover Aluno           ║
      ║  5 - Listar Alunos           ║
      ╠══════════════════════════════╣
      ║  0 - Menu Principal          ║
      ╚══════════════════════════════╝
     ```

### 2. **Gerenciamento de Turmas**
   - Adição de turmas, permitindo associar um conjunto de alunos a cada turma.
   - Detalhamento de informações sobre turmas, incluindo alunos associados.
   - Modificação e exclusão de turmas, com tratamento de erros para dados inexistentes.
     
      ** Menu de Cadastro de Turmas
     ```plaintext
      ╔══════════════════════════════╗
      ║     CADASTRO DE TURMAS       ║
      ╠══════════════════════════════╣
      ║  1 - Cadastrar Turmas        ║
      ║  2 - Detalhar Turmas         ║
      ║  3 - Alterar Turmas          ║
      ║  4 - Remover Turmas          ║
      ║  5 - Listar Alunos por Turma ║
      ╠══════════════════════════════╣
      ║  0 - Menu Principal          ║
      ╚══════════════════════════════╝
     ```

### 3. **Gerenciamento de Notas**
   - Atribuição de notas aos alunos de cada turma.
   - Visualização de médias e distribuição de notas por aluno ou turma.
   - Edição e remoção de notas, com validação para garantir a consistência das informações.

     ** Menu de Cadastro de Notas
     ```plaintext
      ╔══════════════════════════════╗
      ║       LANÇAR NOTAS           ║
      ╠══════════════════════════════╣
      ║  1 - Adicionar Notas         ║
      ║  2 - Detalhar Notas          ║
      ║  3 - Alterar Notas           ║
      ║  4 - Remover Notas           ║
      ║  5 - Listar APROVADOS        ║
      ╠══════════════════════════════╣
      ║  0 - Menu Principal          ║
      ╚══════════════════════════════╝
     ```

### 4. **Listagem de Dados**
   - Listagem completa de contatos, turmas e notas.
   - Tratamento de exceções quando não há dados a serem exibidos.


### Tecnologia Utilizada
- Java: Linguagem principal utilizada no desenvolvimento do sistema.
- Paradigma de Orientação a Objetos (POO): Implementado para gerenciar as entidades Aluno, Turma e Nota.
- Coleções Java: Utilização de List para armazenamento de alunos, turmas e notas.


## Estrutura do Projeto
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
git clone https://github.com/seu-usuario/sistema-gestao-escolar-java.git

   - Compile o projeto com o seu ambiente de desenvolvimento Java (Eclipse, IntelliJ, etc.).
   - Execute a classe Main.java para iniciar o sistema.
```

## Arquitetura do Projeto

Este projeto utiliza o conceito de herança da Programação Orientada a Objetos. A classe **Contato** serve como a classe base (pai), 
fornecendo atributos e métodos comuns como nome, telefone e e-mail. As classes **Aluno** e **Professor** herdam esses atributos e comportamentos, 
estendendo-os com informações específicas, como notas para os alunos e disciplinas lecionadas para os professores. Essa abordagem permite um design mais flexível e modular, 
facilitando o crescimento futuro do sistema.
