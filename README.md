# field_spec_data_tests
Desenvolvimento dos modelos preditivos

Os dados espectrais serão submetidos a uma associação de diferentes pré-processamentos para remoção de ruído e/ou intensificação de certas características do sinal espectral. Sobre os dados espectrais será utilizado: (1) primeira e segunda derivada de Savitzky-Golay(SAVITZKY e GOLAY, 1964; GORRY, 1990); (2) correção multiplicativa de espalhamento (MSC) (ISAKSSON e NAES, 1988); e (3) padronização normal de sinal (SNV) (BARNES et al., 1989). Os dados espectrais brutos ou pré-processados de cada amostra serão as variáveis independentes (X – variáveis preditoras), enquanto os atributos de qualidade serão as variáveis dependentes (Y – variáveis respostas). O conjunto de dados será separado na proporção 70-30, ou seja, 70% dos dados irão compor o conjunto de calibração/validação cruzada e 30% o conjunto de predição/validação externa. A validação cruzada será aplicada a todas as amostras do conjunto de calibração. A análise de componentes principais (PCA) será utilizada para fins de análise exploratória, fornecendo informações sobre a estrutura latente da matriz espectral. Também, a PCA será utilizada para detecção de amostras anômalas utilizando os critérios baseados nos parâmetros estatísticos de alavancagem e resíduos de Student. As amostras anômalas serão retiradas quando os limites de alavancagem e resíduos de Student
foram ultrapassados simultaneamente. Os modelos preditivos, baseados nos atributos de qualidade e nos sinais espectrais, serão desenvolvidos através da regressão das componentes principais (PCR), regressão dos quadrados mínimos parciais (PLSR), regressão Support Vector Machine (SVMR), regressão Random Forest (RFR), e regressão redes neurais artificiais (ANNR). O desempenho dos modelos preditivos será avaliado com uso de diferentes parâmetros estatísticos, sendo: coeficiente de determinação (R2); raiz quadrada do erro médio quadrático (RMSE); viés (bias); e relação de previsão para valor de desvio (RPD).
