
# Hesaplamalı Biyoloji ve Biyoinformatiğe Giriş
# Uygulamalar

## Problem 6 - Bonus Soru

Pictures/RNA_kodon_tablosu.png

Splicing out introns, part one


Here's a short section of genomic DNA:
ATCGATCGATCGATCGACTGACTAGTCATAGCTATGCATGTAGCTACTCGATCGATCGA
TCGATCGATCGATCGATCGATCGATCATGCTATCATCGATCGATATCGATGCATCGACT
ACTAT
It comprises two exons and an intron. The first exon runs from the start of the
sequence to the sixty-third character, and the second exon runs from the ninety-
first character to the end of the sequence. Write a program that will print just the
coding regions of the DNA sequence.


Splicing out introns, part two


Using the data from part one, write a program that will calculate what percentage
of the DNA sequence is coding.



#### Örnek Verilen:


Örnek veri:

> AGCTTTTCATTCTGACTGCAACGGGCAATATGTCTCTGTGTGGATTAAAAAAAGAGTGTCTGATAGCAGC

#### Örnek İstenen:


Örnek çıktı:

>

### Problem 6 İçin Veri:

Komplementer DNA
ACTGATCGATTACGTATAGTATTTGCTATCATACATATATATCGATGCGTTCAT


Problem

The 20 commonly occurring amino acids are abbreviated by using 20 letters from the English alphabet (all letters except for B, J, O, U, X, and Z). Protein strings are constructed from these 20 symbols. Henceforth, the term genetic string will incorporate protein strings along with DNA strings and RNA strings.

The RNA codon table dictates the details regarding the encoding of specific codons into the amino acid alphabet.

Given: An RNA string s

corresponding to a strand of mRNA (of length at most 10 kbp).

Return: The protein string encoded by s

.
Sample Dataset

AUGGCCAUGGCGCCCAGAACUGAGAUCAAUAGUACCCGUAUUAACGGGUGA

Sample Output

MAMAPRTEINSTRING
