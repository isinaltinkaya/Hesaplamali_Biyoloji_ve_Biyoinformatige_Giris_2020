# Hesaplamalı Biyoloji ve Biyoinformatiğe Giriş 
# Ders Notu

## Terminoloji

<b>String (karakter dizileri):</b> Sabit veya değişken olabilen bir veya daha fazla karakterden (harfler, sayılar, simgeler) oluşan bir dizidir.

`>>> s1 = ”string”`

`>>> s2=“123”`

`>>> s3 =“hesaplamalı biyoloji”`

`print(s1,s2,s3)`

> string 123 hesaplamalı biyoloji 

<b>Değişken:</b> Değerleri depolamak için ayrılmış bellek konumlarıdır.

`>>> var =30`

`>>> print(var)`

>`30`

`>>> var = "şimdi de değişken bir karakter dizisi olsun"`

`>>> print(var)`

>`şimdi de değişken bir karakter dizisi olsun`


<b>Fonksiyon:</b> Girdi alan, belirli hesaplamalar yapan ve çıktı üreten bir ifade kümesidir.

```
def ekrana_yaz( str ):
   print(str)
   return
```

`ekrana_yaz("Merhaba")`
> Merhaba

Kısa bir DNA dizisini my_dna değişkeni içerisinde saklayalım:

`>>> my_dna = "ATGCGTA"`

Şimdi DNA dizisini yazdıralım

`>>> print(my_dna)`

>`ATGCGTA`

Değişken ismi tamamen keyfidir. İstediğiniz herhangi bir ismi verebilirsiniz.

`>>> jon_snow= “ATGCGTA”`

`>>> print(jon_snow)`

>`ATGCGTA`

### DNA dizisi ile bir örnek:

`>>> s = "GATTACA"`

`>>> s[1:3]`

>`'AT'`

`>>> s[:3]`

>`'GAT'`

`>>> s[4:]`

>`'ACA'`

`>>> s[3:5]`

>`'TA'`

`>>> s[:]`

>`'GATTACA'`

`>>> s[-3:-1]`

>`'AC'`

### Protein sekansı ile bir örnek:

`>>> protein = "vlspadktnv"`

3’ten 5’ e kadar olan pozisyonları yazdıralım:

`>>> print(protein[3:5])`

>`pa`

 <b> Dikkat! </b> Pozisyonlar 0 dan itibaren başlar ve başlangıçta kapsayıcı bitişte hariç bırakıcıdır.
 
`>>> print(protein[0:6])`

>`vlspad`

<b> Dikkat! </b> ! Değişken isimleri BÜYÜK - küçük harfe duyarlıdır. Yani; 

`my_dna`

`MY_DNA`

`My_DNA`

`My_Dna`

farklı değişkenlerdir.

### Stringleri birleştirme

`>>> my_dna = "AATT" + "GGCC"`

`>>> print(my_dna)`

>`AATTGGCC`

Bu örnekte iki string birleştirilmiştir, ancak stringleri işaret eden değişkenler de birleştirilebilir.

`>>> upstream = "AAA"`

`>>> my_dna = upstream + "ATGC"`

`>>> print(my_dna)`

>`AAAATGC`

### len() fonksiyonu:

`>>> len("GATTACA")`

>`7`

### Birkaç örnek:

`>>> "GAT" + "TACA"`

>`'GATTACA'`

`>>> "A" * 10`

>`'AAAAAAAAAA'`

`>>> "G" in "GATTACA"`

>`True`

`>>> "GAT" in "GATTACA"`

>`True`

`>>> "AGT" in "GATTACA"`

>`False`

`>>> "GATTACA".find("ATT")`

>`1`

`>>> "GATTACA".count("T")`

>`2`

### Büyük-küçük harf değiştirme: lower()  ve upper() fonksiyonları

`>>> my_dna = "ATGC"`

`>>> print(my_dna.lower())`

>`atcg`

Ya da 

`>>> my_dna = "atgc"`

`>>> print(my_dna.upper())`

>`ATGC`

### Yenisiyle değiştirme: replace fonksiyonu

`>>> protein = "vlspadktnv"`

Şimdi valin’i (v) tirozinle (y) değiştirelim
 
`>>> print(protein.replace("v", "y"))`

>`ylspadktny`

Burada birden fazla karakteri de değiştirebilirz.

`>>> print(protein.replace("vls", "ymt"))`

>`ymtpadktnv`

### substring’leri sayma ve bulma

`>>> protein = "vlspadktnv"`

Burada istediğimiz bir amino asidi saydırabiliriz.

`>>> valine_count=protein.count(‘v’)`

`>>> print(valine_count)`

>`2`

`>>> lsp_count = protein.count('lsp')`

`>>> print(lsp_count)`

>`1`

`>>> tryptophan_count = protein.count('w')`

`>>> print(tryptophan_count)`

>`0`

### Dosyadan metinleri okuma: open ve read fonksiyonları

`>>> my_file = open("dna.txt")`

`>>> file_contents=my_file.read()`

`>>> print(file_contents)`

1  	`>>> my_file_name = "dna.txt"`

2 		`>>> my_file = open(my_file_name)`

3 		`>>> my_file_contents = my_file.read()`

>`ACTGTACGTGCACTGATC`

1. satırda dna.txt stringi my_file_name değişkeni içerisinde saklanıyor.

2. satırda my_file_name değişkenini open fonksiyonu için bir argüman olarak kullanıyor ve sonucu my_file değişkeni içerisinde saklıyoruz.

3. satırda my_file değişkenindeki read metodunu çağırıyoruz ve elde edilen stringi my_file_contents değişkeninde saklıyoruz.
