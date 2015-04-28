# 1a-regexSet
Adam Pearce  




##### Load data from URL

```r
words <-read.table("http://benschmidt.org/words.txt")
```

##### Words with 6 consective i or j

```r
subset(words, grepl("[il][il][il][il][il][il]", V1))
```

```
##                 V1
## 61665   milliliter
## 61666 milliliter's
## 61667  milliliters
```

##### Words that use all the vowels in alphabetical order

```r
subset(myData, grepl(".*a.*e.*i.*o.*u.*", V1))
```

```
## Error in subset(myData, grepl(".*a.*e.*i.*o.*u.*", V1)): object 'myData' not found
```

##### Replace `"NU"` and `"NEU"` with the word "Northeastern."

```r
gsub("NUE?", "Northeastern", "NU NEU NUE", perl=TRUE)
```

```
## [1] "Northeastern NEU Northeastern"
```

##### i before e, except after c

```r
gsub("cie", "cei", gsub("ei", "ie", "ei cei"))
```

```
## [1] "ie cei"
```


##### Remove duplicate spaces

```r
gsub(" +", " ", "a b  c     d e f   g", perl=TRUE)
```

```
## [1] "a b c d e f g"
```


##### Remove duplicate spaces

```r
gsub(" +", " ", "a b  c     d e f   g", perl=TRUE)
```

```
## [1] "a b c d e f g"
```


##### Remove duplicate spaces

```r
gsub(" +", " ", "a b  c     d e f   g", perl=TRUE)
```

```
## [1] "a b c d e f g"
```

