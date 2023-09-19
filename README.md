# NumberAnalyzer
Exercício sugerido pelo curso básico do Curso em Video do professor Gustavo Guanabara.
A aplicação irá analisar o número que será adicionado pelo usuário.

### Seleção de elementos HTML:
- O código começa selecionando três elementos HTML usando o método `document.querySelector()`. Esses elementos são identificados pelos seus IDs:
  - `num`: um elemento de entrada (`<input>`) com o ID "fnum".
  - `lista`: um elemento de seleção (`<select>`) com o ID "flista".
  - `res`: um elemento de divisão (`<div>`) com o ID "res".

### Array para armazenar valores:
- O código cria uma variável chamada `valores` como um array vazio. Este array será usado para armazenar os valores digitados pelo usuário.

### Função `isNumero()`:
- Esta função recebe um parâmetro `n`.
- Verifica se o valor passado é um número entre 1 e 100.
- Retorna `true` se for um número válido e `false` caso contrário.

### Função `inLista()`:
- Esta função recebe dois parâmetros: um número `n` e um array `l`.
- Verifica se o número `n` está presente no array `l` usando o método `indexOf()`.
- Retorna `true` se o número estiver na lista e `false` caso contrário.

### Função `adicionar()`:
- Esta função é chamada quando o usuário clica em um botão ou realiza alguma ação para adicionar um valor.
- Verifica se o valor inserido no elemento `num` é um número válido e não está na lista `valores`.
- Se for válido e não estiver na lista, adiciona o valor ao array `valores` e cria um elemento de opção (`<option>`) com o texto indicando que o valor foi adicionado à lista.
- Limpa o conteúdo da divisão `res` (para atualização futura).
- Se o valor não for válido ou já estiver na lista, exibe um alerta.

### Função `finalizar()`:
- Esta função é chamada quando o usuário decide finalizar o processo.
- Verifica se pelo menos um valor foi adicionado à lista `valores`.
- Se a lista estiver vazia, exibe um alerta pedindo ao usuário para adicionar um valor primeiro.
- Caso contrário, calcula várias estatísticas dos valores na lista, como a quantidade total, o maior valor, o menor valor, a soma de todos os valores e a média.
- Atualiza o conteúdo da divisão `res` com as estatísticas calculadas.

Em resumo, esse código é uma aplicação simples que permite ao usuário adicionar números a uma lista, calcular várias estatísticas sobre esses números e exibir os resultados na página HTML. Ele usa funções JavaScript para validar os números e executar os cálculos.
