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
  
  ![observer](https://user-images.githubusercontent.com/31738300/97812836-01a71800-1c63-11eb-8db4-ca240b06339e.png)
  
* Participants:
  - Subject:
    - Classe que possui a informação do estado que se deseja observar.
  - Observer:
    - Interface que define os métodos de notificação de interesse dos observadores.
  - ConcreteObserverA, ConcreteObserverB:
    - Classes concretas que observam a classe Subject.
    
 - Sample Code:
    - [Código](https://github.com/aleboer/PadroesDeProjeto/tree/master/Composite/CompositeExemplo/src)
    - 
