INTEGRANTES DA EQUIPE
Roberto Ferreira de Assis Filho (@robertoferreira7)
Rodrigo de Oliveira Farias (@rodrigo-farias10)

COMENT�RIOS DA EQUIPE
O c�digo da classe SetWithQueue desenvolvido atende ao desafio proposto, usando a classe FilaArray como estrutura para armazenar elementos de forma ordenada e garantir que n�o haja duplicatas. A fun��o add(element) assegura a aus�ncia de duplicidade ao verificar se o elemento j� est� presente antes de enfileir�-lo, usando o m�todo contains(element), que faz a busca linear pelo elemento na fila. A opera��o remove(element) retira o elemento especificado, criando uma fila tempor�ria para manter a ordem dos elementos restantes, mantendo a integridade da estrutura. A opera��o contains(element) permite verificar a exist�ncia de um elemento no conjunto, enquanto size() retorna o n�mero total de elementos e list() devolve todos os elementos armazenados em ordem, sem modific�-los. Essas opera��es garantem que o conjunto funcione conforme especificado, mantendo o comportamento e as caracter�sticas de um conjunto, mas com as caracter�sticas de uso de uma fila como estrutura de armazenamento.
O c�digo apresenta uma implementa��o funcional, por�m enfrenta alguns problemas de efici�ncia e limita��es. A remo��o de elementos, que preserva a ordem original, requer a cria��o de uma fila tempor�ria, resultando em uma complexidade ??(??) para a opera��o de dequeue, o que pode ser ineficiente para grandes conjuntos. Al�m disso, a verifica��o de duplicidade atrav�s do m�todo contains tamb�m � linear, ??(??), o que se contrap�e com a efici�ncia ??(1) esperada em estruturas de dados tradicionais de conjunto, como o set em Python. Embora o c�digo inclua m�todos essenciais como add, remove, contains, size e list, ele poderia ser melhorado, por exemplo, com um m�todo para facilitar a itera��o sobre os elementos. Esses pontos sugerem que, embora a implementa��o atenda aos requisitos b�sicos e passe nos testes fornecidos, ela pode n�o ser a mais eficiente ou adequada para cen�rios que exijam alta performance.



ATIVIDADE 01: IMPLEMENTAR SetWihQueue
A implementa��o de SetWithQueue est� no reposit�rio https://github.com/robertoferreira7/mini_projeto_filas.git no arquivo projeto_fila.py.
ATIVIDADE 02: DISCUSS�O SOBRE DESEMPENHO
Para analisar a complexidade das fun��es na classe SetWithQueue, deve-se considerar a implementa��o de cada m�todo e como ele interage com a estrutura FilaArray. Sendo FilaArray uma fila que utiliza uma lista para armazenar os elementos, a seguir encontra-se a complexidade de cada m�todo desenvolvido na classe SetWithQueue.
Complexidade de cada m�todo:
add(element): inicialmente, o m�todo chama contains(element), que verifica se o elemento j� est� na fila. Essa opera��o tem complexidade O(n), pois percorre a lista para encontrar o elemento. Se o elemento n�o estiver presente, o m�todo chama enqueue(element) para adicionar o elemento ao final da fila, que � uma opera��o O(1). Logo, a complexidade de add(element) � O(n) devido � chamada para contains.
remove(element): o m�todo chama contains(element) para verificar se o elemento est� na fila, o que � O(n). Se o elemento estiver presente, ele cria uma fila tempor�ria (temp_queue) e usa um loop para realizar o dequeue de todos os elementos da fila original e reenfileirar aqueles que n�o correspondem ao elemento a ser removido. O dequeue() e enqueue() s�o ambos O(1) em uma lista. Como percorre todos os elementos da fila, a complexidade desse loop � O(n), resultando em uma complexidade total de O(n) para o m�todo remove(element).
contains(element): este m�todo percorre todos os elementos na fila subjacente para verificar a presen�a do elemento. A complexidade � O(n).
size(): este m�todo simplesmente retorna o tamanho da lista subjacente da fila. Sendo size() no FilaArray uma opera��o constante, a complexidade � O(1).
list(): a complexidade de list() na classe SetWithQueue � O(1), j� que ele retorna diretamente a lista sem realizar qualquer processamento adicional.
Os m�todos que envolvem a verifica��o de elementos na fila, como add, remove e contains, t�m complexidade O(n), pois precisam percorrer a lista para localizar ou remover elementos. J� size e list s�o opera��es r�pidas, com complexidade O(1).
CONTE�DO CONSULTADO PARA A REALIZA��O DO PROJETO
https://www.ufsm.br/pet/sistemas-de-informacao/2020/04/01/entendendo-listas-pilhas-e-filas
http://sites.poli.usp.br/p/fabio.cozman/Didatico/Comp/Material/estruturas.pdf
https://docente.ifsc.edu.br/vilson.junior/ed/04_Listas_Filas_Pilhas.pdf
https://pessoal.dainf.ct.utfpr.edu.br/maurofonseca/lib/exe/fetch.php?media=cursos:if63c:if63ced_03_pilhasfilas.pdf
