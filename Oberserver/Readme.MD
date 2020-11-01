# Padrão Obeserver

* Pattern Name and Classification
  - Name: Observer
  - Classification: Comportamental


* Intent
  - Definir uma forma de comunicação entre classes.

* Motivation
  - O Oberver é usado para para que um objeto publique mudanças de estado.
  - O Observer, também permite que outros objetos se inscrevam para receber notificações sobre essa mudança de estados.

* Applicability
  - O Observer deve ser utilizado quando deseja monitorar mudanças de estado de um determinado objeto.

* Structure
  
  ![Observer](https://user-images.githubusercontent.com/31738300/93829660-82c2c680-fc44-11ea-8d80-69a9ca5b250e.png)
  
* Participants:
  - Component:
    - Declara interface para objetos da composição
    - Implementa comportamentos padrão comuns para todas as classes
    - Declara uma interface para acessar e gerenciar componentes filho
  - Leaf:
    - Representa objetos folha da consição que não tem filhos
    - Define o comportamento para objetos primitivos da composição
  - Composite:
    - Define o comportamento para componentes que possuem filhos
    - Armazena componentes filhos
    - Implementa operações relacionadas a filhos e definidas na interface Component
  - Client:
    - Manipula os objetos da composição via interface Component
    
 - Sample Code:
    - [Código](https://github.com/aleboer/PadroesDeProjeto/tree/master/Composite/CompositeExemplo/src)
    - Para exemplificar o padrão composite usei o exemplo do professor João Cunha em sala de aula e implementei um programa que cálcula o saldo do cliente levando em conta todas as suas contas (Corrente e poupança).
