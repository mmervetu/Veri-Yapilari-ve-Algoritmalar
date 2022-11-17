# Proje 3 - Binary Search Tree

**[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]** dizisinin Binary-Search-Tree aşamalarını yazınız.

**Örnek:** root x'dir. root'un sağından y bulunur. Solunda z bulunur vb.

---
## Cevap:
Binary Search Tree: 

```
	    7
      /  \
     5    8
    / \    \
   1   6    9
  / \
 0   3
    / \
   2   4
```

İlk aşamada root = 7 olarak belirlenir. İkinci aşamada 5, 7 den küçük olduğu için soluna yazılır. Üçüncü aşamada 1, 5'ten küçük olduğu için soluna yazılır. Dördüncü aşamada 8, 7'den büyük olduğu için sağına yazılır. Beşinci aşamada 3, 1'den büyük olduğu için sağına yazılır. Altıncı aşamada 6, 5'ten büyük olduğu için sağına yazılır. Yedinci aşamada 0, 1'den küçük olduğu için soluna yazılır. Sekizinci aşamada 9, 8'den büyük olduğu için sağına yazılır. Dokuzuncu aşamada 4, 3'ten büyük olduğu için sağına yazılır. Onuncu aşamada 2, 3'ten küçük olduğu için soluna yazılır.
<br/><br/> 

Bu proje [Patika.dev](https://www.patika.dev/tr) eğitimi kapsamında yapılmıştır.