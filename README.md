# Análise Financeira e Desempenho de Mercado — WEG S.A. (WEGE3)

<p align="center">
  <img src="SG_Site.png" alt="WEG S.A. — Análise Financeira e Desempenho de Mercado" width="400">
</p>

<p align="center">
  <a href="https://silvaniosg.github.io/Relatorio-Tecnico-Analise-De-Saude-Financeira/" target="\_blank">
    <img src="https://img.shields.io/badge/🌐\_Acessar\_Relatório\_Online-Click\_Aqui-success?style=for-the-badge" alt="Acessar Relatório Online">
  </a>
  <a href="https://github.com/SilvanioSG/Relatorio-Tecnico-Analise-De-Saude-Financeira/actions/workflows/publish.yml" target="\_blank">
    <img src="https://github.com/SilvanioSG/Relatorio-Tecnico-Analise-De-Saude-Financeira/actions/workflows/publish.yml/badge.svg" alt="Status do Pipeline">
  </a>
</p>

> Relatório técnico de acompanhamento do desempenho de mercado da \*\*WEG S.A. (WEGE3.SA)\*\*, com pipeline de dados 100% automatizado, indicadores técnicos e visualizações interativas orientadas a negócios.

&#x20;[**Clique aqui para acessar a versão web atualizada e interativa**](https://silvaniosg.github.io/Relatorio-Tecnico-Analise-De-Saude-Financeira/)

\---

## Destaques do Projeto

* **Atualização Automática Diária:** O pipeline de dados é executado de segunda a sexta (após o fechamento do mercado) via **GitHub Actions**, extraindo cotações e volumes em tempo real pela API do Yahoo Finance.
* **Publicação Contínua (CI/CD):** O Jupyter Notebook é executado em um ambiente headless, convertido para HTML limpo (sem expor o código-fonte) e publicado automaticamente no **GitHub Pages**.
* **Indicadores Técnicos:** Cálculo automático de médias móveis simples (MM50 e MM200) para identificação de tendências operacionais.
* **Visualização Integrada:** Gráficos interativos construídos com a biblioteca Plotly, consolidados em um painel duplo de preços e volumes.
* **Orientação a Negócios:** Análise focada em responder a perguntas estratégicas sobre liquidez, resiliência e estabilidade.

\---

## Perguntas de Negócio e Respostas

### **Pergunta 1:** A tendência recente do preço de fechamento indica um ciclo de expansão ou de consolidação em relação às médias históricas?

> \*\*Resposta:\*\* O preço de fechamento da WEGE3.SA manteve-se predominantemente acima da Média Móvel de 200 dias (MA200) ao longo do período analisado, o que confirma uma tendência estrutural de alta no longo prazo. O alinhamento das médias (MA50 sobrepondo a MA200) sinaliza momentos recorrentes de \*Golden Cross\*, caracterizando apetite comprador e confiança nas entregas operacionais da empresa.

### **Pergunta 2:** Existe correlação entre picos de volume negociado e mudanças na tendência do preço da ação?

> \*\*Resposta:\*\* Os picos significativos no volume diário de negociação concentram-se em janelas pós-divulgação de balanços trimestrais (RI) e rebalanceamentos de carteiras institucionais. Esse comportamento evidencia que oscilações de preço pontuais não são motivadas por especulações desordenadas, mas sim por reajustes de valor intrínseco com respaldo fundamentalista.

### **Pergunta 3:** Quais métricas de estabilidade operacional e liquidez a WEG entrega para subsidiar decisões de investimento de longo prazo?

> \*\*Resposta:\*\* A consistência no padrão das oscilações da WEG reflete sua forte saúde financeira:
> \* \*\*Baixa Dependência de Alavancagem Excessiva:\*\* Protege a empresa em ciclos de juros elevados.
> \* \*\*Diversificação Geográfica:\*\* Atua como um \*hedge\* natural contra flutuações do cenário macroeconômico doméstico.

\---

## Estrutura do Repositório

```text
├── .github/workflows/
│   └── publish.yml       # Pipeline de CI/CD (GitHub Actions) para execução e deploy
├── RelatorioTecnicoAnaliseDeSaudeFinanceira.ipynb  # Jupyter Notebook com as análises
├── requirements.txt      # Dependências do projeto
├── SG\_Site.png           # Elemento visual para cabeçalho do relatório
└── README.md             # Documentação do repositório
```

\---

## Requisitos de Execução (Ambiente Local)

Caso deseje reproduzir a análise localmente, as bibliotecas necessárias são:

* Python 3.8+
* pandas
* numpy
* yfinance
* plotly
* jupyter / nbconvert

### Instalação das Dependências

```bash
pip install -r requirements.txt
```

\---

## Como Executar o Projeto Localmente

1. **Clone o repositório:**

```bash
   git clone https://github.com/SilvanioSG/Relatorio-Tecnico-Analise-De-Saude-Financeira.git
   ```

2. **Acesse o diretório:**

```bash
   cd Relatorio-Tecnico-Analise-De-Saude-Financeira
   ```

3. **Instale as dependências:**

```bash
   pip install -r requirements.txt
   ```

4. **Abra o Jupyter Notebook:**

```bash
   jupyter notebook RelatorioTecnicoAnaliseDeSaudeFinanceira.ipynb
   ```

5. **Execute todas as células** para gerar a análise atualizada com os dados mais recentes do mercado.

\---

## Como Funciona a Atualização Automática Online

O projeto utiliza o **GitHub Actions** como esteira de automação. O fluxo ocorre da seguinte forma:

1. O agendador (*cron*) do GitHub dispara o workflow de segunda a sexta às 19h (horário de Brasília), logo após o fechamento da B3. (Também pode ser disparado manualmente clicando em *Run workflow* na aba **Actions**).
2. O robô instala as dependências em um ambiente virtual Linux.
3. O `nbconvert` executa o notebook silenciosamente (capturando os dados mais recentes via `yfinance`) e o converte para um arquivo `index.html`.
4. O arquivo final é publicado automaticamente na branch do **GitHub Pages**, ficando disponível na web para qualquer usuário, sem necessidade de instalação de software.

\---

## Autor

**Silvânio Gois**

* **Cargo:** Gestor de Operações e Negócios Orientado a Dados
* **Website:** [silvaniogois.com.br](https://silvaniogois.com.br)
* **LinkedIn:** [linkedin.com/in/silvanio-gois](https://linkedin.com/in/silvanio-gois)
* **GitHub:** [github.com/SilvanioSG](https://github.com/SilvanioSG)
* **E-mail:** sg@silvaniogois.com.br

\---

## Licença

Este projeto é de uso livre para fins educacionais e de análise de dados. Consulte o autor para mais informações sobre uso comercial.

<div align="center">
  <sub>Desenvolvido com foco em dados, estratégia e tomada de decisão orientada a negócios.</sub>
</div>

