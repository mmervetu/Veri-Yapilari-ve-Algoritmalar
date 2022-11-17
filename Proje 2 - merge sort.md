# Proje 2 - Merge Sort

**[16,21,11,8,12,22]** -> Merge Sort

- Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
- Big-O gösterimini yazınız.

---
## Cevap:

Merge Sort’da listeyi bir anda sıralamak yerine; parçalara ayırıp sonra onu da kendi içerisinde en küçük parçalara kadar ayırıp, ardından kendi arlarında sıralayarak birleştirme işlemi yapılmakadır. 

Divide 1:                                     [16,21,11]  [8,12,22]

Divide 2:                              [16,21] - [11]       [8,12] - [22]

Divide 3:                         [16] - [21] - [11]         [8] - [12] - [22]

Merge 1:                               [16,21] - [11]      [8,12] - [22]

Merge 2:                                      [11,16,21]   [8,12,22]

Merge 3:                                        [8,11,12,16,21,22]
<br/><br/> 
Merge Sort’da herbir adımda elemanlı bazlı gittiğimiz ve her adımdaki eleman sayısı da aynı olduğu için adımların hepsi aynı time complexcity’ye sahiptir = O(n) 

Ayrıca her seferinde yarıya indiği için, 2^x  = n ise x= logn’dir.  İşlem, logn kez yapılmaktadır. 

Bu nedenle Big-0 = O(n*logn)’dir.
<br/><br/> 

Bu proje [Patika.dev](https://www.patika.dev/tr) eğitimi kapsamında yapılmıştır.