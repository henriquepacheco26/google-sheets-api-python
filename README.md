# Integração Python + Google Sheets

Este projeto demonstra como extrair, transformar e carregar (ETL) dados de um arquivo CSV local para uma planilha do Google Sheets usando Python, pandas e a biblioteca gspread.

O código foi desenvolvido em Jupyter Notebook e segue um fluxo que vai desde a limpeza dos dados até a atualização automatizada de uma aba específica em uma planilha online.

# Funcionalidades:

- Leitura de CSV: importa bases com separador " ; ".

- Limpeza e padronização.

- Remove duplicados.

- Ajusta colunas de códigos (Cód. Paciente, Cód. Admissão) para texto, removendo sufixos " .0 ".

# Transformações:

- Seleção e renomeação de colunas.

- Criação de campos como PERÍODO e OBSERVAÇÃO.

- Conversão de datas e indicadores para formatos adequados.

# Preparação de DataFrame: 

- Organiza colunas na ordem esperada pelo Google Sheets.

# Integração com Google Sheets:

- Autenticação via Service Account (arquivo JSON).

- Conexão com planilha pelo ID.

- Escrita dos dados na aba Consolidado_Teste por meio do método append_row.

# Tecnologias Utilizadas:

- Python 3.x

- pandas — manipulação de dados.

- gspread — integração com Google Sheets.

- oauth2client — autenticação via chave de service account.

- Google Sheets API

# Estrutura do Código

- Imports: bibliotecas de manipulação de dados, autenticação e integração.

- Leitura e limpeza do CSV.

- Transformações e preparação dos dados (rob_hosp).

- Configuração da API do Google Sheets:

- Definição do scope.

- Carregamento das credenciais JSON.

- Autorização do cliente.

- Conexão com a planilha (via spreadsheet_id).

- Escrita dos dados: envio das linhas do DataFrame para o Google Sheets.
