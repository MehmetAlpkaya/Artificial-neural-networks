# Artificial-neural-networks
Yapay sinir ağları, insan beyninin bilgi işleme tekniğinden esinlenerek geliştirilmiş bir bilgi işlem 
teknolojisidir. YSA ile basit biyolojik sinir sisteminin çalışma şekli taklit edilir. Yani biyolojik nöron 
hücrelerinin ve bu hücrelerin birbirleri ile arasında kurduğu sinaptik bağın dijital olarak 
modellenmesidir.
1: Girişler 1. katmanda ağırlıklarla elde edilen bir ara cevaplara sahiptir(Z1).
2. Daha sonra elde edilen bu ara cevaplar bir sigmoid fonksiyonundan geçirilerek 2. katman 
cevabına dönüştürülür.
3. Tekrar bir sigmoid fonksiyonundan geçirilip tahmin sonucunu ortaya çıkarıyor.
4. Daha sonra tahmin ile gerçek cevaplar kıyaslanarak ağırlıklar değiştirilip tekrar bir tahmin 
denemesi yapılır.
Çözümde 2 katman kulanıldı
Z11=X1 * W11 + X2 * W21 + B1
Z21=X1 * W12 + X2 * W22 + B1
1.Katman Sigmoid fonksiyonlarının uygulanması:
A11 = 1/(1-exp(-Z11))
A21 = 1/(1-exp(-Z21))
Z2=A11 * W3 + A21 * W4 + B2
2. Katman Sigmoid fonksiyonlarının uygulanması:
A2=1/(1-exp(-Z2)) #Tahmin değerimiz
Loss Function:
Kayıp veya hata fonksiyonumuz tahmin ettiğimiz değerin gerçek değerinden ne kadar 
uzakta olduğumuzu anlamamıza yardımcı olacak bir çeşit ters transfer fonksiyonudur
Backpropagation:
Backpropagation’lar öncelikli olarak rastgele seçtiğimiz W ağırlıklarının güncellenmesi 
için kullanılan fonksiyonlardır.
