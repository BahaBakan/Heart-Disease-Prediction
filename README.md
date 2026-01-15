# CardioRisk AI: Makine Öğrenmesi ile Kalp Hastalığı Tahmini

Bu proje, bir bireyin yaşam tarzı ve sağlık verilerini analiz ederek kalp hastalığı riskini tahmin eden uçtan uca bir veri bilimi iş akışıdır. Proje; veri ön işlemeden özellik mühendisliğine, dengesiz veri yönetiminden (SMOTE) açıklanabilir yapay zekaya (SHAP) kadar modern ML tekniklerini içermektedir.

## 🌟 Öne Çıkan Özellikler

* **Dinamik Paket Yönetimi:** Gerekli kütüphaneleri (`xgboost`, `shap`, `imblearn` vb.) çalışma anında kontrol eden ve yükleyen otomatik kurulum betiği.
* **Gelişmiş Özellik Mühendisliği:** Sigara, diyabet ve genetik faktörleri birleştiren bir "Toplam Risk Skoru" algoritması geliştirilmiştir.
* **Dengesiz Veri Çözümü (SMOTE):** Veri setindeki sınıf dengesizliğini gidermek için sentetik veri üretimi tekniği kullanılmıştır.
* **Model Kıyaslama:** Lojistik Regresyon, Random Forest, SVM ve XGBoost modelleri GridSearchCV ile hiperparametre optimizasyonuna tabi tutulmuştur.
* **Açıklanabilir Yapay Zeka (SHAP):** Modelin verdiği kararların arkasındaki nedenleri gösteren SHAP analizi eklenmiştir.

## 🛠 Kullanılan Teknolojiler

* **Dil:** Python 3.x
* **Kütüphaneler:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn
* **Gelişmiş Araçlar:** SMOTE (imbalanced-learn), SHAP (TreeExplainer)

## 📊 İş Akışı (Workflow)

1. **Veri Analizi (EDA):** Veri setinin istatistiksel dağılımı ve hedef değişken analizi.
2. **Ön İşleme:** Eksik verilerin median ile doldurulması, kategorik değişkenlerin Label & Ordinal Encoding ile sayısallaştırılması.
3. **Özellik Seçimi:** Random Forest kullanılarak en etkili 5 özelliğin belirlenmesi.
4. **Model Eğitimi:** 4 farklı modelin eğitilmesi ve F1-Score, Recall, Accuracy metrikleri ile değerlendirilmesi.
5. **Eşik Optimizasyonu:** F1-Score'u maksimize etmek için dinamik olasılık eşiği (threshold) belirlenmesi.

## 🚀 Sonuçlar

XGBoost modeli, yapılan testlerde ve eşik optimizasyonu sonrasında kalp hastalıklarını tespit etmede en yüksek başarıyı göstermiştir. SHAP analizi sonuçlarına göre, bireyin risk skorunun ve yaş faktörünün model kararları üzerinde en baskın özellikler olduğu doğrulanmıştır.

## 📦 Kurulum ve Kullanım

1. Depoyu klonlayın:
   ```bash
   git clone [https://github.com/kullanici_adin/Heart-Disease-Prediction.git](https://github.com/kullanici_adin/Heart-Disease-Prediction.git)
