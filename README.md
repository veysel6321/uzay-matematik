[Yeşil bayrak tıklanınca]
değişken puan → 0
[sonsuz döngü]
  set soru → rastgele 1 ile 10
  set cevap → rastgele 1 ile 10
  set dogruCevap → soru * cevap  // ya da - (rastgele seçmek için ek blok eklenebilir)
  söyle (soru + " x " + cevap + " kaç eder?") 2 saniye
  [kullanıcıdan yanıt al]  // Scratch’te “cevap” girdisi
  eğer cevap = dogruCevap ise
    puan → puan + 1
    söyle ("Doğru! Puan: " + puan) 1 saniye
    [uzay gemisine "yıldız kazan" mesajı gönder]
  değilse
    söyle ("Yanlış! Doğru cevap: " + dogruCevap) 2 saniye["yıldız kazan" mesajını aldığında]
  bir yıldız klonu oluştur[Ben başladığımda gizlen]
[Klon başladığında]
  görün
  x → rastgele -200 ile 200, y → 150
  y'yi -150'ye kadar yavaşça indir
  sonra yok ol
