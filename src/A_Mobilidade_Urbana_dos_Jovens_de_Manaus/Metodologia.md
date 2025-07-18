# Metodologia

Este relatório foi elaborado a partir de uma análise rigorosa de dados provenientes de uma pesquisa sobre a mobilidade urbana dos jovens em Manaus. A metodologia adotada visou garantir a fidelidade aos dados e a construção de uma argumentação sólida que conteste a premissa de que os transportes por aplicativo são a solução definitiva para a mobilidade urbana. As etapas seguidas foram organizadas em três fases principais: Planejamento, Condução e Análise.

## 1. Planejamento

Nesta fase, foram definidos os objetivos da pesquisa e a estrutura para a coleta de dados. O principal instrumento de coleta foi um questionário, cuidadosamente elaborado para capturar informações relevantes sobre os hábitos de mobilidade dos jovens em Manaus. O questionário incluiu perguntas sobre:

*   **Dados Demográficos:** Idade, zona de residência e ocupação dos participantes.
*   **Uso de Aplicativos de Transporte:** Frequência de uso de serviços como Uber e 99, gasto mensal e comportamento em relação à comparação de preços.
*   **Percepção de Custo e Tempo:** Avaliação da importância do preço e do tempo na escolha do meio de transporte.
*   **Reação à Tarifa Dinâmica:** Comportamento dos usuários diante das variações de preço dos aplicativos.
*   **Uso de Motos por Aplicativo:** Frequência e percepção de segurança em relação a esta modalidade.
*   **Confiabilidade dos Serviços:** Número de cancelamentos de viagens nos últimos três meses.
*   **Segurança:** Uso de ferramentas de segurança oferecidas pelos aplicativos.
*   **Transporte Público:** Nível de satisfação com o transporte público (ônibus) e os principais problemas percebidos.

## 2. Condução

A fase de condução envolveu a aplicação do questionário aos participantes da pesquisa. O questionário foi enviado a 34 jovens de Manaus, garantindo uma amostra diversificada em termos de idade (entre 18 e 28 anos), zona de residência e ocupação. Os dados coletados foram compilados em um arquivo CSV (`mobilidade_urbana.csv`), que serviu como base para as análises subsequentes. A coleta de dados foi realizada de forma a garantir a privacidade e o anonimato dos participantes, focando na obtenção de informações precisas e representativas sobre seus hábitos e percepções de mobilidade.

## 3. Análise

A fase de análise foi dividida em três etapas principais: processamento e análise estatística dos dados, geração de gráficos e visualizações, e interpretação e argumentação.

### 3.1. Processamento e Análise Estatística dos Dados

Para a manipulação e análise dos dados do arquivo CSV, foi utilizada a biblioteca `pandas` do Python, uma ferramenta robusta para análise de dados. As etapas de processamento incluíram:

*   **Carregamento dos Dados:** O arquivo `mobilidade_urbana.csv` foi carregado em um DataFrame do pandas, permitindo a fácil manipulação e acesso às variáveis.
*   **Tratamento de Dados Categóricos:** Variáveis categóricas, como 'Viagens/semana (Uber/99)', 'Gasto Mensal (Apps)', 'Viagens Moto (de 10)', e 'Cancelamentos (3 meses)', foram mapeadas para valores numéricos representativos para permitir cálculos e correlações. Por exemplo, categorias de gasto como 'Até R$ 50' foram convertidas para um valor médio representativo (e.g., 25), e faixas de viagens como '1 a 2' foram convertidas para o ponto médio (e.g., 1.5).
*   **Conversão de Tipos de Dados:** Colunas como 'Satisfação Ônibus (1-5)', 'Peso Preço (1-5)' e 'Peso Tempo (1-5)' foram convertidas para o tipo numérico, com tratamento de erros para valores não numéricos, garantindo a integridade dos cálculos.

As análises estatísticas realizadas incluíram:

*   **Estatísticas Descritivas:** Cálculo de médias (e.g., satisfação com o ônibus, peso do preço e tempo, cancelamentos, viagens de moto) para resumir as características principais dos dados.
*   **Análise de Correlação:** Utilização do coeficiente de correlação de Pearson para verificar a relação entre o gasto mensal com aplicativos e a frequência de uso, indicando a força e a direção dessa relação.
*   **Análise de Frequência e Distribuição:** Contagem da frequência de respostas para variáveis categóricas (e.g., 'Reação à Tarifa Dinâmica', 'Compara Preços?', 'Uso Ferramenta Segurança'), apresentadas em termos percentuais para facilitar a compreensão da distribuição das respostas.

### 3.2. Geração de Gráficos e Visualizações

Para complementar a análise estatística e proporcionar uma compreensão visual mais clara dos dados, foram gerados diversos gráficos utilizando as bibliotecas `matplotlib.pyplot` e `seaborn` do Python. Cada gráfico foi projetado para ilustrar um aspecto específico da análise, permitindo a identificação rápida de padrões e tendências. Os gráficos gerados incluem:

*   Gráfico de barras para a satisfação com o transporte público.
*   Gráfico de dispersão para a correlação entre gasto mensal e viagens por semana.
*   Gráficos de pizza para a reação à tarifa dinâmica e a frequência de comparação de preços.
*   Gráfico de barras para a importância do preço versus tempo.
*   Gráficos de barras para a média de cancelamentos e a média de viagens de moto.
*   Gráfico de pizza para o uso de ferramentas de segurança.

### 3.3. Interpretação e Argumentação

Os resultados das análises estatísticas e as visualizações foram interpretados criticamente. A interpretação focou em:

*   **Contextualização dos Dados:** Análise dos números dentro do contexto socioeconômico e urbano de Manaus, considerando as implicações para a população jovem.
*   **Construção de Argumentos:** Desenvolvimento de argumentos baseados em evidências que demonstram as limitações dos aplicativos de transporte como solução abrangente, focando em aspectos como custo, confiabilidade, segurança e impacto no transporte público.

Finalmente, todas as informações coletadas, processadas e interpretadas foram sintetizadas e organizadas em um relatório no formato MD Book.

