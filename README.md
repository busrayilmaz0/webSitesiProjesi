<h1 align="center">🧠 Derin Öğrenme Tabanlı Beyin Tümörü Sınıflandırması</h1>

<p align="center">
  Bu proje, tıbbi teşhis süreçlerini hızlandırmak ve MRI görüntülerinden beyin tümörü türlerini yüksek doğrulukla tespit etmek amacıyla geliştirilmiştir.
</p>

<p align="center">
  Proje kapsamında popüler derin öğrenme mimarileri (VGG16, VGG19, AlexNet, SqueezeNet) kullanılarak kapsamlı bir performans analizi yapılmıştır.
</p>

<hr>

<h2>🚀 Projenin Amacı</h2>

<p>Tıbbi görüntüleme sistemlerinden alınan MRI sonuçlarını analiz ederek;</p>

<ul>
  <li><b>Hızlı Teşhis:</b> Uzmanların manuel inceleme yükünü azaltmak.</li>
  <li><b>Karşılaştırmalı Analiz:</b> Farklı CNN mimarilerinin tıbbi görüntü sınıflandırmadaki başarısını ölçmek.</li>
  <li><b>Detaylı Sınıflandırma:</b> Sadece tümör tespiti değil, tümör türünün (Menenjiom, Glioma, Hipofiz) belirlenmesi.</li>
</ul>

<hr>

<h2>📊 Veri Seti Bilgileri</h2>

<p>Projede kullanılan veri seti Kaggle üzerinden temin edilmiştir.</p>

<ul>
  <li><b>Toplam Veri:</b> 7200 adet insan beyni MRI görüntüsü.</li>
  <li><b>Sınıf Sayısı:</b> 4 Sınıf (3 Tümör Türü + 1 Sağlıklı).</li>
  <li><b>Veri Dağılımı:</b> Her bir sınıf için 1400 adet eğitim, 400 adet test görüntüsü ayrılmıştır.</li>
</ul>

<p><b>Sınıf Tanımları:</b></p>

<ul>
  <li><b>Menenjiom (Meningioma):</b> Beyin zarlarından kaynaklanan tümörler.</li>
  <li><b>Glioma:</b> Beyin ve omurilikteki destek hücrelerinden kaynaklanan hızlı büyüyen tümörler.</li>
  <li><b>Hipofiz Tümörü (Pituitary Tumor):</b> Hormon dengesini kontrol eden bezde oluşan tümörler.</li>
  <li><b>Sağlıklı Beyin:</b> Herhangi bir tümör bulgusu içermeyen görüntüler.</li>
</ul>

<p>
  Not: Veri seti görselleri boyut nedeniyle GitHub'a yüklenmemiştir. Veri setine buradan ulaşabilirsiniz: 
  <a href="https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset">Kaggle Veri Seti</a>.
</p>

<hr>

<h2>🧠 Kullanılan Derin Öğrenme Mimarileri</h2>

<p>Projede Transfer Learning (Transfer Öğrenme) yöntemiyle şu dört farklı model eğitilmiştir:</p>

<ul>
  <li><b>VGG16 & VGG19:</b> Derinlikleri sayesinde karmaşık özellikleri yakalamada oldukça başarılı olan klasik mimariler.</li>
  <li><b>AlexNet:</b> Derin öğrenmenin öncüsü, daha hızlı ancak güçlü bir mimari.</li>
  <li><b>SqueezeNet:</b> Özellikle düşük parametre sayısı ve hızıyla bilinen, mobil ve gömülü sistemlere uygun hafif model.</li>
</ul>

<hr>

<h2>📈 Eğitim Sonuçları ve Ekran Görüntüleri</h2>

<p>Model eğitimleri sonucunda elde edilen başarı oranları ve sonuç grafikleri aşağıda yer almaktadır:</p>

<p align="center">
  <img src="vgg19_sonuc1.png" alt="Eğitim Sonucu" width="800">
</p>

<p align="center"><i>Görsel 1: Model eğitim aşaması ve doğruluk (accuracy) grafikleri.</i></p>

<hr>

<h2>⚠️ Önemli Not</h2>

<p>
  Eğitilmiş modellerin ağırlıklarını içeren <code>.mat</code> dosyaları (örneğin <code>tumor_vgg19.mat</code>), 
  dosya boyutları GitHub limitlerini aştığı için bu depoya dahil edilmemiştir.
</p>

<p>
  Kodlar çalıştırıldığında model ilgili mimariyi indirip eğitimi başlatacak ve kendi <code>.mat</code> dosyanızı yerel olarak oluşturacaktır.
</p>

<hr>

<h2>🛠️ Teknolojiler</h2>

<ul>
  <li><b>Yazılım:</b> MATLAB</li>
  <li><b>Mimariler:</b> VGG16, VGG19, AlexNet, SqueezeNet</li>
  <li><b>Veri Kaynağı:</b> Kaggle</li>
</ul>
