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
Usage:
```
Container: .nakkery or block&container: .plop.nakkery

with .nakkery
* grid padding : .guttery / buttery-large / guttery-xlarge
* .top : align-items flex-start
* .bottom:  align-items flex-end
* .center: align-items center
* .stretch: align-items stretch
* .baseline: align-items baseline
* .justify: justify-content space-between
* .justify-center: justify-content center
* .justify-around: justify-content space-around
* .flexy-plops: .plop display flex
* .autosize: .plop flex: none; max-width 100%: width auto
* .fit: .plop: flex 1 1 0px
* .full: .plop: flex 0 0 100%
* .for{i}: .plop: flex 0 0 round((100% / i), 3); max-width round((100% / i), 3)

with .plop
* .of{i}: flex 0 0 round((100% / i), 3); max-width round((100% / i), 3)
* .to{j}of{i}: flex 0 0 round((100% * (j / i)), 3); max-width round((100% * (j / i)), 3)
* .reset: flex 1 1 0px !important
* .totop: align-self flex-start
* .tobottom: align-self flex-end
* .tocenter: align-self center
* .tostretch: align-self stretch
* .toright: margin-left auto
* .tobottom: margin-top auto
* .toautosize: flex none; max-width 100%; width auto
* .tofit: flex 1 1 0px
* .tofull: flex 0 0 100%; max-width 100%
* .order{i}: order i

same classes starting with
.med-[top/bottom/toautosize/tofit..]: (min-width: 36em)
.large-[..]: (min-width: 48em)


Settings with variables in nakkery.styl:
$guttery = .2em
$guttery-large = .6em
$guttery-xlarge = 1em
$max-columns = 12
$max-order = 20
```
