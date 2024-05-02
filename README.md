# Audio-Classification
Classification was performed by building CNN architecture with Tensorflow and Keras libraries. Finally, the CNN model was used to predict the class of an audio file.
## Dataset
  https://urbansounddataset.weebly.com/download-urbansound8k.html

## Classes
0=air_contitioner
1=car_horn
2=children_bark
3=dog_bark
4=drilling 
5=engine_idling 
6=gun_shot
7=jackhammer
8=siren
9=street_music


## Summary
Bu projede ilk olarak Librosa kütüphanesi yardımıyla MFC kullanılarak ses dosyaları işlenerek yapay zekanın anlayabileceği bir formata getirildi. librosa kütüphanesi kullanarak veri setimizdeki her ses sinyalinin özellikleri alındı  ve bunlar bir listede tutuldu . Daha sonra URBANSOUND8K isimli veri setindeki dosyalar önce rastgele bir şekilde train ve validation test set olarak ikiye ayırıldı. Tensorflow ve Keras kütüphaneleri ile CNN mimarisi inşa ederek sınıflandırma yapıldı. Son olarak CNN modeli  ile bir ses dosyası kullanılarak sınıfı tahmin edildi. Bu adımlar aşağıda anlatılmıştır.


## Step1 : Ses sinyal işleme ve uygun formata getirme. 
Python ile ses tanıma ve sınıflandırma yapabilmek için  ses dosyalarının derin öğrenme algoritmalarında kullanılabilir formatta olması gerekir .  
Projede ilk olarak bir örnek bir ses sinyalini librosa ile yükledik iki farklı ses kanalını  mono şeklinde okuttuk ve sesi dijital forma dönüştürüldü. Bu sinyal formu üzerinden ses dosyasının sinyal özelliklerini görmek amacıyla örnek olarak yapıldı.
 
## STEP 2: CNN modeli oluşturularak sınıflandırma 
 Yapay Sinir ağları derin öğrenme modellemesinde sıklıkla kullanılan ve genellikle veri analizi veya tahmin gibi görevlerde kullanılan bir tür makine öğrenme modelidir. Bu projede Modelin eğitimi  ve sınıflandırılması için Yapay sinir ağı modeli oluşturuldu. Model için 3 hidden layer kullanıldı. 

## STEP 3: CNN Modeli kullanılarak bir ses dosyasının sınıfını tahmin etme

Veri seti içinden bir ses verisi seçildi ve bu ses verisi için yukarıdaki işlemler tekrar edildi. Daha sonra verisetinde olmayan  farklı bir kaynaktan alınan polis siren sesini içeren bir ses dosyası indirildi . Ve test edildi
