# seaAnimals-deep-learning-project

## 🐟 Giriş

* Bu projede **görsel sınıflandırma** üzerine bir derin öğrenme çalışması gerçekleştirdim.  
* Kullandığım veri seti su altı canlılarından oluşuyor. Referans aldığım hazır veri seti ile sayın tüplü dalış eğitmenim **Serhan İlhan**'ın su altı fotoğraflarını birleştirdim. 
* Görselleri ön işleme adımlarıyla normalize edip **train, validation ve test setlerine** ayırdım.
* Modelleme aşamasında Transfer Learning yöntemlerinden VGG16 tabanlı bir yapı kullandım. Böylece önceden büyük veri setleri üzerinde eğitilmiş güçlü bir temel kullanarak modelimin daha hızlı ve daha başarılı bir şekilde öğrenmesini sağladım.
* Modelin son katmanlarını serbest bırakarak fine-tuning yaptım ve eklenen Dense + Dropout katmanları ile özelleştirilmiş sınıflandırma sağladım. ⊹₊⟡⋆ Çünkü kendi veri setime özgü ayrıntıları da öğrenebilmesine istiyordum. ⊹₊⟡⋆

##
