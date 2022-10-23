# Proje-2
### [16,21,11,8,12,22] -> Merge Sort

#### 1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
#### İlk olarak dizimizi ikiye bölüyoruz. Böldüğümüz dizileri tekrar bölüyoruz. Tek eleman kalana kadar bu işleme devam ediyoruz.

```mermaid
graph TD;
16,21,11,8,12,22;
16,21,11,8,12,22-->16,21,11;
16,21,11,8,12,22-->8,12,22;
16,21,11-->16,21;
16,21,11-->11_;
11_-->11;
16,21-->16;
16,21-->21;
8,12,22-->8_;
8_-->8;
8,12,22-->12,22;
12,22-->12;
12,22-->22;
```

Diziyi ikiye bölerek yeniden yazıyoruz => Sol ve sağdaki dizileri tekrar ikiye böluyoruz => Tek eleman kalana kadar bu işleme devam ediyoruz. 


####  Bölme işlemi bitikten sonra, tek elemanlı dizilerimizi ikili ikili birleştiriyoruz. Sıralı dizi elde edinceye kadar bu işleme devam ediyoruz.

```mermaid
graph TD;
16--> 16,21;
21-->16,21;
11_-->11;
8_-->8;
12_-->12,22;
22_-->12,22;
16,21-->11,16,21;
11-->11,16,21;
8-->8,12,22;
12,22-->8,12,22;
11,16,21-->8,11,12,16,21,22;
8,12,22-->8,11,12,16,21,22;
```

ikili ikili ikili sıralayarak birleştiriyoruz => Tekrar ikili ikili sıralayarak birleştiriyoruz => Son birleştirmede dizimizi elde ediyoruz.


#### 2. Big-O gösterimini yazınız.
Recursive bir fonksiyon olduğu için sürekli kendini çağırarak diziyi hep ikiye bölmektedir. Her bölünmüş dizinin Merge işlemi için de dizinin uzunluğu olan n işlem yapıldığından O(n*(logn)) --> O(6*(log6)) olacaktır.
