# nakkery-flexgrid
Flexbox grid for html and css/stylus

Mixed column count, classes via wrapper and/or columns, custom gutter for mixed wrappers

:green_apple: [**demo**](http://j-kallunki.github.io/nakkery-flexgrid/)

Jade-HTML example:
```
article.nakkery.top.full
  header#minheightsomething.plop.nakkery.baseline.autosize.justify-center
      a(href='/').plop Baseline Autosize (justify-center)
      p.plop.tofull.med-of3.large-autosize 1of3
      p.plop.tofull.med-2of7.large-autosize 2of7
  footer.plop.tobottom
    p Flex-end
```
