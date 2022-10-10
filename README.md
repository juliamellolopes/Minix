<h1 align="center">Sistema Operacional Minix</h1>

<p> 
Para ler mais informações sobre o trabalho, acesse [WIKI](https://github.com/juliamellolopes/Minix/wiki)
</p>

# Chaveamento de Processos ou Troca de Contexto

<p> 

<h3> O que é? </h3>

Chaveamento de um processo ou como conhecido também como mudança/troca de contexto é o processo computacional de armazenar e restaurar as informações necessárias do estado de uma CPU para que mais de um processo possa utilizar a CPU em uma única instância a partir do ponto que o processo foi interrompido. 

Normalmente, o chaveamento de processo ocorre sempre que um novo processo é selecionado para ser executado. 

<h3> Quando Chavear um Processo?  </h3> 

- Quando o tempo (Quantum) de posse da CPU expirou - principalmente quando usa o escalonador Roud-Robin;
- Quando há interrupção de Entrada e Saída;

<h3> Interrupções do lado do núcleo do Minix </h3> 

O Byte de dado é usado como índice numa tabela de handlers, onde cada handler implementa um tratamento a ser chamado utilizando alguns parâmetros:

- Um ponteiro para uma área na memória;
- Registradores;
- Método mixto;

Ao ser executado, o handler efetua a troca de texto. 

<h3> Ações no Chaveamento  </h3> 

Primeiro precisamos salvar o contexto do processador, incluindo o PC e outros registradores. Assim pode-se alterar o BCP (Bloco de controle de processo) do processo que está no estado “em-execução” e movê-lo para uma fila apropriada e selecionar outro processo para execução. Logo após altera-se o BCP do processo selecionado e as tabelas de gerência de memória e por fim restauramos o contexto do processo anterior selecionado.

</p>

# Gerência de Arquivos

<p> Os arquivos, no geral, são uma forma de armazenar informações em disco. Ou seja, quando um processo está sendo executado, ele armazena informações e, quando esse mesmo processo é finalizado, toda a informação acaba sendo perdida. Porém, se as informações forem gravadas em formato de arquivo, elas poderão ser lidas e utilizadas por outros processos novamente.

Como em qualquer sistema de arquivos, o sistema de arquivos do MINIX deve alocar e desalocar o espaço para os arquivos, monitorar blocos de disco e liberar espaço, oferecer alguma maneira de proteger arquivos contra uso não-autorizado. </p>


# Denvolvedores 
<p>

- Lívia Gonçalves
- Júlia Mello
- Pedro Henrique Pires Dias
- Celso Vinícius

</p>

# Contato

<div>

<div>
 
<p align="justify"> Lívia Gonçalves </p>
<a href="https://t.me/livia_goncalves">
<img align="center" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"/> 

</div>
 
<div>
 
<p align="justify"> Júlia Mello </p>
<a href="https://t.me/juliamello">
<img align="center" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"/> 

</div>

<div>
 
<p align="justify"> Pedro Henrique Pires Dias </p>
<a href="https://t.me/phpdias">
<img align="center" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"/> 

</div>

<div>
 
<p align="justify"> Eduardo Grillo </p>
<a href="https://t.me/eduardogrilloo">
<img align="center" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"/> 

</div>
 
<div>
 
<p align="justify"> Celso Vinícius </p>
<a href="https://web.telegram.org/k/">
<img align="center" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"/> 

</div>
