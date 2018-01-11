---
title: "ggplot2 Practice"
author: "Jewel Ocampo"
date: "January 10, 2018"
output: 
  html_document: 
    keep_md: yes
---






```r
mpg
```

```
## # A tibble: 234 x 11
##    manufac~ model   displ  year   cyl trans  drv     cty   hwy fl    class
##    <chr>    <chr>   <dbl> <int> <int> <chr>  <chr> <int> <int> <chr> <chr>
##  1 audi     a4       1.80  1999     4 auto(~ f        18    29 p     comp~
##  2 audi     a4       1.80  1999     4 manua~ f        21    29 p     comp~
##  3 audi     a4       2.00  2008     4 manua~ f        20    31 p     comp~
##  4 audi     a4       2.00  2008     4 auto(~ f        21    30 p     comp~
##  5 audi     a4       2.80  1999     6 auto(~ f        16    26 p     comp~
##  6 audi     a4       2.80  1999     6 manua~ f        18    26 p     comp~
##  7 audi     a4       3.10  2008     6 auto(~ f        18    27 p     comp~
##  8 audi     a4 qua~  1.80  1999     4 manua~ 4        18    26 p     comp~
##  9 audi     a4 qua~  1.80  1999     4 auto(~ 4        16    25 p     comp~
## 10 audi     a4 qua~  2.00  2008     4 manua~ 4        20    28 p     comp~
## # ... with 224 more rows
```

```r
ggplot(data = mpg) + geom_point(mapping =aes(x = displ, y = hwy, size = class, colour = drv))
```

```
## Warning: Using size for a discrete variable is not advised.
```

![](ggplot2_practice_seminar2b_files/figure-html/unnamed-chunk-2-1.png)<!-- -->
