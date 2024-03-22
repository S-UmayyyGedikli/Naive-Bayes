# Diabetes Veri Seti İçin Naive Bayes Modelleme ve Ön İşleme

## Giriş

Bu proje, diabetes veri seti üzerinde Naive Bayes algoritması kullanılarak modelleme ve farklı ön işleme adımlarının gerçekleştirilmesini içermektedir. Diabetes veri seti, çeşitli klinik ve demografik özellikleri içermektedir ve amacımız bu özellikleri kullanarak bireylerin şeker hastalığı riskini tahmin etmektir.

## Metot

1. **Veri Yükleme ve Ön İşleme**: İlk olarak, diabetes.csv dosyası pandas kütüphanesi ile yüklenir ve gerektiğinde veri ön işleme adımları uygulanır. Bu adımlar arasında eksik verilerin doldurulması, kategorik değişkenlerin dönüştürülmesi ve gereksiz sütunların düşürülmesi yer alabilir.

2. **Veri Setinin Bölünmesi**: Veri seti, eğitim ve test setlerine ayrılır. Bu adım, train_test_split fonksiyonu kullanılarak gerçekleştirilir. Tipik olarak, veri setinin %80'i eğitim için, %20'si ise test için ayrılır.

3. **Model Oluşturma**: Gaussian Naive Bayes algoritması kullanılarak bir model oluşturulur. Bu adımda, eğitim verileri modelle eğitilir ve test verileriyle modelin performansı değerlendirilir.

4. **Ön İşleme Adımlarının Değerlendirilmesi**: Min-Max normalizasyonu, özellik seçimi veya diğer ön işleme adımları uygulanabilir. Her bir adımın modelin performansına etkisi değerlendirilir.

5. **GridSearchCV ile Hiperparametre Ayarı**: GridSearchCV kullanılarak en iyi hiperparametreler belirlenir. Bu adım, modelin performansını artırmak için önemlidir ve overfittingi önlemeye yardımcı olabilir.

## Sonuçlar ve Yorumlar

- Orijinal Model Doğruluğu: %%%%
- Min-Max Normalizasyon Sonrası Model Doğruluğu: %%%%
- GridSearchCV Sonrası Model Doğruluğu: %%%%

Yukarıdaki sonuçlar, farklı ön işleme adımlarının ve modelleme tekniklerinin performansını karşılaştırmak için kullanılabilir. Özellikle, GridSearchCV kullanarak en iyi hiperparametreleri belirlemenin model performansını artırdığı gözlemlenmiştir.

## Çalıştırma Talimatları

Projeyi çalıştırmak için aşağıdaki adımları izleyin:

1. Gerekli kütüphaneleri yükleyin: `pip install numpy pandas scikit-learn`
2. Diabetes.csv veri setini indirin veya yükleyin.
3. Anaconda veya Jupyter Notebook gibi bir Python geliştirme ortamında kodu çalıştırın.

## Referanslar

- Veri seti kaynağı: [Diabetes Dataset](https://www.kaggle.com/uciml/pima-indians-diabetes-database)
- Naive Bayes Algoritması: [Scikit-learn Documentation](https://scikit-learn.org/stable/modules/naive_bayes.html)

