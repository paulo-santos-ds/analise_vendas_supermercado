# 🚀 Coleta de Dados para Análise de Produtos

## 📋 Decrição do projeto

Este projeto realiza o web scraping de Variação de preços de produtos do supermercado, processa os dados extraídos e 
os apresenta em um dashboard interativo. A estrutura é organizada para facilitar o fluxo de 
coleta, transformação e visualização dos dados.


```bash

SCRAPING_RELOGIO_MASCULINO/
├── .venv/                       # Ambiente virtual para dependências do Python
├── dados/                       # Diretório para armazenamento de dados coletados
├── src/
│   ├── coleta/
│   │   ├── spiders/
│   │   │   └── mercado.py      # Spider para extração de dados 
│   │   ├── items.py            # Definição do modelo de dados
│   │   ├── middlewares.py      # Middlewares para processamento durante o scraping
│   │   ├── pipelines.py        # Pipeline para processamento pós-coleta
│   │   └── settings.py         # Configurações do Scrapy
│   ├── dashboard/
│   │   └── app.py              # Aplicação de dashboard para visualização dos dados
│   └── transform/
│       └── main.py             # Script para transformação e carga dos dados coletados
├── .gitignore                  # Arquivos a serem ignorados pelo Git
├── .python-version             # Versão do Python utilizada no projeto
├── Pipeline.jpg                # Imagem ilustrativa do fluxo do pipeline
└── README.md                   # Documentação do projeto
```

## 💻 Funcionalidades
1. Extração de Dados (Extract)
- 🔍 Coleta automatizada de dados de relógios masculinos do Mercado Livre
- 📦 Extração de informações como preços, avaliações, marcas e categoria
- 💾 Armazenamento inicial em formato JSONL
2. Transformação (Transform)
- 🧹 Limpeza e padronização dos dados
- 🔄 Tratamento de valores nulos
- 📊 Conversão de tipos de dados
- 💰 Cálculos de preços totais
3. Carga (Load)
- 🗄️ Armazenamento em banco de dados SQLite
- ⚡ Estruturação otimizada para consultas
4. Visualização (Dashboard)
- 📈 KPIs principais do negócio
- 🏆 Rankings de produtos e marcas
- 📉 Análises de preços e avaliações
- 📊 Gráficos interativos
- 🔧 Como Executar
