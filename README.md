
# Dashboard de Criptomoedas com [Reactjs e Vite](https://pt.vitejs.dev/guide/)

O commit inicial deve incluir as configurações básicas do Reactjs com Vite:
```bash
git add .
git commit -m "ADS-init: <sua_matricula> Reactjs-vite"
```

### Objetivo do INIT
Nessa etapa, o projeto deve ser iniciado do zero para garantir um histórico de evolução completo. A escolha do repositório é livre, mas o histórico de commits e o código-fonte devem estar visíveis para avaliação.

# Iniciando o Projeto
Todos os arquivos criados devem conter a data, nome e matrícula, além de uma breve descrição sobre o documento.

### Exemplo de Documentação em Arquivos
```js
/**
 * Nome do arquivo: exemplo.js
 * Data de criação: 30/04/2024
 * Autor: João Silva
 * Matrícula: 123456
 *
 * Descrição:
 * Este arquivo JavaScript é responsável por implementar as funcionalidades
 * de interação do usuário com a interface gráfica do módulo de vendas.
 * Aqui são tratados eventos de cliques, validações de entrada e comunicação
 * com APIs para envio e recebimento de dados.
 */
```

---

### Funcionalidades do Dashboard de Criptomoedas

1. **Exibição de Criptomoedas Populares**
   - A tabela exibe informações de 10 criptomoedas populares, incluindo:
     - **Nome da Criptomoeda e Símbolo**: Nome completo da moeda (ex.: "Bitcoin") e símbolo abreviado (ex.: "BTC").
     - **Imagem**: Ícone da criptomoeda exibido ao lado do nome para fácil identificação.
     - **Preço Atual em USD**: Mostra o preço atual da criptomoeda em dólares americanos.
     - **Variação em 24 Horas**: Exibe a variação percentual do preço nas últimas 24 horas. O valor é colorido em **verde** para aumento e **vermelho** para queda.
   
   - **Exemplo de Commit**:
     ```bash
     git commit -m "ADS-tabela_criptomoedas: <sua_matricula> Reactjs-vite"
     ```

2. **Campo de Busca**
   - Um campo de busca permite ao usuário filtrar as criptomoedas pelo nome ou símbolo.
   - O usuário pode digitar parte do nome ou símbolo (ex.: "bit" para Bitcoin) para exibir apenas as criptomoedas que atendem ao critério.

   - **Exemplo de Commit**:
     ```bash
     git commit -m "ADS-filtro_busca: <sua_matricula> Reactjs-vite"
     ```

3. **Ordenação de Colunas**
   - O dashboard permite ordenar os dados da tabela clicando nos cabeçalhos das colunas. As opções incluem:
     - **Ordenação por Nome**: Clicando no cabeçalho "Criptomoeda", a tabela organiza os dados em ordem alfabética (ascendente ou descendente).
     - **Ordenação por Preço**: Clicando no cabeçalho "Preço (USD)", as criptomoedas são ordenadas pelo preço atual em USD, do maior para o menor ou vice-versa.
     - **Ordenação por Variação em 24 Horas**: Ao clicar no cabeçalho "Variação 24h (%)", a tabela ordena os dados com base na variação percentual nas últimas 24 horas, para visualizar as criptomoedas que mais subiram ou caíram.
   - Ícones (▲ e ▼) indicam a direção de ordenação para cada coluna, facilitando o entendimento do usuário.

   - **Exemplo de Commit**:
     ```bash
     git commit -m "ADS-ordenacao_colunas: <sua_matricula> Reactjs-vite"
     ```

4. **Carregamento Dinâmico dos Dados**
   - A tabela faz uma chamada à API da CoinGecko para buscar dados atualizados das criptomoedas.
   - Enquanto os dados estão sendo carregados, uma mensagem "Carregando..." é exibida para indicar que a tabela estará disponível em breve.
   - Em caso de erro, uma mensagem de erro é exibida no console para auxiliar na depuração.

   - **Exemplo de Commit**:
     ```bash
     git commit -m "ADS-carregamento_dinamico: <sua_matricula> Reactjs-vite"
     ```

---

### Exemplo de Consulta à API CoinGecko

Abaixo está um exemplo de configuração da URL para buscar dados de criptomoedas usando a CoinGecko. Esta configuração especifica o uso do dólar americano como moeda (`vs_currency: "usd"`), ordena os dados pela capitalização de mercado em ordem decrescente (`order: "market_cap_desc"`), e limita a exibição a 10 criptomoedas por página.

```json
"https://api.coingecko.com/api/v3/coins/markets",
{
  params: {
    vs_currency: "usd",
    order: "market_cap_desc",
    per_page: 10,
    page: 1,
    sparkline: false
  }
}
```

---

### Histórico de Commits

Para garantir o acompanhamento do desenvolvimento e manutenção do projeto, cada funcionalidade deve ser devidamente commitada no Git, conforme os exemplos de commits fornecidos para cada funcionalidade. Abaixo, estão as instruções gerais para versionamento no Git.

1. **Configurações Iniciais do Projeto**:
   - Adicione o conteúdo inicial do projeto:
     ```bash
     git add .
     git commit -m "ADS-init: <sua_matricula> Reactjs-vite"
     ```

2. **Adicionando Funcionalidades e Melhorias**:
   - Para cada nova funcionalidade ou atualização, siga o padrão de nomenclatura conforme mostrado:
     ```bash
     git commit -m "ADS-nome_da_funcionalidade: <sua_matricula> Reactjs-vite"
     ```
   - Exemplos adicionais:
     - **Filtro Alfanumérico**: `git commit -m "ADS-filtro_alfanumerico: <sua_matricula> Reactjs-vite"`
     - **Ícones de Ordenação**: `git commit -m "ADS-icones_ordenacao: <sua_matricula> Reactjs-vite"`
---

### Estrutura do Projeto

Certifique-se de que todos os arquivos e funcionalidades estão devidamente documentados com a data, o nome do autor e a matrícula, para facilitar a revisão e manutenção do código-fonte. Seguindo as orientações e exemplos de commits, o projeto deverá estar bem organizado e apresentará um histórico claro de desenvolvimento.

![image](https://github.com/user-attachments/assets/42c967b3-f96f-4d8a-89c1-d3c0dc69d32e)

## Serão zerados caso os critérios de commit não sejam sequidos, se os arquivos criados pelo autor não contiverem suas credenciais ou plagio.
_____
## A data de entrega e apresentações está definida para o período de 29/10 a 31/11. Recomendo que concluam suas tarefas omais cedo possível, preferencialmente antes do dia 28, para evitar conflitos de última hora, atrasos nas notas ou quaisquer surpresas desagradáveis.



