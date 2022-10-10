<h1 align="center">Sistema Operacional Minix</h1>

# Resumo

<p> O Minix é um sistema operacional gratuito desenvolvido por Andrew Tanenbaum para compensar a proibição da AT&T contra o estudo de SO baseado no código UNIX e prover uma ferramenta de ensino para seus alunos. Originalmente foi projetado para ser compatível com a versão 7 do UNIX e em seguida passou a ser desenvolvido baseado no padrão POSIX. O Minix foi escrito a partir do zero e mesmo sendo compatível com UNIX, não contém código AT&T possibilitando sua distribuição livremente. </p>

# Escalonamento/Política/Aplicabilidade

<h3> Escalonamento </h3>

<p> O Minix devido ao seu projeto de Micro-Kernel tem uma pequena quantidade de processos que são executados em modo de kernel, sendo assim com grande parte do sistema sendo executados em modo de usuário. Para o Minix, o escalonador de processos de usuário tem uma importância extra já que terá que lidar com uma quantidade bem maior do que o escalonador de kernel. Desse modo é vital que o Minix tenho um instalador justo e responsível em espaço de usuário. </p>

<h3> Política </h3>

<p> Os algoritmos de escalonamento servem para implementar politicas que controlam a execução de múltiplos processos uma vez que cada CPU pode ser acessa por apenas um processo por vez, em geral esses algoritmos prezam por:

- Justiça: fazer com que cada processo tenha um tempo justo de CPU;
- Equilíbrio: tentando manter todas as partes do sistema ocupadas.  
</p>

# Gerenciamento de Memória

<p> A gestão de memória do MINIX 3 faz uso de um gerenciamento simples, não utilizando de paginação ou swap, sendo também mesclado com a gestão de processos. Essas são algumas das características que o difere de outros sistemas operacionais.

Contando com um sistema de lacunas, a medida que decorrerem as system call's fork ou exec, a lista percorrerá até encontrar a primeira lacuna que tenha espaço suficiente para receber, denominada como first-fit. </p>

# Gerência de Arquivos

<p> Os arquivos, no geral, são uma forma de armazenar informações em disco. Ou seja, quando um processo está sendo executado, ele armazena informações e, quando esse mesmo processo é finalizado, toda a informação acaba sendo perdida. Porém, se as informações forem gravadas em formato de arquivo, elas poderão ser lidas e utilizadas por outros processos novamente.

Como em qualquer sistema de arquivos, o sistema de arquivos do MINIX deve alocar e desalocar o espaço para os arquivos, monitorar blocos de disco e liberar espaço, oferecer alguma maneira de proteger arquivos contra uso não-autorizado. </p>

# Multiprogramação/Chaveamento de Processos/Swap

# Denvolvedores 
<p>

- Lívia Gonçalves
- Júlia Melo
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
 
<p align="justify"> Júlia Melo </p>
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
