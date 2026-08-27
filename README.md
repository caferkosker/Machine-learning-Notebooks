Makine öğrenmesi çalışırken sıfırdan yazdığım Jupyter Notebook'ları. Her notebook tek bir konuya odaklanıyor: veriyi keşfetme, ön işleme, modeli kurma, hiperparametre optimizasyonu ve sonuçları değerlendirme adımlarını baştan sona içeriyor. Basit doğrusal regresyondan başlayıp SVM ve Naive Bayes'e kadar ilerliyor.

## İçerik

### Regresyon

| # | Notebook | Konu | Veri seti |
|---|---|---|---|
| 1 | `1-SimpleLinearRegression.ipynb` | Basit doğrusal regresyon | `1-studyhours.csv` |
| 2 | `2-MultipleLinearRegression.ipynb` | Çoklu doğrusal regresyon | `2-multiplegradesdataset.csv` |
| 3 | `3-PolynomialRegression.ipynb` | Polinom regresyon | `3-customersatisfaction.csv`, `3-newdatas.csv` |
| 4 | `4-RidgeLassoElasticNet.ipynb` | Düzenlileştirme: Ridge, Lasso, ElasticNet | `4-Algerian_forest_fires_dataset.csv` |
| 5 | `5-RegressionDecision.ipynb` | Regresyon modeli seçimi ve karşılaştırma | — |
| 6 | `6-RegressionAnalysisProject.ipynb` | Uçtan uca regresyon projesi | `diamonds.csv`, `weatherHistory.csv` |

### Sınıflandırma

| # | Notebook | Konu | Veri seti |
|---|---|---|---|
| 7 | `7-LogisticRegression.ipynb` | Lojistik regresyon | `7-cyber_attack_data.csv` |
| 8 | `8-MultipleLogicalRegression.ipynb` | Çok değişkenli lojistik regresyon | `8-fraud_detection.csv`, `6-bank_customers.csv` |
| 9 | `9-LogisticRegressionAdvanced.ipynb` | GridSearchCV, StratifiedKFold, ileri değerlendirme | `9-loan_risk_svm.csv`, `9-email_classification_svm.csv` |
| 10 | `10-SVMClassifier.ipynb` | Destek Vektör Makineleri – sınıflandırma, kernel'lar | `9-seismic_activity_svm.csv` |
| 10 | `10-SVMRegressor.ipynb` | Destek Vektör Makineleri – regresyon (SVR) | — |
| 11 | `11-NaiveBayesClassifier.ipynb` | Gaussian Naive Bayes; SVC ve Lojistik Regresyon ile karşılaştırma | `Iris.csv` |

## Kullanılan kütüphaneler

- **pandas**, **numpy** — veri işleme
- **matplotlib**, **seaborn** — görselleştirme
- **scikit-learn** — modelleme, ön işleme, model seçimi

## Öne çıkan konular

- Keşifsel veri analizi (`pairplot`, `scatterplot`, korelasyon incelemeleri)
- `LabelEncoder` ve `StandardScaler` ile ön işleme
- `train_test_split` ile eğitim/test ayrımı
- `GridSearchCV` ve `RandomizedSearchCV` ile hiperparametre optimizasyonu
- `StratifiedKFold` ile çapraz doğrulama
- Confusion matrix, classification report ve accuracy ile değerlendirme

## Kurulum

```bash
git clone https://github.com/caferkosker/Machine-learning-Notebooks.git
cd Machine-learning-Notebooks

python3 -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate

pip install numpy pandas matplotlib seaborn scikit-learn jupyter
jupyter notebook
```

Notebook'lar veri setlerini aynı klasörden okuduğu için (`pd.read_csv("Iris.csv")`), dosya yapısını değiştirmeden çalıştırman yeterli.

## Notlar

Bu repo bir öğrenme günlüğü niteliğinde; notebook'lar numaralandırılmış sırayla ilerliyor ve her biri bir öncekinin üzerine konu ekliyor.
