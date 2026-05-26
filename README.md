# 📊 Dashboard de Performance das pricipais Seleções Mundiais (2023-2025)

![Status](https://shields.io)
![Ferramenta](https://shields.io)

## 📌 Visão Geral do Projeto
Este projeto analisa dados históricos de desempenho técnico de 6 das principais federações de futebol do mundo: **França, Argentina, Brasil, Inglaterra, Espanha e Holanda**. O painel foi construído para monitorar a evolução do aproveitamento, eficiência de ataque e o balanço de resultados ao longo das temporadas de 2023 a 2025.

---

## 📉 Estrutura do Dashboard

O painel é composto por 5 visualizações principais combinadas com indicadores de KPI:
1. **Performance por Seleção:** Gráfico de barras empilhadas detalhando o balanço absoluto de Vitórias, Empates e Derrotas.
2. **Média de Aproveitamento por Ano e Seleção:** Gráfico de linhas focado em tendências temporais e consistência de performance de 2023 a 2025.
3. **Jogos por Seleções:** Gráfico de colunas indicando a amostragem de dados e carga de partidas de cada país.
4. **Gols Marcados por Seleção:** Gráfico de rosca trazendo o *Market Share* de gols do ecossistema estudado.
5. **Matrizes de KPI (Rodapé):** Cartões calculados dinamicamente mostrando a **Média de Gols por Partida**.

---

## 🚀 Tecnologias e Competências Técnicas
* **ETL (Power Query):** Limpeza, tratamento de nulos e estruturação da base de dados das partidas.
* **Modelagem:** Criação de tabelas e relacionamentos ótimos para filtros cruzados.
* **DAX (Data Analysis Expressions):** Desenvolvimento de medidas para KPIs agregados e médias ponderadas.
    ```dax
    Media Gols por Partida = 
    DIVIDE(
        SUM(estatisticas_selecoes[Gols_Marcados]); 
        SUM(estatisticas_selecoes[Jogos]); 
        0
    )
    ```

---

## 💡 Como Visualizar o Projeto
1. Baixe o arquivo `.pbix` disponível neste repositório.
2. Abra no seu Power BI Desktop para interagir com os filtros de ano e seleção.

