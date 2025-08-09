# 📉 Análise de Cancelamentos de Clientes

Este projeto realiza uma análise detalhada dos cancelamentos de clientes com base em uma base de dados fictícia. Utilizando **Python**, **Pandas** e **Plotly**, o objetivo é identificar padrões de comportamento que levam ao cancelamento e propor ações estratégicas para reduzir a evasão.

## 🧪 Tecnologias Utilizadas

- Python 3.x
- Pandas
- Plotly Express
- Jupyter Notebook (opcional)
- CSV como fonte de dados

## 📊 Base de Dados

O arquivo `cancelamentos_sample.csv` contém 50.000 registros com as seguintes colunas:

- `idade`
- `sexo`
- `tempo_como_cliente`
- `frequencia_uso`
- `ligacoes_callcenter`
- `dias_atraso`
- `assinatura`
- `duracao_contrato`
- `total_gasto`
- `meses_ultima_interacao`
- `cancelou` (1 = cancelou, 0 = manteve)

## 📈 Etapas da Análise

1. **Importação e limpeza dos dados**
   - Remoção de colunas irrelevantes (`CustomerID`)
   - Exclusão de linhas com valores nulos

2. **Análise inicial**
   - Percentual de clientes que cancelaram: **56.8%**
   - Visualização com histogramas coloridos por status de cancelamento

3. **Identificação de padrões**
   - Todos os clientes com contrato mensal cancelaram
   - Clientes que ligam mais de 4 vezes para o call center tendem a cancelar
   - Atrasos acima de 20 dias aumentam drasticamente o risco de cancelamento

4. **Aplicação de filtros estratégicos**
   - Exclusão de contratos mensais
   - Limite de até 4 ligações ao call center
   - Atrasos de até 20 dias

5. **Resultado pós-análise**
   - Percentual de cancelamentos caiu para **18.3%**
   - Redução de **38%** nos cancelamentos

## 📊 Visualizações

Gráficos interativos foram gerados com Plotly para cada variável, facilitando a identificação de padrões visuais.

## 📁 Estrutura do Projeto
├── cancelamentos/ 
├── cancelamentos_sample.csv 
├── analise_cancelamentos.py



## ▶️ Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/ferreira-08/vendas.git
   cd vendas

   Instale as dependências:
   
   pip install pandas plotly
   
Execute o script:

python analise_cancelamentos.py

##💡 Insights estratégicos
Oferecer descontos em planos trimestrais e semestrais

Melhorar atendimento para evitar mais de 3 ligações

Criar políticas para resolver pendências em até 10 dias
   
   
