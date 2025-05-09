# Öğrenci Başarısı ve Sosyal Faktörler Analizi

Bu proje, https://data.mendeley.com/datasets/5b82ytz489/1  veri setini kullanarak üniversite öğrencilerinin akademik başarısını (CGPA) etkileyen sosyal faktörleri (gelir, çalışma süresi, bilgisayar yetkinliği vb.)  analiz ettim

Öğrencilerin genel not ortalamaları ile çeşitli sosyal ve demografik özellikleri arasındaki ilişkileri, temel veri analizi teknikleriyle ortaya koymaya çalıştım.



## Metodoloji
1.  **Veri Yükleme ve Keşif:** Veri seti inceledim, sütunlar ve veri tipleri anladım.
2.  **Veri Ön İşleme:** Kategorik sosyal faktörler (örn: "Düşük Gelir") sayısal değerlere (örn: 0, 1) dönüştürdüm. Eksik verileri kontrol edip  varsa düzeltmeye çalıştım.
3.  **Analiz:** `groupby()` ile her sosyal faktörün farklı seviyelerindeki öğrencilerin ortalama başarıları (CGPA) hesapladım.
4.  **Yorumlama:** Sayısal sonuçlar üzerinden mantıksal çıkarımlar yapmaya çalıştım

##  Bu veri setine göre analiz sonucu
Öncelikle, devam oranının başarı üzerinde belirgin bir etkisi olduğu görülüyor. Özellikle %80-100 oranında derse devam eden öğrencilerin ortalama notu 3.58 iken, %40’ın altında devam edenlerde bu ortalama 1.78’e kadar düşüyor.

Oyun oynama süresi incelendiğinde ise çok büyük etki etmese de başarıyla ters orantısı var . Günde 0-1 saat oyun oynayan öğrencilerin ortalaması 3.62, 3 saatten fazla oyun oynayan öğrencilerde ise bu değer 3.00 seviyesindedir.

Cinsiyete göre başarı karşılaştırıldığında, kadın öğrencilerin ortalama notu 3.32, erkek öğrencilerin ortalaması ise 3.12 olarak hesaplanmıştır.

Yaşanılan yerin de başarı üzerinde kısmi bir etkisi olduğu söylenebilir. Şehirde yaşayan öğrencilerin ortalama başarı puanı 3.22, köyde yaşayanlarda ise 3.16 olarak bulunmuştur.

Son olarak, ekstra etkinliklere katılımın da akademik başarıyı olumlu yönde etkilediği görülmektedir. Etkinliklere katılan öğrencilerin ortalaması 3.40, katılmayanların ise 3.03’tür.


---
*Bu proje, temel veri analizi ve Pandas/NumPy becerilerini sergilemek amacıyla yapılmıştır.*
