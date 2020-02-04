# Hesaplamalı Biyoloki ve Biyoinformatiğe Giriş

# Uygulamalar

## Problem 1

#### Örnek Verilen:

'dizi1' isimli bir DNA dizisi.

Örnek veri:

> AGCTTTTCATTCTGACTGCAACGGGCAATATGTCTCTGTGTGGATTAAAAAAAGAGTGTCTGATAGCAGC

#### Örnek İstenen:

4 adet sayı: `dizi1` içerisindeki sırasıyla 'A', 'C', 'G' ve 'T' nükleotitlerinin görülme sıklığı değerleri.

Örneğin; A sayısı/Toplam nükleotit sayısı

Örnek çıktı:

> A 0.2857142857142857

> C 0.17142857142857143

> G 0.24285714285714285

> T 0.3

### Problem 1 İçin Veri:

`dizi1 = "AGCTTTTCATTCTGAAGCTTTTCATTCTGAAGCCATTCTGAAGCATTCTGAAGCTTTTCATTCTGAAGCTTTCATTCTGACATTCTGTTCTGAGAAAAAGACATCATTCTGCATTCTGGGGAAAAGCTTTTCATTCTGAAGCTTTTCATTCTGAAGGCCATTCTGAAGCATTCTGCCATTCTGAAGCATTCTCATAGAACCCCTTCTCATAGAACCCCCGACATCCGACATCTGTTCTGAGAAAAAGACATCATTCCTGTTCTGAGAAAAAGACATCATTCCTGTTCTGAGAAACCAAGACATCATTCGAAGCATTCTGAAGCTTTTCATTCTGAAGCTTTCATTCTGACATTCTGTTCTGAGAAAAAGACATCATTCTGCATTCTGGGGAAAAGCTTTTCATTCTGAAGCTTTTCATTCTGAAGGCCATTCTGAACAAAAGACATCATT"`

`dizi1` içerisindeki sırasıyla 'A', 'C', 'G' ve 'T' nükleotitlerinin görülme sıklığı değerlerini hesaplayınız.



## Problem 2

% GC içeriği, bir DNA dizisi içerisinde bulunan 'G' ve 'C' nükleotitlerinin toplam sayısının, tüm nükleotitlerin sayısına oranıdır. 

Matematiksel olarak, ((G+C)/(A+T+G+C))\*100 şeklinde hesaplanır.

<b> GC içeriği neden önemlidir? </b> 

Gen dizilerinde ve genomlarda, çoğu ökaryot organizmanın GC içeriğinin yaklaşık %50 olduğu gösterilmiştir. Çoğu prokaryot organizmanın GC içeriğinin ise %50'den anlamlı bir şekilde yüksek olduğu gözlenmiştir. Bu nedenle, GC içeriği prokaryot ve ökaryot gen dizilerini hızlıca ayırt etmek için kullanılabilir.

Bir DNA dizisinin GC içeriğinin yüksek olması, diğer dizilere oranla daha yüksek bir erime sıcaklığı olduğunu gösterir. Bu da, moleküler biyoloji laboratuvar çalışmalarında önem kazanır.

#### Örnek Verilen:

'dizi2' isimli bir DNA dizisi.

Örnek veri:

> AGCTTTTCATTCTGACTGCAACGGGCAATATGTCTCTGTGTGGATTAAAAAAAGAGTGTCTGATAGCAGC

#### Örnek İstenen:

3 adet sayı: `dizi2` içerisindeki yüzde 'AT' içeriği değeri, `dizi2` içerisindeki yüzde 'GC' içeriği değeri ve bulunan bu ilk iki değerin toplamı.

Örnek çıktı:

> AT 58.57142857142858

> GC 41.42857142857143

> Toplam 100.0

### Problem 2 İçin Veri:

GenBank ID'si <b> MG944891.1 </b> olan DNA dizisini <b> NCBI veritabanı </b> üzerinden bulup, <b> FASTA </b> formatındaki verisine ulaşınız. 

Veriden kopyaladığınız DNA dizisini <b> Noccaea_papillosa </b> isimli bir değişkene atayınız.

Bu DNA dizisinin yüzde AT içeriğini, yüzde GC içeriğini ve bu iki değerin toplamını hesaplayınız.
