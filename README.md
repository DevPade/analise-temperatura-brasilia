# Análise de Temperatura - Brasília 

Projeto de análise de dados climáticos de Brasília (maio a agosto de 2026), feito para
praticar Python aplicado à análise de dados e como peça de portfólio.

## Sobre o projeto

Com base no meu aprendizado, decidi criar um pequeno projeto para analisar as temperaturas
de Brasília entre maio e agosto. Em busca de um projeto que pudesse apresentar meu trabalho
a outros analistas, fiz uma análise simples e, principalmente, educativa para mim mesmo,
explorando o clima da região.

## Fonte de dados

Os dados vêm da API pública [Open-Meteo](https://open-meteo.com/), que fornece informações
climáticas históricas de qualquer região a partir de latitude e longitude.

## O que foi feito

- Coleta de dados históricos via requisição HTTP (`requests`)
- Limpeza e validação dos dados (checagem de valores faltantes e consistência)
- Conversão e extração de componentes de data/hora (`pandas`)
- Análise exploratória com `pandas` e visualizações com `matplotlib`

## Principais achados

- **Ciclo diário:** temperatura mínima por volta das 6h (~15,9°C) e máxima por volta das
  15h (~26,1°C) — com atraso térmico em relação ao horário de maior sol.
- **Tendência jun/jul:** a temperatura máxima subiu de 27,1°C para 30,1°C, enquanto a
  mínima ficou estável (~12°C) — o aquecimento se concentrou nas tardes, não nas noites.
- **Limitação:** os dados de maio e agosto no dataset são parciais (5 e 12 dias,
  respectivamente), por isso a comparação mensal foi restrita a junho e julho.

## Como rodar

\`\`\`bash
pip install -r requirements.txt
jupyter notebook analise_temperatura.ipynb
\`\`\`

## Tecnologias

Python · pandas · requests · matplotlib · Jupyter

## Gráficos

# ciclo diario com dados brutos
<img width="873" height="470" alt="CICLO DIARIO DE TEMP_BRUTO" src="https://github.com/user-attachments/assets/542f14c2-ce0c-4e20-9a1b-a1f9596df2ec" />
# ciclo diario 
<img width="842" height="470" alt="CICLO DIARIO DE TEMP" src="https://github.com/user-attachments/assets/6d4e3dc4-9d5e-4dc7-b5f8-64e0f179980e" />
# Tendência de temperatura
<img width="1252" height="524" alt="TEND  TEMPERATURA" src="https://github.com/user-attachments/assets/1fc83a5d-f296-4e29-b9e5-a310da6aa6cc" />
# Tendência máxima, mínima e média 
<img width="1252" height="524" alt="MIN_MAX_ MED" src="https://github.com/user-attachments/assets/f49116b3-9df8-4fd1-b935-9ba02352a4ac" />
