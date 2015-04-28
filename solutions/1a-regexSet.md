# 1a-regexSet
Adam Pearce  




### Load data from URL

```r
words <-read.table("http://benschmidt.org/words.txt")
```

### Words with 6 consective i or j

```r
subset(words, grepl("[il][il][il][il][il][il]", V1))
```

```
##                 V1
## 61665   milliliter
## 61666 milliliter's
## 61667  milliliters
```
