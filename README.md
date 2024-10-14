
## Curso Bacharelado em Sistemas de Informação 
### Disciplina de Estruturas de Dados 
**Professor:** MSc. Ricardo Nunes  
**Contato:** ricardo@ifal.edu.br  

## Mini-projeto 1: Implementação de um Conjunto Usando Fila

### Descrição:
Neste projeto, implementamos uma estrutura de dados de conjunto (set) utilizando uma fila (Queue). O objetivo é garantir que não haja elementos duplicados na estrutura.

### Datas de Realização e Entrega:
- **Início:** 07/10
- **Término:** 14/10

### Regras:
- Pode ser realizado individualmente ou em equipe com até 3 pessoas.
- Este mini-projeto é opcional.
- **Conteúdo a ser entregue:**
  - Arquivos do código-fonte ou um link (GitHub ou Replit).
  - Arquivo `README.md` contendo:
    - Integrantes da equipe.
    - Lista de fontes consultadas (sites, livros, artigos, códigos prontos, etc.).
    - Comentários da equipe sobre o que foi ou não realizado.
    - Problemas ou dificuldades encontradas no código ou nas funcionalidades.
  - Discussão sobre o desempenho das operações implementadas na estrutura.

### Atividades:
1. **Implementação de `SetWithQueue`:**
   - Criar a estrutura `SetWithQueue` utilizando uma fila (Fila_Array) para armazenar elementos.
   - **Operações obrigatórias:**
     - `add(element)`: Adiciona um elemento ao conjunto (sem duplicados).
     - `remove(element)`: Remove um elemento do conjunto (lança exceção se o elemento não existir).
     - `contains(element)`: Retorna `True` se o elemento existir, `False` caso contrário.
     - `size()`: Retorna o número de elementos no conjunto.
     - `list()`: Retorna todos os elementos do conjunto.

2. **Discussão sobre Desempenho:**
   - Incluir no arquivo `README.md` uma análise sobre o desempenho de cada operação (`add`, `remove`, `contains`, etc.).

### Critérios de Avaliação:
1. O código deve executar sem erros.
2. A implementação deve utilizar a estrutura "Fila_Array" como base para o `SetWithQueue`.
3. Atender à especificação solicitada.
4. Passar nos testes fornecidos.
5. Discutir o desempenho das operações implementadas.
6. Incluir todas as referências consultadas.

### Conjunto de Testes:
Utilize o código de teste fornecido pelo professor para verificar se a implementação está correta. O código dos testes pode ser encontrado no link: [set_with_queue_tests.py](https://github.com/ricardo9n/estd/blob/main/mp-testes/set_with_queue_tests.py).

### Execução dos Testes:
Para rodar os testes, utilize um ambiente Python. Os testes validam se as operações (`add`, `remove`, `contains`, etc.) estão funcionando conforme o esperado, utilizando a função `assert`.

### Considerações Finais:
Este mini-projeto oferece a oportunidade de aprofundar o conhecimento sobre estrutura de dados e manipulação de filas, além de testar habilidades em codificação e análise de desempenho.

### Agradecemos às seguintes pessoas que contribuíram para este projeto:

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/robertoferreira7">
        <img src="https://github.com/robertoferreira7.png" width="100px;" alt="Foto de perfil do Roberto Ferreira de Assis Filho no GitHub"/><br>
        <sub>
          <b>Roberto Ferreira de Assis Filho</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/rodrigo-farias10">
        <img src="https://github.com/rodrigo-farias10.png" width="100px;" alt="Foto de perfil do Rodrigo de Oliveira Farias no GitHub"/><br>
        <sub>
          <b>Rodrigo de Oliveira Farias</b>
        </sub>
      </a>
    </td>
  </tr>
</table>
