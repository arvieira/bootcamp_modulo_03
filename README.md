<p align="center">
  <img src="https://raw.githubusercontent.com/arvieira/bootcamp_modulo_03/main/Images/nostradamos.jpg" width = 70%>
</p>

# Projeto: Prevendo Novos Óbitos por COVID19 com o Facebook Prophet
##### Aluno: André Vieira
---
- # Dos Dados:

Os dados analisados nesse estudo são provenientes do site https://brasil.io.
Trata-se de um portal contendo um repositório de dados públicos disponibilizados de maneira adequada para a realização de estudos estatísticos.

Com a pandemia SARS-CoV-2, o site disponibilizou uma equipe para a coleta, aquisição e compilação dos dados referentes a novos casos e óbitos para os municípios do território brasileiro. 
Cabe ressaltar, que os dados presentes no referido site não são divulgados pelo ministério da saúde, o que pode apresentar divergências nas informações apresentadas por aquele.

A tabela utilizada possui os casos confirmados e óbitos obtidos dos boletins das Secretarias Estaduais de Saúde (SES). 
Os dados foram enriquecidos, de forma que a partir do momento em que um município confirma um caso, ele sempre aparecerá nessa tabela (mesmo que para uma determinada data a SES não tenha liberado o boletim - nesse caso é repetido o dado do dia anterior). 
Mais especificamente para este estudo, foram utilizados os dados de óbitos fornecidos por cartórios. 

---
- # Do Objetivo

O objetivo dessa análise é a realização de uma análise exploratória dos dados históricos dos números acumulados e de novos casos de óbitos por covid19 para o estado do Rio de janeiro.
Para tanto, foram obtidas séries históricas dos dados que compõem as os itens pesquisados separados por unidades da federação.
Após a análise exploratória e limpeza dos dados, este estudo terá como foco a criação de configuração de um modelo para realizar a previsão de novos casos para um prazo de 30 dias (1 mês).
Assim como, analisar a qualidade das previsões realizadas pelo modelo construído levando em consideração métricas de erros.

---
- # Da Pergunta
  - Há uma forma de se criar um modelo para realizar as previsões?
  - Qual o erro médio absoluto para cada dia de previsão dentro dos 30 dias seguintes aos dados?

---
- # Da Metodologia Utilizada
Para a análise dos dados e criação do modelo mais adequado, assim como para a avaliação e validação do que será construído, serão adotados as seguintes etapas:
  - Configuração e Importação de Bibliotecas e Dados
  - Análise Exploratória e Tratamento de Dados Faltantes
  - Criação de um Modelo Ingênuo para Previsão de 30 Dias de Novos Óbitos para o Estado do Rio de Janeiro
  - Melhoria do Modelo com Estudo de Pontos de Inflexão
  - Adição de Feriados ao Modelo
  - Avaliação do Tipo de Sazonalidade com Métricas
  - Remoção de Outliers e Avaliação no Impacto de Predição do Modelo com Métricas
  - Validação Cruzada do Modelo Final

---
- # Da Conclusão

Mediante todos os dados analisados e o modelo construído, pode-se concluir que há uma forma de se criar um modelo preditivo para o número de novos óbitos por dia por COVID19 no estado do Rio de Janeiro.
O modelo em questão precisa levar em consideração os feriados do estado e deve utilizar um modelo de sazonalidade multiplicativo.
O erro médio absoluto para o modelo obtido varia de 24 casos com 3 dias a 206 casos com 30 dias.
O modelo em questão pode ser utilizado para o cálculo de risco de novas medidas sanitárias para o estado ou a reabertura gradual após um fechamento dos serviços.
