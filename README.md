# diario_bordo_sist_op2

Parte A: Entendendo a Barreira do Sistema (Chamadas de Sistema)

A) Para explicar esta pergunta, é relembrar que relembrar os estudos realizados nas aulas passadas, systen calls e traps, que mudam o status das aplicações
![System Calls](imagens/diagrama_02.jpg)



B)A representação indica a mudança de estado estuda via system call e traps, estudamos na aulas que as aplicações mudam seus status transitando para o modo usuário, em primeiro plano e modo kernel, segundo plano.
![Mudança de Eestados](<imagens/Diagrama sem nome.drawio.png>)




Parte B: Diagnosticando o Escalonador

A)Para entender o congelamento, recomemos as apresentações feitas nas aulas sobre o sistemas operacionais e as aulas da data de 01/10/2026. As aplicações são selecionadas conforme a ordem de chegeda, sendo que, os usuários fazem requsições "rápidas" e constantes. O relatórios entra na fala e com isso, fica esperando a sua vez
![Fila](imagens/fila.gif)



B)Vamos imaginar que na fila que criamos na questão acima funcione com uma regra a mais, além da ordem de chegada, esta nova regra é: uma vez que o processo começar o seu "atendimento" só retirado ou interrompido com a finalização do processo.
[![Assistir ao vídeo](https://img.youtube.com/vi/waN3YZgaunI/hqdefault.jpg)](https://youtu.be/waN3YZgaunI?si=ufbthX1osCHzjQy1)

Parte C

A)Eu escolheria o Round-Robin. O video abaixo, a principal vantagem é combater a situação de starvation. evitando os congelamentos
[![Assistir ao vídeo](https://img.youtube.com/vi/YoToRdqa6us/hqdefault.jpg)](https://youtu.be/YoToRdqa6us?si=ijldClY1xHc8Ae1Z)

B)Para explicar o stravation, podemos fazer uma analogia com o jogo pacman. Imagine que o processo é o pacman e as bolinhas são o cpu, neste caso, não existe uma proxima fase com mais recursos e um novo pacman irá entrar no jogo. Em determinado momento, os recursos irão, um dos pacman não consiguirá obter recursos e por consequência, ficará congelado. Para resolve isso, podemos utlizar os mecanismo de escolamento.
![Pacman](imagens/pacman-gaming.gif)
