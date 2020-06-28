----------------------------------------------------
------------    PROPOSAL DOCUMENT       ------------
----------------------------------------------------

Capítulo 1: Introdução
    Parágrafo 1: falo sobre pesquisas em USV e por que é interessante automatizar uma embarcação
    
    Parágrafo 2: falo sobre COLREGS e por que é importante implementar evasão de colisão em um USV

    Parágrafo 3: falo que a aplicação da COLREGS está condicionada a cada caso (ilustrada pela imagem 1.1). Falo que é possível identificar se há risco de colisão em um encontro através do CPA

    Parágrafo 4: apresentação do documento

    IMAGEM 1.1

Capítulo 2: Fundamentação Teórica
    Parágrafo 1: apresentação do capítulo    

    Capítulo 2.0: Metodologia de Pesquisa
        

    Capítulo 2.1: USV
        Parágrafo 1: explico as características de um USV e quais são seus componentes

        Parágrafo 2: falo a respeito do sistema GNC (ilustrado pela imagem 2.1)

        Enumerador: falo a respeito dos subsistemas de Guidance, Navigation e Control separadamente.

        IMAGEM 2.1

        Parágrafo 3: falo a respeito dos planejadores global e local presente no subsistema de Guidance
    
    Capítulo 2.2: COLREGS
        Parágrafo 1: falo o que é a COLREGS, quem a detém e que todas as intensões de movimentação do USV devem ser claras e previsíveis.

        IMAGEM 2.2

        Enumerador: falo a respeito de cada encontro ilustrado na IMAGEM 2.2

    Capítulo 2.3: Collision Avoidance
        Parágrafo 1: falo quem, no sistema GNC, é responsável pela tarefa de evasão de colisão. Apresento a definição de evasão de colisão.

        Enumerador: apresento cada etapa do processo de prevenção de colisão

        Parágrafo 2: falo do floxo de informação que acontece no processo de prevenção de colisão (ilustrada pela imagem 2.3) e qual o papel de cada módulo ilustrado

    Capítulo 2.4: Ponto de Maior Aproximação
        Parágrafo 1: falo a respeito Collision Risk Index (CRI), Closest Point of Approach (CPA), Time to CPA (TCPA) e Distance to CPA (DCPA).

        Parágrafo 2: apresento a equação do TCPA e DCPA

        Parágrafo 3: introduzo a apresentação de um exemplo visual do calculo do TCPA, definindo posições e velocidades das embarcações do exemplo (ilustrada pela imagem 2.4) e explico as operações (pa - pb) e (va - vb) (ilustradas pelas imagens 2.5 e 2.6)

        IMAGEM 2.4  
        IMAGEM 2.5
        IMAGEM 2.6  

        Parágrafo 4: explico o porquê utilizamos o valor absoluto do DCPA

        Parágrafo 5: falo a respeito do cálculo do DCPA (ilustrado pela imagem 2.7)

        IMAGEM 2.7

        Parágrafo 6: explico um caso em que, dado às velocidades das embarcações, não haverá colisão (ilustrado pela imagem 2.8)

        IMAGEM 2.8


Capítulo 3: Framework de desenvolvimento
    Parágrafo 1: apresentação do capítulo

    Capítulo 3.1: ROS
        Parágrafo 1: falo o que é o ROS, quem o mantém e suas características 

        Enumerador: apresento conceitos importantes sobre ROS
    
    Capítulo 3.2: Sistema base
        Parágrafo 1: falo o que é o sistema base, para o que foi desenvolvido, quais suas limitações e do que é composto

        Parágrafo 2: aprofundo explicação sobre GNC abordando planejador global e local

        Parágrafo 3: apresento que os planejadores possuem mapas de custo para determinar suas rotas. Também falo que o sistema base utiliza de Artificial Terrain Cost (ATC) para determinar rotas que atendem às exigências da COLREGS

        Parágrafo 4: explicação da imagem 3.1

        IMAGEM 3.1


Capítulo 4: Desenvolvimento
    Parágrafo 1: Explico o que foi implementado e quais informações foram utilizadas para realizar a implementação. Apresento fluxogramas da rotina onde o CPA foi inserido antes e depois da implementação (imagens 4.1 e 4.2)

    IMAGEM 4.1

    IMAGEM 4.2

Capítulo 5: Experimentos Empíricos
    Parágrafo 1: apresentação do capítulo, definição de quais casos de testes serão realizados e quais informações serão apresentadas

    Parágrafo 2: informo qual ferramenta foi utilizada para realizar os testes, qual o tipo de embarcação utilizada (ilustrado pela imagem 5.2) e qual o local simulado (ilustrado pela imagem 5.1)

    Capítulo 5.1: Head On
        Parágrafo 1: explico o caso de teste, explico a trajetória realizada (ilustrada pela imagem 5.3), falo a menor distância registrada no teste, explico o gráfico que mostra o TCPA (imagem 5.4 a), explico o gráfico que mostra o DCPA (imagem 5.4 b), explico o tempo de computação (imagem 5.6)

        IMAGEM 5.3

        IMAGEM 5.4a

        IMAGEM 5.4b

        IMAGEM 5.5

    
    Capítulo 5.2: Overtake
        Parágrafo 1: explico o caso de teste, explico a trajetória realizada (ilustrada pela imagem 5.6), falo a menor distância registrada no teste, explico o gráfico que mostra o TCPA (imagem 5.7a), explico o gráfico que mostra o DCPA (imagem 5.7b), explico o tempo de computação (imagem 5.8)

        IMAGEM 5.6

        IMAGEM 5.7a

        IMAGEM 5.7b

        IMAGEM 5.8


    Capítulo 5.3: Crossing from Left
        Parágrafo 1: explico o caso de teste, explico a trajetória realizada (ilustrada pela imagem 5.9), falo a menor distância registrada no teste, explico o gráfico que mostra o TCPA (imagem 5.10a), explico o gráfico que mostra o DCPA (imagem 5.10b), explico o tempo de computação (imagem 5.11)

        IMAGEM 5.9

        IMAGEM 5.10a

        IMAGEM 5.10b

        IMAGEM 5.11


    Capítulo 5.4: Crossing from Right
        Parágrafo 1: explico o caso de teste, explico a trajetória realizada (ilustrada pela imagem 5.12), falo a menor distância registrada no teste, explico o gráfico que mostra o TCPA (imagem 5.13a), explico o gráfico que mostra o DCPA (imagem 5.13b), explico o tempo de computação (imagem 5.14)

        IMAGEM 5.12

        IMAGEM 5.13a

        IMAGEM 5.13b

        IMAGEM 5.14


    Capítulo 5.5: Crossing from Right
        Parágrafo 1: explico o caso de teste, explico a trajetória realizada (ilustrada pela imagem 5.12), falo a menor distância registrada no teste, explico o gráfico que mostra o TCPA (imagem 5.13a), explico o gráfico que mostra o DCPA (imagem 5.13b), explico o tempo de computação (imagem 5.14)

        IMAGEM 5.12

        IMAGEM 5.13a

        IMAGEM 5.13b

        IMAGEM 5.14


    Capítulo 5.5: Crossing from Right - Embarcação Parada
        Parágrafo 1: Apresentação do capítulo

        Capítulo 5.5.1: Sem CPA
            Parágrafo 1: explico o caso de teste, explico a trajetória realizada (ilustrada pela imagem 5.15), falo a menor distância registrada no teste, explico o tempo de computação (imagem 5.16)
    
            IMAGEM 5.15
    
            IMAGEM 5.16


    Capítulo 5.5: Crossing from Right
        Parágrafo 1: explico o caso de teste, explico a trajetória realizada (ilustrada pela imagem 5.17), falo a menor distância registrada no teste, explico o gráfico que mostra o TCPA (imagem 5.18a)e o DCPA (imagem 5.18b) em conjunto para evidenciar o momento em que os thresholds são atingidos e é detectado o risco de colisão erroneamente, explico o tempo de computação (imagem 5.19)

        IMAGEM 5.17

        IMAGEM 5.18a

        IMAGEM 5.18b

        IMAGEM 5.19
    
    5.6 Discussão
       - Discussão comparando os resultados do Darlan e o que tu conseguiste
       
