# Solicitação de Banco de Dados

Data: 22/03/2020 <br>
Empresa: Clínica Análises Ltda. <br>
Cliente(s): Davi Amaral, Ryan Moraes <br>

<p>
	Caro Sr. Marcello Novaes,
<br>
<br>
	Boa noite. Nós da Clínica Análises somos uma nova empresa especializada em exames laboratoriais, e nos interessamos por seus serviços de criação e organização de banco de dados; gostaríamos, então, de contratá-lo. Recentemente, começamos a receber uma quantidade maior de clientes, mais do que nossa antiga capacidade de gerenciamento. Estamos expandindo a empresa, mas precisamos de um banco de dados personalizado para facilitar a busca de exames de cada um de nossos pacientes. Por exemplo, no caso de um exame de sangue de rotina, antes da coleta é requisitado ao paciente seu:
	<ul>
		<li> CPF
		<li> RG
		<li> Número de telefone
		<li> Telefone fixo
		<li> E-mail
		<li> Endereço
		<li> Tipos de exames
	</ul>
	Necessitamos, portanto, de um banco de dados que atenda à essas entidades. Um protocolo único será entregue ao paciente para a busca dos exames com a data prevista do resultado, e caso o paciente prefira receber o resultado em sua residência ou houver algum compromisso no dia de entrega, o protocolo terá um link que, copiado em um navegador da internet, levará o cliente até uma página de entrada aonde precisa apenas inserir seu login e senha do protocolo, e poderá então clicar na opção de imprimir os exames do paciente.
<br>
<br>
	Caso algo de errado apareça em algum exame, será feito uma busca no banco de dados para resgatar o número de telefone do paciente e a listagem dos exames do dia em que foi feito. Cada paciente tem um número de protocolo único gerado pelo sistema; o funcionário que colheu sangue ou atendeu o paciente irá telefonar para o cliente explicando a situação do exame, e que será feito uma nova coleta de sangue. Caso um paciente perca o protocolo, será necessário ir ao laboratório explicar a situação e mostrar sua identidade ou CPF, para que seja feito uma busca no banco de dados. Quando digitado o CPF ou nome completo, irão aparecer os resultados da busca do exame do paciente, e assim sendo, será impresso e entregue ao cliente.
</p>

# Normalização de Dados

<i>Primeira Forma Normal (1FN):</i> Nenhum atributo deve possuir mais de um valor, e nenhuma tabela pode possuir valores repetidos. Cada valor deve ser único e exclusivo. Sua normalização dá-se por:
	<ol>
		<li> Identificar a chave primária e a coluna que possui dados repetidos, e removê-los.
		<li> Construir uma outra tabela com o atributo em questão, estabelecendo uma relação entre a nova e a anterior.
	</ol>
<i>Segunda Forma Normal (2FN):</i> É necessário satisfazer a 1FN para proseguir para a 2FN. Essa forma define que os atributos normais devem depender apenas da chave primária da tabela. Para colunas não dependentes dessa chave, deve-se movê-las para uma nova tabela. Sua normalização dá-se por:
	<ol>
		<li> Identificar os dados não dependentes da chave primária, e removê-los.
		<li> Construir uma outra tabela com os dados em questão.
	</ol>
<i>Terceira Forma Normal (3FN):</i> É necessário satisfazer 2FN e, por conseguinte, a 1FN para proseguir para a 3FN. Todos os atributos de uma tabela devem ser simultaneamente independentes uns dos outros, e dependentes exclusivamente da chave primária. Sua normalização dá-se por:
	<ol>
		<li> Identificar os dados dependentes de outros, e removê-los.
	</ol>
