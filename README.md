# seaAnimals-deep-learning-project

## 🐟 Giriş

✿ Bu projede **görsel sınıflandırma** üzerine bir derin öğrenme çalışması gerçekleştirdim. 
✿ Kullandığım veri seti **sea-animals-image-dataste** (evet dataste yazmışlar :')) su altı canlılarından oluşuyor. Referans aldığım hazır veri setinde bulunan mercan ve balık sınıflarındaki görselleri, sayın tüplü dalış eğitmenim **Serhan İlhan**'ın su altı fotoğraflarından yine mercan ve balık görselleri ile aynı sınıflarda birleştirdim.
✿ Görselleri ön işleme adımlarıyla normalize edip **train, validation ve test setlerine** ayırdım.
✿ Modelleme aşamasında Transfer Learning yöntemlerinden VGG16 tabanlı bir yapı kullandım. Böylece önceden büyük veri setleri üzerinde eğitilmiş güçlü bir temel kullanarak modelimin daha hızlı ve daha başarılı bir şekilde öğrenmesini sağladım.
✿ Modelin son katmanlarını serbest bırakarak fine-tuning yaptım ve eklenen Dense + Dropout katmanları ile özelleştirilmiş sınıflandırma sağladım. ⊹₊⟡⋆ Çünkü modelimin kendi veri setime özgü ayrıntıları da öğrenebilmesini istiyordum. ⊹₊⟡⋆
✿ Ayrıca Keras Tuner kütüphanesi kullanarak en iyi hiperparametreleri (optimizer, dense units, dropout oranı) seçtim. Eğitim sürecinde EarlyStopping gibi callback mekanizmaları kullanarak modelin aşırı öğrenmesini engellemeye çalıştım.

## 🐟 Metrikler

✿ Modelin performansını eğitim sürecinde **accuracy** ve **loss** metrikleri üzerinden değerlendirdim.
✿ Eğitim ve doğrulama kayıplarındaki düşüş paralel ilerledi, ciddi bir overfitting görülmedi.
✿ Eğitim sonunda doğrulama doğruluğu yaklaşık %62–65 seviyelerine ulaştı.

Grafikler üzerinden yapılan analizde ise,

✿ Başlangıçta underfitting etkisi gözlendi, epoch ilerledikçe de doğruluk arttı.

✿ Validation loss’un düşük ve stabil kalması, modelin genelleme yeteneğinin güçlü olduğunu göstermektedir. ദ്ദി ˉ͈̀꒳ˉ͈́ )✧

  <img width="925" height="599" alt="image" src="https://github.com/user-attachments/assets/ecfabd04-1a43-47b9-8a87-e76967171d16" />

  <img width="925" height="627" alt="image" src="https://github.com/user-attachments/assets/17e40524-2df2-43b9-9806-f8c0acc87275" />

✿ Modelin hangi bölgelere dikkat ederek tahmin yaptığını görselleştirmek için heatmap görselleştirmeden yararlanarak GRAD CAM kullandım.

  <img width="458" height="571" alt="image" src="https://github.com/user-attachments/assets/9cc9460f-a0b6-4d6e-acf1-ce140b19381b" />



## 🐟 Ekler

✿ GPU hızlandırma kullanarak modelimin daha kısa sürede eğitilmesini sağladım.

## 🐟 Sonuç ve Gelecek Çalışmalar

Projem kapsamında temel bir görsel sınıflandırma modelini görece başarıyla uyguladım. Transfer learning sayesinde düşük epoch sayıları ile anlamlı doğruluk değerlerine ulaşabildim.

Gelecek çalışmalarım için planladığım adımlar şunlardır:

✿ Kesinlikle daha büyük ve çeşitlendirilmiş veri setleriyle modeli geliştirmek :')

✿ Modeli Streamlit veya Flask tabanlı bir arayüz ile deploy etmek.

✿ Gerçek zamanlı veri toplama ve canlı sınıflandırma özellikleri eklemek.


## 🐟 Lİnkler

https://www.kaggle.com/code/busraertekin/sea-animals-classification-project


𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟𓆝 𓆟 𓆞 𓆝 𓆟


Kaggle kitty sunar! İnceleme için teşekkürler ⸜(｡˃ ᵕ ˂)⸝♡
<img width="126" height="88" alt="image" src="https://github.com/user-attachments/assets/36c7817d-c020-4036-b439-f9cc0d199472" /> 















