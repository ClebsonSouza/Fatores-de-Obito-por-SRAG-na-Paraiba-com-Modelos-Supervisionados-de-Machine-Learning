# Fatores-de-Obito-por-SRAG-na-Paraiba-com-Modelos-Supervisionados-de-Machine-Learning
Fatores de Óbito por Síndrome Respiratória Aguda Grave na Paraíba com Modelos Supervisionados de Machine Learning

# Predição de Óbito por SRAG na Paraíba com Modelos de Aprendizado de Máquina

Este projeto tem como objetivo identificar os principais fatores associados ao óbito por Síndrome Respiratória Aguda Grave (SRAG) no estado da Paraíba, utilizando modelos supervisionados de aprendizado de máquina. A análise foi conduzida com dados do **SIVEP-Gripe**, abrangendo o período de **2022 a 2024**, com foco na construção de modelos preditivos capazes de auxiliar na priorização de recursos clínicos e no suporte à gestão hospitalar.

## Modelos Aplicados

Foram aplicados e comparados cinco algoritmos principais:

- **Regressão Logística**
- **Decision Tree**
- **Random Forest**
- **XGBoost**
- **LightGBM**

Todos apresentaram desempenho satisfatório, com **acurácia superior a 85%** e **AUC acima de 0,89**, demonstrando boa capacidade de discriminar os desfechos. O **LightGBM** obteve os melhores resultados na base de teste, com ótimo equilíbrio entre **precisão**, **recall**, **F1-score** e **AUC**, ainda que os demais modelos tenham apresentado métricas próximas.

Adicionalmente, foi explorada uma **Rede Neural Artificial (RNA)** do tipo *perceptron multicamadas*. A RNA obteve:

- **Acurácia**: 85,16%  
- **Loss**: 0,3525 (base de teste)

Apesar do desempenho competitivo, não superou os modelos baseados em árvores, especialmente o LightGBM, destacando que modelos mais complexos nem sempre oferecem melhores resultados em bases **tabulares e estruturadas**.

## Principais Resultados

As análises indicaram associação significativa entre o risco de óbito e os seguintes fatores:

- Idade avançada
- Presença de comorbidades
- Internação em UTI
- Uso de ventilação invasiva
- Infecção hospitalar
- Desconforto respiratório

> ⚠️ Importante: Algumas dessas variáveis são indicativas de gravidade clínica e não necessariamente causas diretas do óbito, podendo refletir **viés de endogeneidade**.

A **vacinação contra a COVID-19** apresentou efeito protetor estatisticamente significativo, corroborando evidências já estabelecidas na literatura.

## Perspectivas Futuras

Para ampliar a robustez e aplicabilidade dos modelos, recomenda-se:

- 📊 **Expandir a base de dados** com variáveis adicionais:
  - Tempo de permanência na UTI
  - Histórico de tabagismo
  - Uso prévio de medicamentos
  - Tempo entre início dos sintomas e hospitalização
  - Saturação de oxigênio na admissão
  - Coinfecções
- 🧠 **Incorporar dados multimodais**:
  - Exames laboratoriais
  - Imagens radiológicas
  - Prontuários eletrônicos
  - Técnicas de **PLN** e **Visão Computacional**
- 🌍 **Replicar o estudo em outros estados ou regiões** para avaliar a generalização dos modelos
- ⏱️ **Desenvolver modelos dinâmicos** para análise temporal e predições em tempo real
- 🧩 **Investigar estratégias de deployment**:
  - Integração com sistemas clínicos
  - Usabilidade e interpretabilidade
  - Estudos de impacto prático em ambiente hospitalar

## Conclusão

O uso de algoritmos de aprendizado de máquina — com destaque para o **LightGBM** — mostrou-se eficaz na predição do risco de óbito por SRAG no estado da Paraíba. Os resultados obtidos oferecem subsídios valiosos para ações preventivas, decisões clínicas e formulação de políticas públicas em saúde.

A continuidade desta linha de pesquisa, com dados mais completos e diversas fontes, pode aumentar ainda mais o impacto e a aplicabilidade desses modelos no contexto hospitalar e epidemiológico.

---

🔗 Repositório desenvolvido por **Clébson Freire de Souza**
