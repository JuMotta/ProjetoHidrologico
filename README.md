# ProjetoHidrologico
### Projeto Hidrológico

O projeto hidrológico consistirá na realização e apresentação de cálculos hidrológicos para o projeto de uma central hidrelétrica. Cada item deverá ser respondido neste documento do repositório, usando a ferramenta de edição.


  - Com os dados de vazão usados no projeto do aproveitamento, os grupos deverão identificar e organizar os dados em médias semanais (Se a disposição dos dados for diária) ou anuais (Se a disposição dos dados for mensal);
  
  - Cada grupo deverá realizar uma caracterização estatística destes dados. Para a caracterização dos dados, o grupo deverá utilizar de programação, onde a linguagem de programação é de livre escolha do grupo. **O algoritmo programado deverá ser enviado ao repositório via *upload*. Não será permitida a utilização de planilhas excel ou de programas já feitos**. Os seguintes itens deverão ser respondidos neste documento:
  
       - Fluviograma dos dados, dispostos em valores anuais e decenais;
       
       ![Fluviograma anual](Fluviograma_anual.jpg)
       
       ![Fluviograma decenal](Fluviograma_decenal.jpg)
       
       - Curva de duração de vazões;
       
       ![Curva de duração de vazões](Curva_duracao_vazoes.jpg) 
       
       - Curva de duração de potência para uma queda (Determinada no projeto do aproveitamento) e rendimento de **85%**;
       ![Curva de duração de potência](Curva_duracao_potencia.jpg)
       
       - Diagrama de Rippl;   
       ![Diagrama de Rippl](Diagrama_rippl.jpg)

       - Determinação do período crítico;   
       
       A partir da Figura 6, pode-se determinar o período crítico, que é aquele que resulta na maior capacidade do reservatório. Considerando um coeficiente de regulariação de vazão igual a 1, ou seja, tomando a vazão necessária como a vazão média dos dados disponibilizados, temos que o período crítico é aproximadamente entre maio e dezembro.
       
       ![Médias semanais das vazões](Medias_semanais_vazao.jpg)
        
       - Determinação de períodos seco e úmido;
      
      O período seco corresponde aos meses do ano hidrológico em que ocorre o período crítico, ou seja, no caso analisado corresponde ao meses entre maio e dezembro.
       Já o período úmido são os meses restantes, no caso analisado, os meses de janeiro, fevereiro, março e abril.
        
       - Determinação de valores extremos;
       
       Como os dados do ano hidrológico e do ano civil são muito próximos para o nosso caso, pode-se admitir que são iguais. Com isso, a partir da Figura 6, é possível determinar os valores de vazão máxima e vazão mínima, os quais correspondem a 900 m³/s e 260 m³/s, respectivamente.
        
       - Estimativa da vazão firme e da vazão de projeto para dimensionamento de uma central hidrelétrica;
       
       A vazão firme é definida como a mínima vazão com que se pode contar e que possui uma frequência de ocorrência de, no mínimo, 95%. Com isso, a partir da Figura 3, definiu-se a Vazão Firme do projeto como sendo de 210 m³/s. E como a vazão de projeto deve ser menor que a vazão firme, definiu-se a Vazão de projeto como sendo 200 m³/s.
        
      
       - Cálculo da vazão regularizada: O grupo deverá fazer um cálculo da vazão regularizada baseado nos dados fornecidos de vazão. O método a ser usado é o método de Conti-Varlet. A formulação deste método está disponível no livro-texto do curso (Souza, Z., Santos, A. H. M e Bortoni, E. C.  **Centrais Hidrelétricas: Implantação e Comissionamento**, 2a. Edição, Editora Interciência.). Para este cálculo o grupo deverá:
        
       - Usar o programa disponibilizado pelo livro-texto do curso ou implementar o método em uma linguagem de programação da escolha do grupo. Caso o grupo escolha a segunda alternativa, **o algoritmo programado deverá ser enviado ao repositório via *upload***;
       
       - Análisar o resultado obtido de vazão regularizada e comparar este resultado com as vazões firme e de projeto calculados anteriormente;
       
       Para a realização do cálculo da vazão regularizada, foi utilizado o programa  Centrais Hidrelétricas, disponível em https://www.editorainterciencia.com.br/index.asp?pg=downloads.asp&token= que se encontra no livro Centrais Hidrelétricas: Implantação e Comissionamento, de Souza, Z. Santos A. H. M e Bortoni, E. C. Foi utilizado a função/programa Conti, que tem como entradas os dados de vazão obtidos para o estudo de caso, o volume útil de regularização, percentual do volume inicial e final do reservatório, número de discretizações e número de iterações. Para o caso deste estudo foi estabelecido o mesmo critério utilizado no livro texto, onde se determinou 78 como o número de discretizações e 3 o número de iterações. 
       
       Com a simulação do programa, foram obtidos um novo arquivo de saída com as vazões e os dados de vazão, e volume para regularização total, sendo esses equivalentes à 704,13 m³/s e 19820144 m³respectivamente. 
       
       O valor da vazão regularizada obtido nessa simulação é consideravelmente maior do que os valores de vazão firme e de projeto estimados previamente. Essa diferença tem impacto direto no tamanho do reservatório a ser construído de modo a regularizar a vazão. Sendo a vazão necessária para tocar o empreendimento tão maior do que a vazão que se pode contar com regularidade, o reservatório deverá ser grande de modo a acumular água nos períodos úmidos e permitir o aumento da vazão no período seco.
        
  - Projetos que não tiverem todos estes itens respondidos ou que estiverem incompletos **não serão avaliados!**
Este projeto deverá ser feito neste arquivo até o dia **23/09/2018**. Pedidos de adiamento só serão concedidos em casos excepcionais, a serem decididos pelo professor.

### Projeto do Conduto

O projeto do conduto consistirá na realização e apresentação de cálculos de condutos e canais para a central hidrelétrica. 


  - Projeto do canal para a futura usina hidrelétrica utilizando as fórmulas de Chezy, determinando de acordo com os dados de vazão de cada grupo:
  
  Podemos estimar o valor do coeficiente de Chézy através da fórmula de Manning como sendo:
  
  ![Equação 1](eq1.gif)
  
   Tomando o material das paredes do conduto como sendo concreto com acabamento ordinário, o valor tabelado do coeficiente de Gauckler-Manning para a rugosidade do conduto é de 0,014.
  Se considerarmos o escoamento como forçado, ou seja, preenchendo toda a área interna da tubulação, temos que:
  
  ![Equação 2](eq2.gif)
  
   Assim, podemos reescrever o coeficiente de Chézy para o escoamento em questão como:
  
  ![Equação 3](eq3.gif)
  
   Substituindo na fórmula de Chézy em função da vazão:
  
  ![Equação 4](eq4.gif)
  
   Podemos assumir o valor da declividade do conduto através de uma aproximação razoável, sendo observados outros projetos de parâmetros semelhantes. Para o nosso caso, foi estimado um ângulo de 25° entre a horizontal e o fim do canal, o que nos leva a um valor para o coeficiente de inclinação de:
  
  ![Equação 5](eq5.gif)
  
   -A melhor forma geométrica de seção para o canal em questão;
       
   - O diâmetro hidráulico da seção;
     Substituindo os valores obtidos na fórmula de Chézy, e considerando a vazão média estimada no projeto do aproveitamento (490,67 m³/s), temos:
       
       ![Equação 6](eq6.gif)
       
       Resolvendo esta equação, obtemos r = 1,84 m.
       
       Logo, o diâmetro hidráulico é de 3,68 m.
       
       
   - Velocidade da água no canal;
       
     Substituindo o valor do raio na equação da continuidade, temos:
       
        ![Equação 7](eq7.gif)

        ![Equação 8](eq8.gif)

        ![Equação 9](eq9.gif)
       
       
     - Vazão de água no canal;
     
       Para fins de cálculos, foi assumido que a vazão no canal é a mesma vazão média medida no rio, no caso 490,67 m³/s.
       
      
  - Baseado nos valores de queda dispostos no projeto do aproveitamento, o grupo deverá inserir no desenho esquemático deste projeto os seguintes itens:
        
       - Valores de cota de altura;
       - Alturas de queda;
       - Linhas piezométrica e de energia;
       
       Com o valor obtido para o diâmetro hidráulico, estabelecemos as linhas piezométrica e de energia, como pode ser visto na imagem abaixo onde há uma relação das linhas com o desenho técnico e as respectivas cotas.
       
       ![Desenho](desenho_esquematico.png)
       
        
  - Determinação do semiperíodo da onda de pressão para dimensionamento do conduto fechado. Cada grupo poderá fazer as considerações que achar necessárias;
  
     Com o ângulo estimado de 25° entre a horizontal e o fim do canal, pode ser calculado o comprimento do tubo:
     
     ![Equação 9.1](eq9.1.gif)
  
     Para o cálculo do tempo de parada do escoamento (tv), utilizou-se a fórmula empírica de Mendiluce:
     
     ![Equação 10](eq10.gif)
     
     ![Equação 11](eq11.gif)
     
     ![Equação 12](eq12.gif)
     
     
       Sendo, 
       
      L = comprimento do conduto;
      
      u = velocidade do escoamento;
      
      H = altura de queda;
      
      K = um coeficiente, tal que:
      
	   K = 2, quando L < 500m 
		  
	   K = 1,5, quando 500m < L < 1500m
		  
	   K = 1, quando L > 1500m

      Calculando a Celeridade (Vs), obteve-se:
      
     ![Equação 13](eq13.gif)
     
     ![Equação 14](eq14.gif)
     
     ![Equação 15](eq15.gif)
     
       Sendo,
       
     Km = 5, para o concreto;
     
     D = diâmetro do conduto;
     
     e = espessura do conduto. Adotou-se a espessura do conduto como sendo de 1cm.
     
     Para o cálculo do semiperíodo (T), obteve-se:
     
     ![Equação 16](eq16.gif)
     
     ![Equação 17](eq17.gif)
     
     ![Equação 18](eq18.gif)
     
     Como tv>T, essa manobra é classificada como manobra lenta.
  
  - Determinação de valores de golpe de aríete positivo máximo;
  
    O valor do golpe de aríete positivo máximo (hs+) obtido foi de:
    
     ![Equação 19](eq19.gif)
     
     ![Equação 20](eq20.gif)
     
     ![Equação 21](eq21.gif)
  
  - Determinação de valores do golpe de aríete aceitável;
  
    Como nossa central é de baixa queda, calculou-se o valor de Kb:
    
     ![Equação 22](eq22.gif)
     
     ![Equação 23](eq23.gif)
     
     ![Equação 24](eq24.gif)
     
     Com isso, o valor do golpe de aríete aceitável (hs) será:
     
     ![Equação 25](eq25.gif)
     
     ![Equação 26](eq26.gif)
     
     ![Equação 27](eq27.gif)
    
    
  - Projetos que não tiverem todos estes itens respondidos ou que estiverem incompletos **não serão avaliados!**
Este projeto deverá ser feito neste arquivo até o dia **07/10/2018**. Pedidos de adiamento só serão concedidos em casos excepcionais, a serem decididos pelo professor.
