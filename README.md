# 📈 Perfil dos investidores do Tesouro Direto (2002–06/2025): uma análise descritiva por razões de chances

## 💡 Sobre este Projeto
Este repositório reúne a análise descritiva sobre o perfil dos investidores do Tesouro Direto, utilizando técnicas estatísticas e de modelagem por razões de chances (logistic odds). O objetivo é investigar como características como faixa de adesão ao programa, profissão agrupada, região de residência, estado civil agrupado, gênero e faixa etária se associam ao investor ter operado nos últimos 12 meses no programa. Antes da análise, considerei os investidores ativos, o que significa que ele ainda opera no programa.

Esta pesquisa integra conceitos de estatística aplicada, ciência de dados e finanças públicas, com foco na compreensão do comportamento do investidor brasileiro diante da evolução do acesso ao Tesouro Direto e das mudanças no cenário econômico e tecnológico nacional.


## 📂 Estrutura do Projeto
```
00002_investidores_tesouro_direto/
│
├── figuras_tcc/                     
│   └── imagens e gráficos gerados para visualização
│
├── metadados/                       
│   └── dicionários de variáveis, descrições e documentação dos campos
│
├── 01_analise_exploratoria_e_tratamento_dados.ipynb   # EDA inicial e limpeza
├── 02_analise_dados_limpOS.ipynb                      # base filtrada e tratada
├── 03_regressao_logistica                             # análise de razões de chances
├── 04_analises_adicionais                             # gráficos adicionais
│
├── base_atualizada.csv                                # dataset completo raw original (após coleta)
├── df_atualizado.csv                                  # dataset final tratado para análise
│
└── README.md                                          # documentação do projeto
│
└── requirements                                       # requisitos do projeto

```

## 📊 Licença e Fonte dos Dados
Os dados utilizados neste projeto são provenientes do dataset "Investidores do Tesouro Direto — base completa", disponibilizado pelo Ministério da Fazenda / Tesouro Nacional por meio do Portal Brasileiro de Dados Abertos:

https://dados.gov.br/dados/conjuntos-dados/investidores-do-tesouro-direto

Este conjunto de dados contém registros de investidores cadastrados no programa Tesouro Direto. Caso um investidor possua cadastro em mais de uma instituição financeira, cada vínculo é registrado como uma nova linha associada ao mesmo código identificador.

**Observações sobre o uso dos dados**

- Os dados são públicos e disponibilizados conforme a Lei de Acesso à Informação (Lei nº 12.527/2011) e diretrizes de dados abertos do Governo Federal.
- Este projeto não possui qualquer vínculo oficial com o Ministério da Fazenda ou Tesouro Nacional.
- A responsabilidade pela geração, manutenção e exatidão dos dados é do órgão público que os publica originalmente.

## 🧠 Tecnologias utilizadas
- Python.
- Pandas, matplotlib, seaborn, numpy, statsmodels, wordcloud.
- VS code.  

## 🚀 Como reproduzir
1. Clone este repositório
git clone git@github.com:NathaliaMainenti/perfil_dos_investidores_do_tesouro_direto_2022-06.2025.git
cd perfil_dos_investidores_do_tesouro_direto_2022-06.2025

2. Crie um ambiente virtual (opcional, mas recomendado)
python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows

3. Instale as dependências
pip install -r requirements.txt

4. Execute os notebooks na ordem
01_analise_exploratoria_e_tratamento_dados.ipynb   -> limpeza e padronização dos dados
02_analise_dados_limpOS.ipynb                      -> dataset final tratado
03_regressao_logistica.ipynb                       -> análise estatística, razões de chances e interpretação
