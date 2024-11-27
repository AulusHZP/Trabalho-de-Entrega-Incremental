# Previsão de Falhas em Sistemas Complexos 

* Aulus Arcanjo Alves Batista
* Leonardo de Freitas Viana
* Henrique Leite Najar
* Nome do orientador acadêmico e de conteúdo: Lesandro Ponciano dos Santos


## Introdução

1. A área da Engenharia de Software tratada neste trabalho é: Previsão de Falhas em Sistemas Complexos, utilizando técnicas de Deep Learning para melhorar a capacidade de antecipação de falhas e otimizar a confiabilidade dos sistemas.

2. O problema que este trabalho busca resolver nessa área é: Como prever falhas de forma eficaz em sistemas complexos que apresentam alta variabilidade e interdependência de componentes. Métodos tradicionais muitas vezes falham em capturar a complexidade e os sinais sutis que indicam falhas iminentes, resultando em perdas financeiras e em disponibilidade do sistema. Estudos como "Deep-Learning-Enabled Predictive Maintenance in Industrial Internet of Things: Methods, Applications, and Challenges" (disponível em [https://ieeexplore.ieee.org/document/9851995]), pelos autores Wang et al. (2023) evidenciam que métodos tradicionais apresentam limitações na captura de padrões complexos em sistemas industriais, destacando a superioridade do Deep Learning em relação à previsão de falhas.

3. Resolver este problema é relevante porque: A previsão eficiente de falhas pode evitar paradas inesperadas, reduzir custos operacionais e aumentar a confiabilidade e a disponibilidade de sistemas complexos. Embora outras técnicas como Gradient Boosting Machines (GBM) e Redes Bayesianas também capturem padrões não lineares e interdependências, as técnicas baseadas em Deep Learning oferecem vantagens adicionais, como a capacidade de capturar padrões hierárquicos em situações de alta dimensionalidade e a habilidade de extrair características automaticamente dos dados brutos, reduzindo a necessidade de pré-processamento intensivo e engenharia manual de atributos. Isso as torna particularmente adequadas para problemas de previsão de falhas em sistemas com alta complexidade e interdependências. Estas vantagens são confirmadas por revisões como "Deep Learning for Predictive Maintenance: A Survey", que destacam a superioridade das técnicas de Deep Learning para a previsão de falhas em sistemas complexos.

4. Objetivo Geral deste trabalho é avaliar modelos de aprendizado profundo (deep learning) para melhorar a previsão de falhas em sistemas complexos, reduzindo o tempo de inatividade e aumentando a eficiência operacional

5. Os *três* objetivos específicos deste trabalho são: (1)Coletar e organizar dados relevantes sobre falhas em sistemas, garantindo sua adequação para análise. Aqui será feito o trabalho de preparação dos dados, seja obtendo conjuntos públicos, simulados ou processando os existentes.(2)Implementar e testar modelos básicos de aprendizado profundo para prever falhas, explorando sua aplicação prática. Focar na construção inicial de modelos acessíveis e funcionais, como redes neurais simples, alinhando-se ao que é viável no projeto.(3)Avaliar o desempenho dos modelos utilizando métricas como precisão, simplicidade e eficiência, para determinar sua viabilidade. Garantir que a análise se baseie em resultados claros e objetivos, utilizando ferramentas acessíveis.

## Fundamentação Teórica

1. Predição: A predição refere-se à capacidade de prever eventos futuros com base em dados históricos e padrões observáveis. Este conceito é explorado no contexto da manutenção preditiva no artigo "Deep-Learning-Enabled Predictive Maintenance in Industrial Internet of Things: Methods, Applications, and Challenges" por Wang et al. (2023), que detalha como técnicas de aprendizado profundo podem ser aplicadas para prever falhas e mitigar paradas não planejadas de máquinas industriais. Isso permite a manutenção proativa e a prevenção de falhas catastróficas, maximizando a eficiência operacional do sistema​

2. Sistemas Complexos: Sistemas complexos são caracterizados por múltiplos componentes interdependentes, cuja dinâmica resulta em comportamentos não lineares que não podem ser previstos pela simples soma dos comportamentos individuais. No contexto da manutenção preditiva em sistemas de produção multiestágio, como descrito no artigo "Predictive Maintenance Decision Making Based on Reinforcement Learning in Multistage Production Systems" por Feng e Li (2022), a complexidade é enfatizada através da necessidade de otimizar decisões de manutenção considerando as interdependências entre as máquinas, que podem causar paradas inesperadas e afetar a eficiência do sistema de produção​

3. Confiabilidade: Confiabilidade refere-se à capacidade de um sistema ou componente de desempenhar suas funções esperadas sem falhas durante um período específico. No contexto de previsão de falhas, a confiabilidade pode ser melhorada por meio de técnicas de verificação formal que garantem a precisão dos modelos preditivos. Isso é abordado no artigo "Formal Verification of a Hybrid Machine Learning-Based Fault Prediction Model in Internet of Things Applications" por Souri et al. (2020), onde o objetivo é formalmente verificar modelos de previsão para garantir que eles funcionem conforme esperado e minimizar a ocorrência de falhas não detectadas

4. Disponibilidade: Disponibilidade refere-se à proporção de tempo em que um sistema está operando corretamente e disponível para uso. No artigo "Deep Learning-Based Method for the Robust and Efficient Fault Diagnosis in the Electric Power System" por Yoon e Yoon (2022), a disponibilidade é destacada no contexto de sistemas de energia elétrica, onde a rápida detecção e classificação de falhas é essencial para manter a operação do sistema e evitar apagões em larga escala. O uso de redes neurais convolucionais permite identificar falhas e garantir que o sistema esteja disponível o maior tempo possível, minimizando o tempo de inatividade devido a falhas
  

## Trabalhos Relacionados

1. O trabalho mais relacionado é "Deep Learning-Based Method for the Robust and Efficient Fault Diagnosis in the Electric Power System" (https://doi.org/10.1109/ACCESS.2022.3170685), publicado no ano de 2022, porque ele apresenta uma abordagem baseada em aprendizado profundo, utilizando redes neurais convolucionais para detectar e diagnosticar falhas em sistemas de energia elétrica. Este trabalho é relevante para o nosso projeto, pois aborda técnicas de Deep Learning que permitem identificar falhas de maneira eficiente em sistemas complexos, alinhando-se ao nosso objetivo de prever falhas com precisão.<br/>
2. O segundo trabalho mais relacionado é "Formal Verification of a Hybrid Machine Learning-Based Fault Prediction Model in Internet of Things Applications" (https://doi.org/10.1109/ACCESS.2020.2967629), publicado no ano de 2020, porque ele propõe a verificação formal de um modelo híbrido de previsão de falhas que combina Perceptron Multicamada (MLP) e Particle Swarm Optimization (PSO). A abordagem de verificação formal fornece uma base sólida para garantir a precisão dos modelos preditivos, o que é essencial para nosso objetivo de melhorar a confiança na previsão de falhas em sistemas complexos.<br/>
3. O terceiro trabalho mais relacionado é "Predictive Maintenance Decision Making Based on Reinforcement Learning in Multistage Production Systems" (https://doi.org/10.1109/ACCESS.2022.3151170), publicado no ano de 2022, porque explora o uso de aprendizado por reforço para otimizar decisões de manutenção preditiva em sistemas de produção multistágio. Apesar de não utilizarmos aprendizado por reforço em nosso trabalho, a aplicação de técnicas de otimização para melhorar as políticas de manutenção é extremamente relevante, proporcionando insights para o desenvolvimento de estratégias eficientes de previsão de falhas.<br/>
4. O quarto trabalho mais relacionado é "Deep-Learning-Enabled Predictive Maintenance in Industrial Internet of Things: Methods, Applications, and Challenges" (https://doi.org/10.1109/JSYST.2022.3193200), publicado em 2023, porque oferece uma visão abrangente sobre as técnicas de Deep Learning aplicadas à manutenção preditiva. Este trabalho descreve como redes neurais profundas, como CNNs e LSTMs, podem ser usadas para prever falhas, o que está diretamente alinhado ao nosso projeto, proporcionando uma compreensão prática dos desafios e aplicações do Deep Learning para previsão de falhas.<br/><br/>

## Materiais e Métodos

1- O tipo de pesquisa adotado neste trabalho é exploratória e experimental, porque buscamos testar ferramentas e conceitos de inteligência artificial para prever falhas em máquinas, usando recursos acessíveis e explorando soluções práticas para manutenção preditiva.

2- Os materiais utilizados neste trabalho são: Computadores: Um notebook ou desktop básico, com acesso à internet.
Softwares: Python e bibliotecas gratuitas como NumPy, Pandas e Scikit-learn. Google Colab, uma ferramenta online gratuita para rodar códigos Python, caso o computador tenha limitações. 
Dados: Conjuntos de dados públicos ou exemplos simulados, criados para representar falhas de máquinas.

3- Os métodos empregados neste trabalho são: Método de Modelagem: Criação de modelos simples de aprendizado de máquina, como árvores de decisão ou regressão, para prever falhas em sistemas.
Método de Simulação de Dados: Geração de dados fictícios para simular falhas, caso dados reais não estejam disponíveis.
Método de Testes: Divisão dos dados em treinamento (para ensinar o modelo) e teste (para verificar sua precisão).

4- As métricas de avaliação são: Acurácia: Para medir quantas vezes o modelo acerta. Simplicidade e Eficiência: Avaliar se o modelo pode ser usado facilmente com os recursos disponíveis.

5- As etapas de execução do trabalho são:
Etapa 1: Pesquisar sobre manutenção preditiva e inteligência artificial.
Etapa 2: Obter ou criar dados representando falhas de máquinas.
Etapa 3: Implementar os modelos utilizando Python e bibliotecas disponíveis.
Etapa 4: Testar os modelos para verificar a precisão e desempenho.
Etapa 5: Analisar os resultados e registrar as conclusões para avaliação.

