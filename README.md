# ds-fraud-analysis-detection
Notebook único contendo análise exploratória, feature engineering, modelagem e explicabilidade de um classificador binário para detecção de fraudes em transações de cartão de crédito.

Veja artigo completo em: https://medium.com/@pedrocnf/detec%C3%A7%C3%A3o-de-fraudes-em-transa%C3%A7%C3%B5es-financeiras-com-cart%C3%A3o-de-cr%C3%A9dito-da169b9303bf

🧠 Tecnologias

Python 3.10+

pandas, numpy, scikit-learn

matplotlib, seaborn, shap

joblib, pyarrow

⚙️ Estrutura

fraud-detector/

├─ data/ # dados (não versionar)

├─ models/             # modelo treinado (.pkl)

├─ notebooks/

│   └─ analise_modelagem_fraude.ipynb

├─ requirements.txt

└─ README.md

🚀 Como usar
python -m venv venv

source venv/bin/activate  # (Windows: venv\Scripts\activate)

pip install -r requirements.txt

jupyter lab  # ou jupyter notebook


Abra o notebook em notebooks/analise_modelagem_fraude.ipynb e execute as células.

📊 Resultados

AUC-ROC: ~0.987

Recall (fraude): ~0.90

Principais variáveis: amt, periodo_dia, category_shopping_net

🧩 Observações

Os dados não devem ser versionados por questões de privacidade.

O modelo final é salvo em models/model_rf.pkl.

Este projeto é puramente acadêmico e demonstra a importância da engenharia de atributos no combate à fraude.
