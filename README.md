# Diabetes Veri Seti İçin Naive Bayes Modelleme 

## Giriş

Bu proje, diabetes veri seti üzerinde Naive Bayes algoritması kullanılarak modelleme ve farklı işlem adımlarını gerçekleştirmekdir. Diabetes veri seti, hamilelik, şeker, kan basıncı, cilt kalınlığı, insülin, BMI, yaş ve soy ağacında bulunma özellklerini içerir. Amacımız bu özellikleri kullanarak bireylerin şeker hastalığı riskini tahmin etmektir.

## Metot

1. **Veri Yükleme ve Ön İşleme**: İlk olarak, diabetes.csv dosyası pandas kütüphanesi ile yüklenir ve gerektiğinde veri ön işleme adımları uygulanır. Bu adımlar arasında eksik verilerin doldurulması, kategorik değişkenlerin dönüştürülmesi ve gereksiz sütunların düşürülmesi yer alabilir. Bizim elimizdeki veri setinde eksik veri yoktur, ihityaca bağlı diğer işlemleri siz kendiniz yapabilirsiniz.

2. **Veri Setinin Bölünmesi**: Veri seti, eğitim ve test setlerine ayrılır. Bu adım, train_test_split fonksiyonu kullanılarak gerçekleştirilir. Genel olarak, veri setinin %80'i eğitim için, %20'si ise test için ayrılır.

3. **Model Oluşturma**: Gaussian Naive Bayes algoritması kullanılarak bir model oluşturulur. Bu adımda, eğitim verileri modelle eğitilir ve test verileriyle modelin performansı değerlendirilir.

4. **Ön İşleme Adımlarının Değerlendirilmesi**: Min-Max normalizasyonu, özellik seçimi veya diğer ön işleme adımları uygulanabilir. Her bir adımın modelin performansına etkisi değerlendirilir.

5. **GridSearch ile Hiperparametre Ayarı**: GridSearch kullanılarak en iyi hiperparametreler belirlenir. Bu adım, modelin performansını artırmak için önemlidir ve overfittingi önlemeye yardımcı olabilir.

6.  **En İyi Modelin Belirlenmesi**:En son yaptığımız şeydir. Veri setindeki özelliklere bakılarak bu özelliklerin kullanılması ve bir final modelin oluşturulması burada yaptığımız işlemdir. Bu, modelin performansını artırmak ve veri setindeki istenmeyen veya anlamsız bilgileri azaltmak için kullanılır.
## Sonuçlar ve Yorumlar

- Orijinal Model Doğruluğu: 0.7857142857142857
Confusion Matrix (Orijinal Model):
 [[87 18]
 [15 34]]
- Min-Max Normalizasyon Sonrası Model Doğruluğu: 0.7857142857142857
Confusion Matrix (Min-Max Normalizasyon Sonrası Model):
 [[87 18]
 [15 34]]
-  GridSearch Sonrası Model Doğruluğu: 0.7792207792207793
Confusion Matrix (GridSearch Sonrası Model):
 [[86 19]
 [15 34]]
- Özellik Seçimi Sonrası Model Doğruluğu: 0.7467532467532467
Confusion Matrix (Özellik Seçimi Sonrası Model):
 [[87 18]
 [21 28]]
Yukarıdaki sonuçlar, farklı ön işleme adımlarının ve modelleme tekniklerinin performansını karşılaştırmak için kullanılabilir. Özellikle, GridSearchCV kullanarak en iyi hiperparametreleri belirlemenin model performansını artırdığı gözlemlenmiştir.

## Çalıştırma Talimatları

Projeyi çalıştırmak için aşağıdaki adımları izleyin:

1. Gerekli kütüphaneleri yükleyin: `pip install numpy pandas scikit-learn`
2. Diabetes.csv veri setini indirin veya yükleyin.
3. Anaconda veya Jupyter Notebook gibi bir Python geliştirme ortamında kodu çalıştırın.

## Referanslar

- Veri seti : diabetes.csv 
- Naive Bayes Algoritması: [Scikit-learn Documentation](https://scikit-learn.org/stable/modules/naive_bayes.html)

