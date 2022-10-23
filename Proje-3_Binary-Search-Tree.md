# Proje-3

[Patika.dev](https://www.patika.dev/tr)

### [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aşamalarını yazınız.
##### İkili arama ağacı, her düğümün solundaki koldan ulaşılabilecek bütün verilerin düğümün değerinden küçük, sağ kolundan ulaşılabilecek verilerin değerinin o düğümün değerinden büyük olmasını şart koşar.

|   Görsel  Açıklama    |
|--               |
```mermaid
graph TD;
7;
```

## **root=7**       



**5 sayısı 7'den küçük olduğunda 7'nin soluna ekledik.**
|   Görsel  Açıklama    |
|--           |
```mermaid
graph TD;
    7-->5*;
    7-->-;
```
## **5 ekledik**


**1 sayısı 5'ten ve 7'den küçük olduğunda 7 ve 5'in soluna ekledik.** 
|   Görsel  Açıklama    |
|--             |
```mermaid
graph TD;
    7-->5;
    7-->-;
    5-->1*;
    5-->*;
```

## **1 ekledik**

**8 sayısı 7'den büyük olduğunda 7'nin sağına ekledik.** 
|   Görsel  Açıklama    |
|--             |
```mermaid
graph TD;
    7-->5;
    7-->8*;
    5-->1;
    5-->*;
```
## **8 ekledik**


**3 sayısı  7'den ve 5'ten küçük  olduğunda 5'in soluna, 1'den büyük olduğunda 1'in sağına ekledik.**  
|   Görsel  Açıklama    |
|--             |
```mermaid
graph TD;
    7-->5;
    7-->8;
    5-->1;
    5-->*;
    1-->-;
    1-->3*;
```
## **3 ekledik**

**6 sayısı 7'den küçük  olduğunda 7'nin soluna, 5'ten büyük olduğunda 5'in sağına ekledik.**  
|   Görsel  Açıklama    |
|--             |
```mermaid
graph TD;
    7-->5;
    7-->8;
    5-->1;
    5-->6*;
    1-->-;
    1-->3;
```
## **6 ekledik**


**0 sayısı  7'den, 5'ten ve 1'den küçük  olduğunda 1'in soluna ekledik.**  
|   Görsel  Açıklama    |
|--              |
```mermaid
graph TD;
    7-->5;
    7-->8;
    5-->1;
    5-->6;
    1-->0*;
    1-->3;
```
## **0 ekledik**

**9 sayısı  7'den ve 8'den büyük olduğunda  8'in sağına ekledik.**  
|   Görsel  Açıklama    |
|--            |
```mermaid
graph TD;
    7-->5;
    7-->8;
    8-->9*;
    5-->1;
    5-->6;
    1-->0;
    1-->3; 
```
## **9 ekledik**



**4 sayısı  7'den ve 5'ten küçük olduğunda 5'in soluna, 1'den ve 3'ten büyük olduğunda 3'ün sağına ekledik.** 
|   Görsel  Açıklama    |
|--           |
```mermaid
graph TD;
    7-->5;
    7-->8; 
    8-->9;
    5-->1;
    5-->6;
    1-->0;
    1-->3;
    3-->-;
    3-->*4;
```
## **4 ekledik**

**2 sayısı  7'den ve 5'ten küçük olduğunda 5'in soluna, 1'den büyük olduğunda 1'in sağına ve 3'ten küçük olduğunda 3'ün soluna ekledik.** 
|   Görsel  Açıklama    |
|--           |
```mermaid
graph TD;
    7-->5;
    7-->8;  
    8-->9;
    5-->1;
    5-->6;
    1-->0;
    1-->3;
    3-->*2;
    3-->4;
```
## **2 ekledik**
