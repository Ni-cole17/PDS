# EPILEPSIAE

## Processamento Digital de Sinais

#### Esse projeto foi desenvolvido ao longo da cadeira de processamento digital de sinais, onde aprendemos primeiro conceitos teóricos sobre a manipulação de sinais, demonstrado nas listas de exercícios, para que enfim pudessemos juntar todos os conhecimento e aplicar no projeto final da disciplina. O projeto final consistiu em fazer o pré-processamento de uma base de dados contendo sinais de EEG (Eletroencefalograma) antes e depois de pacientes receberem um estímulo acústico binaural. Essa base de dados tem um total de 27 arquivos de sinais e tem uma frequência de amostragem de 500Hz. Ela foi disponibilizada pelo grupo de computação biomédica, liderada pelo professor Wellington Pinheiro dos Santos.

#### Grupo: Nicole Charron, Pedro Gurgel, Breno José dos Santos, Caio Vinícius e Eduarda Regina
 
### Dificuldade no desenvolvimento do projeto:
 - Escolha de um filtro ideal para a filtragem dos dados de acordo com as bandas do EEG
 - Janelamento dos dados
 - Capacidade Limitada das nossas máquinas 

### Soluções:
#### Escolha de um filtro ideal:
##### Para a escolha do filtro, foram feitas revisões na literatura para buscar a aplicação de filtros em problemas semelhantes. Achamos uma utilização de filtros FIR e IIR, e pela familiaridade do grupo com os filtros IIR e pelo seu baixo custo computacional em relação aos filtros FIR, decidimos por começar esse trabalho explorando os filtros IIR. No entanto, como trabalhos futuros e com a disponibilidade de máquinas mais potentes, pretendemos testar outros filtros e outras configurações com o objetivo de verificar melhoras no pré-processamento dos dados.
#### Janelamento dos dados:
##### Durante o desenvolvimento do trabalho utilizamos em grande parte dele um janelamento de 300ms com sobreposição de 100ms, isto por que o EEG capta sinais gerados por um somatório de potenciais de ação de um determinado grupo de células. Sabendo que o potencial de ação de uma célula nervosa dura em torno de 5ms, procuramos utilizar um janelamento próximo em magnitude do potencial de ação das células nervosas. No entanto, ao realizar a extração de atributos de cada um dos sinais janelados, foi observado que a base de dados resultante precisava de um armazenamento muito superior ao suportado por nossas máquinas. Em vista disso, optamos por selecionar um janelamento maior dos dados, agora com 1s com sobreposição de 250ms, obtendo uma base de dados menor e que poderia ser trabalhada.
#### Capacidade Limitada das nossas máquinas:
##### Em alguns casos, buscamos ter acesso aos computadores disponibilizados pelo nosso departamento de Engenharia Biomédica, assim, alguns processos que precisavam de um maior custo computacional foi desenvolvido no laboratório de informática.
