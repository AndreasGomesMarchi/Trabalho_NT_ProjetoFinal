🎮 Predição de Preços de Jogos da Steam

Sobre o Projeto

Este projeto foi desenvolvido para a disciplina de Novas Tecnologias e tem como objetivo aplicar técnicas de Ciência de Dados e Machine Learning na previsão do preço de jogos da plataforma Steam.

Utilizando uma base de dados pública contendo informações sobre milhares de jogos, foram realizadas todas as etapas de um projeto de Machine Learning:

* Preparação e limpeza dos dados;
* Análise estatística;
* Visualização dos dados;
* Treinamento do modelo;
* Avaliação do desempenho;
* Simulação de uso em um cenário real.

O modelo desenvolvido é capaz de estimar o preço de um jogo com base em características como avaliações, tempo médio de jogo, gêneros, sistema operacional suportado, pontuação da crítica, entre outras variáveis.

⸻

📂 Estrutura do Projeto

.
├── Projeto_NT.ipynb          # Notebook principal
├── games_march2025_full.csv  # Base de dados original
├── X_train.csv               # Conjunto de treino
├── X_test.csv                # Conjunto de teste
├── y_train.csv               # Variável alvo (treino)
├── y_test.csv                # Variável alvo (teste)
├── modelo_rf_final.pkl       # Modelo treinado
└── README.md

⸻

👥 Divisão das Responsabilidades

O desenvolvimento foi dividido entre cinco integrantes, seguindo as etapas clássicas de um projeto de Machine Learning.

Integrante 1 — Engenharia de Dados

Responsável por:

* Importação da base de dados;
* Limpeza dos dados;
* Tratamento de valores ausentes;
* Transformação das variáveis categóricas;
* Separação entre treino e teste.

⸻

Integrante 2 — Análise Exploratória

Responsável por:

* Estatísticas descritivas;
* Distribuições das variáveis;
* Identificação de outliers;
* Caracterização da base de dados.

⸻

Integrante 3 — Visualização dos Dados

Responsável por:

* Histogramas;
* Boxplots;
* Heatmap de correlação;
* Visualizações para geração de insights.

⸻

Integrante 4 — Modelagem

Responsável por:

* Construção do modelo Random Forest Regressor;
* Treinamento;
* Ajuste de hiperparâmetros;
* Salvamento do modelo treinado.

⸻

Integrante 5 — Validação e Simulação

Responsável por:

* Validação final utilizando o conjunto de teste;
* Cálculo das métricas MAE, RMSE e R²;
* Simulação de uso utilizando um jogo fictício;
* Conclusão da aplicação prática do modelo.

⸻

🧠 Modelo Utilizado

Foi utilizado o algoritmo:

Random Forest Regressor

Biblioteca:

* Scikit-Learn

Esse algoritmo foi escolhido por apresentar bom desempenho em problemas de regressão envolvendo relações não lineares entre as variáveis.

⸻

📊 Métricas Utilizadas

O desempenho do modelo foi avaliado utilizando:

* MAE (Mean Absolute Error)
* RMSE (Root Mean Squared Error)
* R² (Coeficiente de Determinação)

Essas métricas permitem avaliar a precisão das previsões realizadas pelo modelo.

⸻

▶️ Como Executar

1. Clonar o repositório

git clone <URL_DO_REPOSITORIO>
cd <REPOSITORIO>

⸻

2. Instalar o Git LFS

Este projeto utiliza Git Large File Storage (Git LFS) devido ao tamanho dos arquivos CSV e do modelo treinado.

Caso ainda não possua o Git LFS instalado:

git lfs install

Após clonar o projeto:

git lfs pull
git lfs checkout

⸻

3. Instalar as bibliotecas

pip install pandas numpy matplotlib seaborn scikit-learn joblib

⸻

4. Executar o Notebook

Abra o arquivo

Projeto_NT.ipynb

e execute todas as células em ordem.

⸻

⚠️ Observações

Este projeto utiliza arquivos grandes armazenados através do Git LFS.

Caso algum arquivo CSV apresente apenas o conteúdo:

version https://git-lfs.github.com/spec/v1

execute novamente:

git lfs pull
git lfs checkout

⸻

Compatibilidade do modelo

O arquivo modelo_rf_final.pkl foi gerado em um ambiente específico de desenvolvimento.

Dependendo das versões instaladas de NumPy e Scikit-Learn, pode ocorrer incompatibilidade durante seu carregamento.

Para garantir a execução completa do projeto em diferentes ambientes, a Seção 5 do notebook implementa uma rotina de contingência: caso o modelo salvo não possa ser carregado, um novo modelo é treinado automaticamente utilizando os mesmos dados de treino e os mesmos hiperparâmetros empregados originalmente.

⸻

📚 Tecnologias Utilizadas

* Python 3
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Joblib
* Git
* Git LFS
* Jupyter Notebook

⸻

🎯 Objetivo Acadêmico

Este projeto tem finalidade exclusivamente educacional e foi desenvolvido como atividade avaliativa da disciplina de Novas Tecnologias, aplicando conceitos de Ciência de Dados, Engenharia de Dados e Machine Learning em um problema real envolvendo dados da plataforma Steam.
