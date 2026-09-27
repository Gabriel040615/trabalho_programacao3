# ENEM e desenvolvimento municipal (2019–2023)

Notebook de análise longitudinal que agrega os microdados públicos do ENEM por município de localização da escola e ano e os relaciona a indicadores do PIB municipal do IBGE.

## Conteúdo

- `Analise_ENEM_Desenvolvimento_Municipal_2019-2023.ipynb`: relatório, método, gráficos executados e código integral de reconstrução.
- `resultados/municipio_ano.csv`: consolidação municipal anual usada pelo notebook.
- `dados/`: fontes INEP e IBGE fornecidas com o projeto.
- `dados_github/`: cópias gzip dos microdados ENEM 2019 e 2020. Os CSVs originais são maiores que o limite por objeto Git LFS e permanecem no disco local, sem alteração.
- `prompt.txt`: enunciado e escopo do trabalho.

Os arquivos grandes de `dados/` e `dados_github/` são rastreados com Git LFS. Para clonar e baixar os arquivos completos, instale Git LFS antes de clonar.

## Executar

Use Python com `pandas`, `numpy` e `IPython` e execute as células do notebook em ordem. A consolidação incluída permite começar sem reler os arquivos brutos. A última seção do notebook reconstrói `resultados/municipio_ano.csv` a partir dos dados disponíveis, incluindo a leitura dos microdados compactados `.csv.gz`.

## Escopo e fontes

As fontes são os microdados do ENEM e materiais de documentação do INEP para 2019–2023 e a planilha PIB dos Municípios 2010–2023 do IBGE. A análise documenta no notebook limitações de cobertura, unidade ecológica, ausência de renda domiciliar, Censo Escolar e denominador populacional elegível. Associações não têm interpretação causal.
