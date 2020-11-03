# Padrão Memento

* Pattern Name and Classification
  - Name: Memento
  - Classification: Comportamental


* Intent
  - Capturar e externalizar um estado interno de um objeto, de maneira que o objeto possa ser restaurado para esse estado mais tarde.

* Motivation
  - O Memento é usado para registrar o estado interno de um objeto para implementação de mecanismos de checkpoints e para desfazer operações no caso de erros.

* Applicability
  - O Memento deve ser utilizado quando deseja criar pontos de restauração ou para o programa se recuperar de erros.

* Structure
  
  ![memento](https://user-images.githubusercontent.com/31738300/97938072-34ced180-1d5f-11eb-8a83-77a983f3fac9.png)
  
* Participants:
  - Memento:
    - classe que representa um snapshot, contendo o estado de um objeto a ser restaurado em um Originador. Possui métodos para obter e definir o estado que um Memento encapsula dentro.
  - Originador:
    - classe na qual o estado atual é mantido. Define método que permite criar um Memento com o estado atual do Originador armazenado no Memento retornado. Originator também tem um método que define seu estado atual com o estado de um determinado objeto Memento. Portanto, pode criar um Snapshot (Memento) ou restaurar o estado do Snapshot fornecido (Memento).
  - Caretaker:
    - classe auxiliar responsável por armazenar restaurar o estado do Originador por meio do objeto Memento. Um objeto Caretaker mantém os Mementos, mas nunca modifica os Mementos.
    
 - Sample Code:
    - [Código](https://github.com/aleboer/PadroesDeProjeto/blob/master/Memento/MementoExemplo/Main.java)
