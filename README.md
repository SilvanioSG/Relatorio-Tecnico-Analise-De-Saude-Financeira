# Análise Financeira e Desempenho de Mercado — WEG S.A. (WEGE3)

<p align="center">
  <img src="SG_Site.png" alt="WEG S.A. — Análise Financeira e Desempenho de Mercado" width="600">
</p>

> Relatório técnico de acompanhamento do desempenho de mercado da **WEG S.A. (WEGE3.SA)**, com pipeline de dados automatizado, indicadores técnicos e visualizações interativas orientadas a negócios.

---

## Destaques do Projeto

- **Atualização Automática:** O pipeline de dados extrai cotações e volumes atualizados em tempo real a cada execução do Jupyter Notebook, garantindo dados sempre atuais via API do Yahoo Finance.
- **Indicadores Técnicos:** Cálculo automático de médias móveis simples (50 e 200 dias) para identificação de tendências operacionais.
- **Visualização Integrada:** Gráficos interativos construídos com a biblioteca Plotly, consolidados em um painel duplo de preços e volumes.
- **Orientação a Negócios:** Análise focada em responder a perguntas estratégicas sobre liquidez, resiliência e estabilidade.

---

## Estrutura do Repositório

```text
├── relatorio_weg.ipynb   # Jupyter Notebook contendo o pipeline de dados e análises
├── SG_Site.png           # Elemento visual para cabeçalho do relatório
└── README.md             # Documentação do repositório
```

---

## Requisitos de Execução

As bibliotecas necessárias para executar a análise são:

- **Python 3.8+**
- **pandas**
- **numpy**
- **yfinance**
- **plotly**

### Instalação das Dependências

```bash
pip install pandas numpy yfinance plotly
```

---

## Como Executar o Projeto

1. **Clone o repositório:**

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

2. **Acesse o diretório do projeto:**

```bash
cd seu-repositorio
```

3. **Instale as dependências:**

```bash
pip install pandas numpy yfinance plotly
```

4. **Abra o Jupyter Notebook:**

```bash
jupyter notebook relatorio_weg.ipynb
```

5. **Execute todas as células** para gerar a análise atualizada com os dados mais recentes do mercado.

---

## Atualização Automática dos Dados

> **Nota de Atualização:** Este relatório utiliza dados extraídos dinamicamente. A cada nova execução do código, os indicadores, cotações e volumes são atualizados automaticamente com os dados mais recentes da B3, por meio da API do Yahoo Finance.

O diferencial deste projeto é que o pipeline foi construído para **atualização automatizada**: a cada execução do script, a API do Yahoo Finance reflete as cotações e volumes diários mais recentes da B3, garantindo dados sempre atuais para a análise de tomada de decisão.

---

## Visão Geral da Análise

O relatório aborda os seguintes aspectos do desempenho de mercado da WEG S.A.:

- **Liquidez:** Análise dos volumes negociados e sua evolução ao longo do tempo.
- **Resiliência:** Comportamento do preço das ações em diferentes cenários de mercado.
- **Estabilidade:** Identificação de tendências por meio de médias móveis e indicadores técnicos.
- **Tomada de Decisão:** Consolidação de dados que subsidiam decisões estratégicas de negócio.

---

## Autor

**Silvânio Gois**

- **Cargo:** Gestor de Operações e Negócios Orientado a Dados
- **Website:** [silvaniogois.com.br](https://silvaniogois.com.br)
- **LinkedIn:** [linkedin.com/in/silvanio-gois](https://linkedin.com/in/silvanio-gois)
- **E-mail:** [sg@silvaniogois.com.br](mailto:sg@silvaniogois.com.br)

---

## Licença

Este projeto é de uso livre para fins educacionais e de análise de dados. Consulte o autor para mais informações sobre uso comercial.

---

<div align="center">
  <sub>Desenvolvido com foco em dados, estratégia e tomada de decisão orientada a negócios.</sub>
</div>