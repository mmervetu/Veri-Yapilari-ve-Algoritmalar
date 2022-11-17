# Proje 1 - Insertion Sort

**[22,27,16,2,18,6]** -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

1. Average case: Aradığımız sayının ortada olması
2. Worst case: Aradığımız sayının sonda olması
3. Best case: Aradığımız sayının dizinin en başında olması.

**[7,3,5,8,2,9,4,15,6**] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

---

## Cevap:
Bu algoritma, belirli bir anda array’in belirli bir kısmını sıralı tutarak ve bu kısmı her adımda biraz daha genişleterek çalışmaktadır.

1. Adım: [22,27,16,2,18,6] - 22 kendi başına sıralı olduğu için hiçbir işlem yapılmadan devam eder. 
2. Adım: [22,27,16,2,18,6] - 22 ve 27 verisi arasında karşılaştırma yapılır. 22 daha küçük olduğu için bir değişiklik yapılmaz. 
3. Adım: [16,22,27,2,18,6] - Veriyi bir adım daha genişletir; 16, 22 ve 27’den küçük olduğu için başa geçer.
4. Adım: [2,16,22,27,18,6] - Veriyi bir adım daha genişletir; 2, gerisindeki 16,22 ve 27’den küçük olduğu için başa geçer.
5. Adım: [2,16,18,22,27,6] - Veriyi bir adım daha genişletir; 18, 22 ve 27 ile kıyaslanır, küçük olduğu için yer değiştirir, ardından 16 ile karşılaştırılır, büyük olduğu için değişiklik yapılmaz.  
6. Adım: [2,6,16,18,22,27] - Veriyi bir adım daha genişletir; 6, gerisindeki 16, 18,22 ve 27 ile kıyaslanır, küçük olduğu için yer değiştirir, ardından 2 ile karşılaştırılır, büyük olduğu için değişiklik yapılmaz. 

Big O gösterimi = O(n²)

Time Complexity:

- **Worst Case:** Aradığımız sayının en sonda olan sayı olması durumudur. Örneğin: Sıralama olarak tam ters verilmiş bir dizinin olduğunu düşelim. Bu durumda dizindeki her bir eleman, gerisindekinden küçük olacaktır. Bu nedenle herbir eleman için geriye doğru hareket edilecektir.  1. eleman için 0 döngü,  2. eleman için 1, 3. eleman 2, sonra ise 3,4,5,… n kadar geriye hareket yapacaktır. Bunların toplamı ise: 0+1+2+3…+n = n.(n+1)/2’dir. n² dominant olduğu için worst case: O(n²)’dir.
- **Best Case:** Elimizde tam sıralı bir dizinini olması durumudur. Algoritma n sayılı dizinin üzerinden bir defa geçer ve hiçbirini değiştirmez. Dolayısıyla best case: 0(n)’dir.
- **Average Case:**  Çoğu algoritma en kötü durumla aynı ortalama duruma sahip olmaktadır. Zira her ne kadar istisnaları olsa da ortalama durumun, en kötü ve en iyi durumun ortalaması olduğu varsayıldığından ve ortalama alındığında da katsayıları önemsemediğimizden; ortalama durum, dominant olan en kötü durumla aynı olacaktır. Average case: O(n²)’dir.

Dizi sıralandıktan sonra 18 sayısı, dizide ortada kalacağından average case kapsamına girer. 
<br/><br/> 

**[7,3,5,8,2,9,4,15,6**] dizisinin Selection Sort'a göre ilk 4 adımı:

Bu algoritma dizinin ilk elemanının en küçük eleman olduğunu varsaymakta ve ardından tek tek bu elemanı diğer elemanlarla karşılaştırarak çalışmaktadır. 

1. Adım: [2,3,5,8,7,9,4,15,6] - 7 elemanı diğer elemanlarla kıyaslanır, 2 en küçük olduğu için 7 ile yer değiştirir ve başa geçer. İlk sıra tamamlanır. 
2. Adım: [2,3,5,8,7,9,4,15,6] - 2. sıradaki 3 elemanı kalan diğer elemanlarla kıyaslanır, en küçük olduğu için değişiklik olmaz. ilk iki sıra tamamlanmış olur. 
3. Adım: [2,3,4,8,7,9,5,15,6] -3. sıradaki 5 elemanı kalan diğer elemanlarla kıyaslanır, 4 en küçük olduğu için 5 ile yer değiştirir. İlk üç sıra tamamlanmış olur. 
4.  Adım: [2,3,4,5,7,9,8,15,6] -4. sıradaki 8 elemanı kalan diğer elemanlarla kıyaslanır, 5 en küçük olduğu için 8 ile yer değiştirir. İlk dört sıra tamamlanmış olur.
<br/><br/> 

Bu proje [Patika.dev](https://www.patika.dev/tr) eğitimi kapsamında yapılmıştır.