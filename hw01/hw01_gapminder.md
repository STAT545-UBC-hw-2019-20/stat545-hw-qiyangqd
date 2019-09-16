hw01\_gapminder
================
Qi Yang
2019/9/14

# Exploring Gapminder

## An overview of gapminder

Let’s take a look at some basic information about gapminder.

    ##         country        continent        year         lifeExp     
    ##  Afghanistan:  12   Africa  :624   Min.   :1952   Min.   :23.60  
    ##  Albania    :  12   Americas:300   1st Qu.:1966   1st Qu.:48.20  
    ##  Algeria    :  12   Asia    :396   Median :1980   Median :60.71  
    ##  Angola     :  12   Europe  :360   Mean   :1980   Mean   :59.47  
    ##  Argentina  :  12   Oceania : 24   3rd Qu.:1993   3rd Qu.:70.85  
    ##  Australia  :  12                  Max.   :2007   Max.   :82.60  
    ##  (Other)    :1632                                                
    ##       pop              gdpPercap       
    ##  Min.   :6.001e+04   Min.   :   241.2  
    ##  1st Qu.:2.794e+06   1st Qu.:  1202.1  
    ##  Median :7.024e+06   Median :  3531.8  
    ##  Mean   :2.960e+07   Mean   :  7215.3  
    ##  3rd Qu.:1.959e+07   3rd Qu.:  9325.5  
    ##  Max.   :1.319e+09   Max.   :113523.1  
    ## 

  - How many **rows** does gapminder have?

<!-- end list -->

    ## [1] 1704

  - How many **columns** does gapminder have?

<!-- end list -->

    ## [1] 6

  - What \*\*variables\* does gapminder have?

<!-- end list -->

    ## [1] "country"   "continent" "year"      "lifeExp"   "pop"       "gdpPercap"

## Maximum, minimum, mean, range

Let’s dig deeper into gapminder by finding out the maximum, minimum,
mean and range of certain variables. - Take **life expectation** of all
years and of all countries as an example:

    ##    Min. 1st Qu.  Median    Mean 3rd Qu.    Max. 
    ##   23.60   48.20   60.71   59.47   70.85   82.60

  - What is the **time** range of gapminder?

<!-- end list -->

    ## [1] 1952 2007

## Extraction based on certain criteria

We can set up a “keyword” to learn everything about it, for instance, a
country.  
\- What if we want to view all records about **Afghanistan**?

    ## # A tibble: 12 x 6
    ##    country     continent  year lifeExp      pop gdpPercap
    ##    <fct>       <fct>     <int>   <dbl>    <int>     <dbl>
    ##  1 Afghanistan Asia       1952    28.8  8425333      779.
    ##  2 Afghanistan Asia       1957    30.3  9240934      821.
    ##  3 Afghanistan Asia       1962    32.0 10267083      853.
    ##  4 Afghanistan Asia       1967    34.0 11537966      836.
    ##  5 Afghanistan Asia       1972    36.1 13079460      740.
    ##  6 Afghanistan Asia       1977    38.4 14880372      786.
    ##  7 Afghanistan Asia       1982    39.9 12881816      978.
    ##  8 Afghanistan Asia       1987    40.8 13867957      852.
    ##  9 Afghanistan Asia       1992    41.7 16317921      649.
    ## 10 Afghanistan Asia       1997    41.8 22227415      635.
    ## 11 Afghanistan Asia       2002    42.1 25268405      727.
    ## 12 Afghanistan Asia       2007    43.8 31889923      975.

## Extraction of specific information

We can also view a single piece of information that we want. - Which
country has **the highest GDP per capita** in **1972**?

    ## [1] Kuwait
    ## 142 Levels: Afghanistan Albania Algeria Angola Argentina ... Zimbabwe

  - When did **Afghanistan** have **the lowest GDP**?

<!-- end list -->

    ## [1] 1997

## Graphic

If we want to learn something more directly, we can use graphics based
on gapminder. - **Population** changes of all countries over time:  
![](hw01_gapminder_files/figure-gfm/unnamed-chunk-11-1.png)<!-- -->
