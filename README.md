MVP Análise de Dados e Boas Práticas - Wine Quality Dataset

📊 Sobre o Projeto
Este projeto realiza uma análise exploratória completa e pré-processamento de dados no dataset Wine Quality do UCI Machine Learning Repository. O objetivo é compreender as características físico-químicas que influenciam a qualidade dos vinhos portugueses (tintos e brancos) e preparar os dados para futura modelagem de machine learning.
🎯 Objetivos

Realizar análise exploratória detalhada dos dados
Identificar padrões e correlações entre variáveis químicas e qualidade
Comparar características entre vinhos tintos e brancos
Aplicar técnicas de pré-processamento e limpeza de dados
Validar hipóteses sobre fatores que influenciam a qualidade do vinho

📁 Estrutura do Repositório
wine-quality-analysis/
│
├── README.md                 # Documentação do projeto
├── requirements.txt          # Dependências Python
├── wine_quality_analysis.py  # Notebook principal em Python
├── datasets/                 # Datasets utilizados
│   ├── winequalityred.csv
│   └── winequalitywhite.csv
└── images/                   # Imagens geradas (gráficos)
    └── (gráficos serão salvos aqui)
📊 Dataset
O projeto utiliza dois datasets do UCI Machine Learning Repository:

winequalityred.csv: 1.599 amostras de vinhos tintos
winequalitywhite.csv: 4.898 amostras de vinhos brancos
Total combinado: 6.497 amostras

Atributos do Dataset
AtributoDescriçãoUnidadefixed acidityAcidez fixa (ácido tartárico)g/dm³volatile acidityAcidez volátil (ácido acético)g/dm³citric acidÁcido cítricog/dm³residual sugarAçúcar residualg/dm³chloridesCloretos (cloreto de sódio)g/dm³free sulfur dioxideDióxido de enxofre livremg/dm³total sulfur dioxideDióxido de enxofre totalmg/dm³densityDensidadeg/cm³pHAcidez/basicidadeescala 0-14sulphatesSulfatos (sulfato de potássio)g/dm³alcoholTeor alcoólico% vol.qualityQualidade (target)0-10wine_typeTipo de vinhored/white
🔬 Hipóteses Investigadas

Vinhos com maior teor alcoólico tendem a ter melhor qualidade?
Existe correlação entre acidez volátil e qualidade do vinho?
Vinhos tintos e brancos apresentam características químicas diferentes?
A densidade do vinho está relacionada com seu teor alcoólico independentemente do tipo?
Vinhos tintos e brancos têm diferentes fatores determinantes de qualidade?

🚀 Como Executar
Pré-requisitos

Python 3.8 ou superior
Bibliotecas listadas em requirements.txt

Instalação

Clone o repositório:

bashgit clone https://github.com/Adjalma/PUC_RIO.git
cd PUC_RIO

Instale as dependências:

bashpip install -r requirements.txt

Execute o notebook:

bashpython wine_quality_analysis.py
ou execute em Google Colab:
Mostrar Imagem
📈 Principais Resultados
✅ Hipóteses Validadas

Álcool e qualidade: Correlação positiva significativa (r≈0.48)
Acidez volátil: Correlação negativa com qualidade (r≈-0.39)
Diferenças entre tipos: Vinhos tintos e brancos têm padrões químicos distintos
Densidade e álcool: Relação inversa consistente (r≈-0.50)
Fatores de qualidade: Cada tipo tem determinantes específicos

📊 Insights Principais

Vinhos brancos têm distribuição de qualidade mais centrada
Vinhos tintos mostram maior variabilidade nas avaliações
Teor alcoólico é preditor importante para ambos os tipos
Acidez volátil alta prejudica qualidade em ambos os tipos
Equilíbrio químico é crucial para vinhos de alta qualidade

🔧 Técnicas Aplicadas
Análise Exploratória

Estatísticas descritivas detalhadas
Análise de distribuições com histogramas
Boxplots para identificação de outliers
Matriz de correlação com heatmap
Análise comparativa entre tipos de vinho

Pré-processamento

Verificação e tratamento de valores nulos
Identificação e remoção de outliers (método IQR)
Normalização (MinMaxScaler)
Padronização (StandardScaler)
Feature engineering (criação de novas variáveis)
Divisão estratificada treino/teste

📚 Tecnologias Utilizadas

Python 3.8+
Pandas - Manipulação de dados
NumPy - Computação numérica
Matplotlib/Seaborn - Visualização de dados
Scikit-learn - Pré-processamento e ML
Jupyter/Google Colab - Ambiente de desenvolvimento

🤝 Contribuições
Contribuições são bem-vindas! Sinta-se livre para:

Reportar bugs
Sugerir melhorias
Adicionar novas análises
Otimizar código existente

📄 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.
📞 Contato
Autor: Adjalma Machado Aguiar Junior
Email: adjalma.aguiar@icloud.com
LinkedIn: www.linkedin.com/in/adjalma-aguiar

🙏 Agradecimentos

UCI Machine Learning Repository pelos datasets
P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis - autores originais do dataset
Comunidade Python pela disponibilização das bibliotecas utilizadas
