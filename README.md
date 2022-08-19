# Insertion-Sort-Projesi
## proje 1: [22,27,16,2,18,6] 

Insertion Sort  türüne göre bu dizi üzerinde bilgi pekiştirmesi yapalım.

1) Yukarıdaki dizinin insertion sort türüne göre aşamalarını yazalım.
---
```
1.ci aşama [22,27,16,2,18,6] -> n 
2.ci aşama [2|27,16,22,18,6] -> n-1
3.cü aşama [2,6,16,22,18,27] -> n-2
4.cü aşama [2,6|16,22,18,27] -> n-3
5.ci aşama [2,6,16|18,22,27] -> n-4
6.cı aşama [2,6,16,18|22,27] -> n-5
7.ci aşama [2,6,16,18,22|27] -> +1
```

2) Yukardaki dizinin Big-O 'suna bakalım.
---
Big-O neydi? Yapilan işlemlerin toplamı demektir.

yukarıda yazdığımız ilk aşamada tüm rakamları tek tek kontrol etmiştik bu toplam işlem sayısına "n" dedik.  
ikinci aşamada ise ilk bulduğumuz ve birinci sıraya sabitledigimiz 2 rakamının dışında kalanlar arasında en küçük rakamı aradığımız için buradaki işlem sayımızda n-1 olur.  
Bu işlem son rakam kalana kadar sırayla tekrarlanır. n+(n-1)+(n-2)..+1  
+1 nerden geldi derseniz en son sıradaki raKam tek başına kalmasından dolayı +1 yapıyoruz.

Yukardaki dizinde yaptığımız tüm işlemlerin toplam sayısını bulmak için n+(n-1)+(n-2)....+1  sonucunu bulmamız lazım.  
Bizim dizinde bunu hesaplamak kolaydır çünkü "n" sayımız (SIRALAMA YAPTIĞIMIZ RAKAM SAYISI) 6 dır.  
Ama çok büyük ve uzun sıralaması olan işlemlerin kolay hesaplanması icin bir formül vardır.  
n.(n+1)/2 yapılınca 1 den "n"e kadar olan sayıların toplamı bulunur. buda bize n^2+n/2 sonucunu verir.  
Big-O yu bulmada fonksiyonel değeri en büyük olan alınır.  
Dolaysiyla bizim işlemde yani (n^2+n/2) fonksiyonel olarak en büyük değere sahip n^2 olduğundan Big-O (n^2)dir.

### Big-O (n^2)

Time Complexity nin bölümlerini hatırlıyalım;

---
 Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması. 


Buna göre yukardaki dizin sıralandığında 18 sayısının  
Time Complexity si Average case olur.


Son olarak aşağıdaki dizini İnsertion Sort e göre ilk 4 aşamasını yazalım.  

[7,3,5,8,2,6,9,4,15,6]
```
*[7,3,5,8,2,6,9,4,15,6]
*[2|3,5,8,7,6,9,4,15,6]
*[2,3|5,8,7,6,9,4,15,6]
*[2,3,4|8,7,6,9,5,15,6]
```

[Patika.dev](https://www.patika.dev/tr)
