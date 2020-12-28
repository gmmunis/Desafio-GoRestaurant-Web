<h1>🚀 Sobre o desafio</h1>
<p>Nesse desafio, você irá desenvolver mais uma aplicação, a GoRestaurant. Agora você irá praticar o que você aprendeu até agora no React.js junto com TypeScript, praticando o conceito de CRUD (Create, Read, Update, Delete).</p>
<p>Essa será uma aplicação que irá se conectar a uma fake API, e exibir os pratos de comida criados e permitir a criação, remoção e atualização desses pratos.</p>
<p>Agora navegue até a pasta criada e abra no Visual Studio Code, lembre-se de executar o comando yarn no seu terminal para instalar todas as dependências.</p>
<h3>Utilizando uma fake API</h3>
<p>Antes de tudo, para que você tenha os dados para exibir em tela, criamos um arquivo que você poderá utilizar como fake API para te prover esses dados.</p>
<p>Para isso, deixamos instalado no seu package.json uma dependência chamada json-server, e um arquivo chamado server.json que contém os dados para uma rota /foods. Para executar esse servidor você pode executar o seguinte comando:</p>
<pre>yarn json-server server.json -p 3333</pre>
<h3>Funcionalidades da aplicação</h3>
<p>Agora que você já está com o template clonado e pronto para continuar, você deve verificar os arquivos da pasta src e completar onde não possui código, com o código para atingir os objetivos de cada rota.</p>
<ul>
<li><strong>Listar os pratos de comida da sua API:</strong> Sua página Dashboard deve ser capaz de exibir uma listagem, com o campo title, value, e description e available de todos os pratos de comida que estão cadastrados na sua API.</li>
<br />
<p><strong>Dica:</strong> Para exibir se o prato de comida está disponível ou não, você pode validar o campo available que é retornado da API e exibir Disponível caso seja true, e Indisponível caso seja false.</p>
<br />
<li><strong>Adicionar novos pratos de comida a sua API:</strong> Em sua página Dashboard você deve abrir um modal ao clicar no botão Novo Prato no Header. Esse modal deve ser responsável por cadastrar uma nova food passando os campos image, name, description, value.</li>
<br />
<p><strong>Dica 1:</strong> O campo image deve ser uma URL, deixamos três URL de imagens como exemplo no arquivo server.json.</p>
<p><strong>Dica 2:</strong> Ao enviar o request para sua API para salvar a food, lembre-se sempre de setar o campo available como true.</p>
<li><strong>Editar pratos de comida da sua API:</strong> Em sua página Dashboard você deve abrir um modal ao clicar no botão Editar Prato. Esse modal deve ser responsável por editar uma food passando os campos image, name, description, value.</li>
<p><strong>Dica:</strong> Ao editar um item, quando for envia-lo para o backend, lembre de copiar os dados anteriores como o available e o id, ou eles serão perdidos do seu arquivo server.json.</p>
<li>Remover pratos de comida da sua API: Em sua página Dashboard você deve remover um prato de comida ao clicar no botão com ícone de lixeira no componente Food.</li>
<p>Dica: Após remover o item da sua API, lembre-se de remover ele também da listagem.</p>
<li>Alterar disponibilidade dos pratos de comida da sua API: Em sua página Dashboard você deve alterar a disponibilidade de um prato de comida ao clicar no switch que é controlado pelo valor de available.</li>
</ul>
<h3>Específicação dos testes</h3>
<p>Em cada teste, tem uma breve descrição no que sua aplicação deve cumprir para que o teste passe.</p>
<p>Para esse desafio, temos os seguintes testes:</p>
<ul>
<li><strong>should be able to list all the food plates from your api:</strong> Para que esse teste passe, sua aplicação deve permitir que sejam listados, toda os pratos de comidas que são retornadas da sua fake API.</li>
<li><strong>should be able to add a new food plate:</strong> Para que esse teste passe, você deve permitir que um prato de comida seja adicionado a sua api, adicionando-o também à listagem.</li>
<li><strong>should be able to edit a food plate:</strong> Para que esse teste passe, você deve permitir que um prato de comida seja editado na sua api, editando-o também na listagem.</li>
<li><strong>should be able to remove a food plate:</strong> Para que esse teste passe, você deve permitir que um prato de comida seja removido da sua api, removendo-o também da listagem.</li>
<li><strong>should be able to update the availibility of a food plate:</strong> Para que esse teste passe, em sua dashboard você deve permitir que o status do prato de comida seja alterado entre Disponível e Indisponível;</li>
</ul>
