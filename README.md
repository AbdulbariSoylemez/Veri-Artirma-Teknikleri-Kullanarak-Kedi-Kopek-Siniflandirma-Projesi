# Kedi ve Köpek Sınıflandırma Projesi

Bu proje, keras kütüphanesi kullanılarak geliştirilmiş bir derin öğrenme modelini içermektedir. Model, görüntülerdeki kedi ve köpekleri sınıflandırmak üzere eğitilmiştir. Modelin başarı seviyesini artırmak amacıyla, eğitim sürecinde veri artırma teknikleri başarıyla kullanılmıştır. Bu teknikler, rotasyon, kaydırma, şekillendirme, yakınlaştırma ve çevirme gibi işlemleri içermektedir.

## Model Detayları

Projede kullanılan model, evrişimli sinir ağı (CNN) mimarisini temel alır. Modelin temel katmanları şunlardır:

- **Evrişim Katmanları:** Giriş görüntüler üzerinde evrişim işlemlerini gerçekleştirir ve özellikleri çıkarır.
- **Maksimum Havuzlama Katmanları:** Evrişim sonuçları üzerinde maksimum havuzlama işlemi uygular ve özellik haritalarını özetler.
- **Tam Bağlantılı Gizli Katman:** Önceki katmanlardan gelen özellikleri kullanarak karmaşık ilişkileri öğrenir.
- **Çıkış Katmanı:** İkili sınıflandırma için sigmoid aktivasyon fonksiyonu ile bir nöron içerir.

Model, aşırı öğrenmeyi önlemek ve genelleme yeteneğini artırmak için dropout ve veri artırma tekniklerini içermektedir.

## Veri Seti

Proje, "kat_dog" adlı bir veri seti üzerinde eğitilmiştir. Bu veri seti, kedi ve köpek görüntülerini içermektedir ve eğitim ile doğrulama için uygun bir şekilde ayrılmıştır.

## Veri Artırma

Eğitim sırasında kullanılan veri artırma teknikleri, rotasyon, kaydırma, şekillendirme, yakınlaştırma ve çevirme gibi işlemleri içermektedir. Bu teknikler, modelin farklı açılardan ve durumlardan öğrenmesini sağlayarak başarıyı artırmaktadır.

## Modelin Eğitimi

Model, eğitim ve doğrulama veri setleri üzerinde 20 epoch boyunca eğitilmiştir. Daha sonra, veri artırma teknikleri eklenerek model 50 epoch daha eğitilmiştir.

## Sonuçlar

Eğitim sürecinin kayıp (loss) ve doğruluk (accuracy) değerleri, grafiklerle görselleştirilmiştir. Ayrıca, modelin bir test görüntüsü üzerindeki başarısı örneklenmiştir. Veri setindeki çeşitliliği artırmak amacıyla uygulanan veri artırma teknikleri, modelin genelleme yeteneğini artırmış ve daha güvenilir sonuçlar elde edilmiştir.
