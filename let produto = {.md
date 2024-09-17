let produto = {
nome: 'Notebook',
preco: 2500,
emEstoque: true
};
2. Divisão em Duplas
Forme duplas de alunos, onde um aluno escreve o código e o outro testa e ajuda a resolver
os problemas. Eles podem alternar os papéis durante a atividade.
3. Atividade: Gerenciando um Inventário Virtual
Cada dupla vai criar e manipular arrays e objetos para gerenciar o inventário de uma loja
fictícia. Eles precisarão realizar várias tarefas para adicionar, remover e modificar itens no
inventário.
Parte 1: Criando Arrays e Objetos
Cada dupla deve começar criando um array de produtos, onde cada produto será
representado por um objeto com as propriedades nome, preco, e emEstoque.
Exemplo inicial:
let inventario = [
  { nome: 'Teclado', preco: 100, emEstoque: true },
  { nome: 'Mouse', preco: 50, emEstoque: false },
  { nome: 'Monitor', preco: 600, emEstoque: true }
];

Tarefas Práticas:
Adicionar um novo produto ao inventário: A dupla deve usar o método .push() para adicionar
um novo produto ao array.
inventario.push({ nome: 'Cadeira Gamer', preco: 1200, emEstoque: true });

Remover o último produto do inventário: Usar o método .pop() para remover o último item.
inventario.pop();

Modificar o preço de um produto existente: A dupla deve alterar o preço de um dos
produtos, por exemplo, o "Teclado".
inventario[0].preco = 120;

Marcar um produto como fora de estoque: Alterar a propriedade emEstoque de "Monitor"
para false.
inventario[2].emEstoque = false;

Parte 2: Iterando sobre Arrays
Agora, a dupla vai aprender a iterar sobre o array de objetos para listar todos os produtos
ou realizar outras ações, usando o loop for.

Tarefas Práticas:
Exibir todos os produtos em estoque: Use o loop for para exibir apenas os produtos que
estão em estoque.
for (let i = 0; i < inventario.length; i++) {
 if (inventario[i].emEstoque) {
    console.log(inventario[i].nome + ' está em estoque.');
 }
}

Remover produtos fora de estoque: Use o método .filter() para criar um novo array com
apenas os produtos em estoque.
let produtosEmEstoque = inventario.filter(produto => produto.emEstoque);
console.log(produtosEmEstoque);