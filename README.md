# Class Imbalance in Binary Classification

## Descrição  
Este projeto explora estratégias para lidar com **desbalanceamento de classes** em problemas de classificação binária. Empregando o algoritmo **XGBoost** em duas variantes: a implementação canónica e uma versão modificada com ajustes específicos para datasets desbalanceados, avaliamos o seu impacto em métricas como **G-mean**, **precision**, **recall** e **AUC**.  

Desenvolvido na **Faculdade de Ciências da Universidade do Porto (FCUP)** para a disciplina **Aprendizagem Computacional 1**.

---

## Funcionalidades

- **Preparação e Exploração de Dados**  
  - Carregamento de datasets desbalanceados via `pandas.read_csv`.  
  - Cálculo da razão de desbalanceamento (minoria/maioria).  

- **Implementação XGBoost Padrão** (`algorithmImplementation.ipynb`)  
  - Treino de árvores de decisão e modelo de gradient boosting.  
  - Plot de **learning curves**.  
  - Geração de relatório em CSV: `relatorio_sem_mod.csv` e respetiva versão com G‑mean: `relatorio_sem_mod_Gmean.csv`.  

- **XGBoost Modificado** (`algorithmImplementationMod.ipynb`)  
  - Seleção de Features por Mutual Information, através da métrica de *Mutual Information*
  - Log-Loss Ponderado
  - Calibração do Threshold com G-Mean
  - Geração de relatório em CSV: `relatorio_com_mod.csv`.  

- **Análise de Performance**  
  - Comparação lado a lado das duas variantes.   
  - Discussão sobre trade‑offs.  

---

## Tecnologias Utilizadas

- **Python 3.10.12**
  - numpy -> 2.2.3
  - pandas -> 2.2.3
  - scikit-learn -> 1.6.1
  - imbalanced-learn -> 0.13.0
  - matplotlib -> 3.10.0
  - seaborn -> 0.13.2
  - scipy -> 1.15.2
