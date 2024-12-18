# Plant Classification with CNN, VGG19, and DenseNet121

Bu repo, bitki sınıflandırması yapmak için derin öğrenme modelleri olan CNN, VGG19 ve DenseNet121 kullanarak yapılan çalışmaları içermektedir. Amacımız, bitki türlerini tanımak için bu üç farklı modelin performansını karşılaştırmaktır. Eğitim ve test verileri, çeşitli bitki türlerini içeren görüntülerle yapılmıştır.

## Kullanılan Modeller
1. **CNN (Convolutional Neural Network):** Kendi oluşturduğumuz basit bir CNN modeli kullanılmıştır.
2. **VGG19:** Klasik derin öğrenme modelidir, genellikle görüntü tanıma için güçlüdür.
3. **DenseNet121:** Derin öğrenme modelinin DenseNet121 versiyonu kullanılarak derinlemesine bir özellik çıkarımı yapılmıştır.

## Veri Kümesi
Veri kümesi, çeşitli bitki türlerine ait 10 sınıftan oluşan görüntüler içermektedir. Her model, eğitim, doğrulama ve test setleri üzerinde eğitilmiş ve test edilmiştir.

## Kullanılan Kütüphaneler
- TensorFlow (Keras)
- Matplotlib
- Seaborn
- Scikit-learn
- NumPy
- Pandas

## Adımlar

1. **Veri Hazırlığı:** 
   - Eğitim, doğrulama ve test veri setlerinin oluşturulması.
   - Görüntülerin yeniden boyutlandırılması ve normalizasyonu.
   
2. **Model Oluşumu:** 
   - Kendi CNN modelimizi oluşturduk.
   - VGG19 ve DenseNet121 önceden eğitilmiş modeller olarak kullanıldı.

3. **Model Eğitimi:** 
   - Eğitim sürecinde erken durdurma (EarlyStopping) kullanıldı.
   - Her model için eğitim süreci ve doğrulama kayıpları ile doğrulukları izlendi.

4. **Model Değerlendirmesi:** 
   - Test verisi üzerinde modellerin doğrulukları ölçüldü.
   - Sınıflandırma raporları ve karmaşıklık matrisleri (Confusion Matrix) oluşturuldu.

5. **Sonuçlar:** 
   - Test doğrulukları karşılaştırıldı.
   - Her modelin performansı görselleştirildi.

## Model Performansı
| Model      | Test Doğruluğu |
|------------|----------------|
| CNN        | 76.24%         |
| VGG19      | 76.73%         |
| DenseNet121| 93.07%         |
