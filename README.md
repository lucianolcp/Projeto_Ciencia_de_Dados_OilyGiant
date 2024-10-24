## Visão Geral
Este projeto tem o objetivo de encontrar os melhores locais para desenvolver novos poços de petróleo, para uma empresa fictícia de mineração chamada OilyGian. Envolve a leitura de dados sobre poços existentes, construção de modelos preditivos e análise de riscos e lucros.

## Etapas do Projeto
1. **Leitura de Dados**: Importar arquivos com dados de poços de petróleo das regiões selecionadas.
2. **Modelagem Preditiva**: Construir um modelo de regressão linear para prever o volume de reservas em novos poços.
3. **Seleção de Poços**: Identificar os poços com os maiores valores estimados de reservas.
4. **Análise de Lucro**: Escolher a região que apresenta o maior lucro total dos poços selecionados.
5. **Análise de Risco**: Utilizar Bootstrapping para avaliar o lucro potencial e riscos associados.

## Descrição dos Dados
Os dados de exploração geológica estão disponíveis nos seguintes arquivos:
- `geo_data_0.csv`
- `geo_data_1.csv`
- `geo_data_2.csv`

**Colunas dos Dados**:
- `id`: Identificador único do poço de petróleo
- `f0`, `f1`, `f2`: Características geológicas dos poços
- `product`: Volume de reservas no poço de petróleo (em milhares de barris)

## Execução
1. **Preparação dos Dados**: Baixar e preparar os dados, documentando o procedimento.
2. **Treinamento e Teste do Modelo**:
   - Dividir os dados em conjuntos de treinamento e validação (75:25).
   - Treinar o modelo e prever para o conjunto de validação.
   - Calcular o REQM para avaliar a precisão das predições.
   - Armazenar as previsões e respostas corretas.
   - Analisar os resultados.
3. **Cálculo de Lucro**:
   - Armazenar valores necessários para cálculos.
   - Comparar o volume médio de cada região com a média necessária para evitar prejuízos.
4. **Função de Cálculo de Lucro**:
   - Selecionar os 200 poços com os maiores volumes previstos.
   - Calcular e resumir o lucro potencial.
5. **Análise de Riscos**:
   - Utilizar Bootstrapping para calcular distribuição de lucros, lucro médio, intervalo de confiança e risco de prejuízo.

## Ferramentas e Bibliotecas Utilizadas
- **Python**: Linguagem principal utilizada para a análise.
- **Pandas**: Manipulação e análise de dados.
- **Scikit-learn**: Modelagem preditiva e machine learning.
- **NumPy**: Computação numérica e suporte a arrays.

## Conclusão Final
### Região Recomendada: Região 1

**Justificativa**:
- **Baixo Risco de Prejuízo**: Região 1 apresenta um risco de prejuízo de apenas 0.10%.
- **Lucro Médio Competitivo**: O lucro médio é competitivo em relação à Região 0, com menor risco.
- **Intervalo de Confiança**: Estreito e não inclui valores negativos, reforçando a estabilidade da previsão de lucro.

Portanto, com base nas análises de lucro e risco, a Região 1 é a melhor escolha para o desenvolvimento de novos poços de petróleo.

## Aprendizados

Este projeto permitiu-me desenvolver as seguintes habilidades:

- **Análise de Dados**: Aprendi a manipular e explorar grandes conjuntos de dados utilizando a biblioteca Pandas.
- **Modelagem Preditiva**: Aprofundei meus conhecimentos em regressão linear e sua aplicação na previsão de volumes de reservas.
- **Avaliação de Modelos**: Entendi como calcular e interpretar métricas de desempenho como o REQM, para avaliar a precisão das predições.
- **Bootstrapping**: Aprendi a aplicar técnicas de Bootstrapping para análise de risco e distribuição de lucros, melhorando minha capacidade de tomar decisões informadas.
- **Tomada de Decisões Baseadas em Dados**: Desenvolvi a habilidade de usar dados para justificar escolhas estratégicas, como a seleção de regiões para novos poços de petróleo.
- **Documentação e Organização**: Melhorei minhas habilidades em documentar processos e resultados, tornando o projeto mais acessível e compreensível para outros.
- **Trabalho com Dados Sintéticos**: Aprendi a lidar com dados sintéticos e entender suas limitações e aplicações práticas.

Esses aprendizados contribuíram significativamente para meu desenvolvimento como profissional na área de ciência de dados e análise de negócios.

## Como Executar o Projeto

- Clone o repositório.
- Navegue até o diretório do projeto.
- Abra o projeto no seu IDE favorito.
- Instale as dependências.
- Execute o script principal.

## Contato

Luciano Pinto
[LinkedIn](https://www.linkedin.com/in/lucianolcp/)  
Email: dslucianopinto@gmail.com
