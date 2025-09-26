# seaAnimals-deep-learning-project

## 🐟 Giriş

* Bu projede **görsel sınıflandırma** üzerine bir derin öğrenme çalışması gerçekleştirdim. 
* Kullandığım veri seti **sea-animals-image-dataste** (evet dataste yazmışlar :')) su altı canlılarından oluşuyor. Referans aldığım hazır veri setinde bulunan mercan ve balık sınıflarındaki görselleri, sayın tüplü dalış eğitmenim **Serhan İlhan**'ın su altı fotoğraflarından yine mercan ve balık görselleri ile aynı sınıflarda birleştirdim.
* Görselleri ön işleme adımlarıyla normalize edip **train, validation ve test setlerine** ayırdım.
* Modelleme aşamasında Transfer Learning yöntemlerinden VGG16 tabanlı bir yapı kullandım. Böylece önceden büyük veri setleri üzerinde eğitilmiş güçlü bir temel kullanarak modelimin daha hızlı ve daha başarılı bir şekilde öğrenmesini sağladım.
* Modelin son katmanlarını serbest bırakarak fine-tuning yaptım ve eklenen Dense + Dropout katmanları ile özelleştirilmiş sınıflandırma sağladım. ⊹₊⟡⋆ Çünkü modelimin kendi veri setime özgü ayrıntıları da öğrenebilmesini istiyordum. ⊹₊⟡⋆
* Ayrıca Keras Tuner kütüphanesi kullanarak en iyi hiperparametreleri (optimizer, dense units, dropout oranı) seçtim. Eğitim sürecinde EarlyStopping gibi callback mekanizmaları kullanarak modelin aşırı öğrenmesini engellemeye çalıştım.

## 🐟 Metrikler

* Modelin performansını eğitim sürecinde **accuracy** ve **loss** metrikleri üzerinden değerlendirdim.
* Eğitim ve doğrulama kayıplarındaki düşüş paralel ilerledi, ciddi bir overfitting görülmedi.
* Eğitim sonunda doğrulama doğruluğu yaklaşık %62–65 seviyelerine ulaştı.

Grafikler üzerinden yapılan analizde ise,

* Başlangıçta underfitting etkisi gözlendi, epoch ilerledikçe de doğruluk arttı.

* Validation loss’un düşük ve stabil kalması, modelin genelleme yeteneğinin güçlü olduğunu göstermektedir. ദ്ദി ˉ͈̀꒳ˉ͈́ )✧

  <img width="1001" height="605" alt="image" src="https://github.com/user-attachments/assets/2773a7a5-af48-4b7a-aa78-6bd358a11e5d" />
  <img width="956" height="634" alt="image" src="https://github.com/user-attachments/assets/df0ed4d1-059e-47f4-ab61-e2a351f04c0a" />

## 🐟 Ekler

* GPU hızlandırma kullanarak modelin daha kısa sürede eğitilmesi sağladım.



