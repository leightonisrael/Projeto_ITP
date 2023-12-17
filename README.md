# Projeto 3ª Unidade da matéria de Introdução às Técnicas de Programação - T06 - UFRN - 2023.2

<h1>Sistema de Reservas de Assentos em Teatro</h1>
<p>Este projeto consiste na implementação de um programa em linguagem C para gerenciar a reserva de assentos em um teatro. Os assentos são representados por uma matriz, onde cada assento é uma struct com informações como estado de reserva, fileira, número e nome do ocupante (em caso de reserva).</p>

<h2>Funcionalidades Principais</h2>

<h3>Gerenciamento de Teatro e Assentos</h3>

<h4>Inicialização da Matriz:</h4>
<p>
- Função <code>inicializarMatriz</code> aloca e inicializa a matriz de assentos.<br>
- Restrições de no máximo 26 linhas (A-Z) e 99 colunas.<br>
- Retorna <code>NULL</code> se as dimensões excederem as restrições.
</p>

<h4>Criação do Teatro:</h4>
<p>
- Função <code>criarTeatro</code> cria dinamicamente um Teatro com uma matriz de assentos.<br>
- Utiliza a função <code>inicializarMatriz</code> para alocar a matriz.
</p>

<h4>Exibição do Teatro:</h4>
<p>
- Função <code>exibirTeatro</code> apresenta o estado atual da matriz de assentos de forma clara.
</p>

<h4>Liberar Matriz:</h4>
<p>
- Função <code>liberarMatriz</code> desaloca a memória da matriz de assentos.
</p>
<h3>Reservas e Cancelamentos</h3>

<h4>Reserva de Assento:</h4>
<p>
- Função <code>reservarAssento</code> reserva um assento específico se estiver disponível.
</p>

<h4>Reserva de Assentos Consecutivos:</h4>
<p>
- Função <code>reservarAssentosConsecutivos</code> reserva n assentos consecutivos a partir de uma posição.
</p>

<h4>Reserva de Assento pelo Sistema:</h4>
<p>
- Função <code>reservarAssentoPeloSistema</code> reserva um assento disponível, evitando problemas futuros.
</p>

<h4>Reserva de Assentos Consecutivos pelo Sistema:</h4>
<p>
- Função <code>reservarAssentosConsecutivosPeloSistema</code> reserva n assentos consecutivos para um grupo, com estratégias para evitar conflitos.
</p>

<h4>Cancelamento de Reservas:</h4>
<p>
- Função <code>cancelarReserva</code> cancela a reserva de um assento específico.<br>
- Função <code>cancelarReservas</code> cancela todas as reservas de uma pessoa.<br>
- Função <code>cancelarTodasAsReservas</code> cancela todas as reservas disponíveis.
</p>

<h3>Consultas e Estatísticas</h3>

<h4>Verificação de Disponibilidade:</h4>
<p>
- Função <code>verificarDisponibilidade</code> verifica se um assento está disponível.
</p>

<h4>Consulta de Assentos Consecutivos:</h4>
<p>
- Função <code>consultarAssentosConsecutivos</code> exibe os intervalos com pelo menos n assentos disponíveis.
</p>

<h4>Exibição de Informações:</h4>
<p>
- Função <code>exibirInformacoes</code> calcula e exibe informações sobre reservas, espaços livres, sequências de assentos, etc.
</p>

<h3>Armazenamento</h3>

<h4>Salvar e Carregar Estado:</h4>
<p>
- Função <code>salvarEstado</code> salva o estado do Teatro em um arquivo.<br>
- Função <code>carregarEstado</code> carrega o estado do Teatro a partir de um arquivo, alocando nova matriz se necessário.
</p>

<h3>Funcionamento do Programa</h3>

<p>
- A função <code>main</code> lê as dimensões da matriz, cria o Teatro e processa operações conforme entrada do usuário.<br>
- Operações incluem salvar e carregar estado, visualização, reserva, cancelamento, verificação de disponibilidade, consultas e exibição de informações.
</p>