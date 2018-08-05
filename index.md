---
layout: default
title: Welcome to Chipprogrammer AMP Pages
img: /static/img/07.jpg
---

<amp-img src="{{ site.baseurl }}/static/img/macos-sierra.jpg" layout="responsive" width="266" height="150"></amp-img>
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce rutrum ac felis ac tempor. Sed venenatis, nibh ut facilisis convallis, enim turpis congue ligula, quis suscipit libero ex eu justo. Pellentesque eget luctus mauris. Cras viverra, felis id venenatis mattis, nisi massa euismod leo, quis facilisis dolor orci at elit. Proin malesuada quam in sapien mattis, id iaculis leo pulvinar. Nunc nisl odio, lobortis id eleifend sit amet, mollis a nulla. Maecenas a elementum arcu, in malesuada tellus. Nulla tristique est id dui pulvinar, at posuere ipsum sodales. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Etiam efficitur convallis urna, eget iaculis est commodo id. Phasellus molestie a justo eget consequat.

Nullam porta urna ullamcorper, interdum arcu et, pellentesque justo. Quisque facilisis viverra nisl eget porta. Suspendisse ut tempor diam. Nulla facilisi. Nam ac luctus quam. Donec sed quam eleifend, sagittis mauris vitae, ornare eros. Quisque pharetra enim a sem eleifend ultrices. Maecenas facilisis lorem leo, a efficitur augue tempus quis. Sed urna dolor, volutpat nec nibh et, tempor hendrerit sapien. Interdum et malesuada fames ac ante ipsum primis in faucibus. Fusce turpis risus, rutrum et nunc quis, pellentesque fermentum quam. Aliquam erat volutpat.

In luctus iaculis metus in tincidunt. Aliquam consequat ligula at ex porttitor, elementum convallis odio molestie. Nullam vitae sapien aliquam, luctus odio eget, cursus sem. Nullam feugiat diam ac varius rutrum. Aliquam sed nunc ac nunc vulputate volutpat ac ac nisi. Donec accumsan erat non erat interdum commodo. Duis lobortis ante elit, id mattis ex interdum ac. Etiam pharetra vel nunc sed ullamcorper. Fusce tellus leo, facilisis elementum quam vitae, iaculis eleifend sem. Nam blandit augue ut augue dictum accumsan. Nunc elementum odio eu ex tempor facilisis. Duis pellentesque interdum mauris sit amet molestie. Morbi ornare auctor mi, vitae semper lacus posuere et.

Ut tempus varius urna, ut aliquet ante pellentesque a. Fusce maximus a est non facilisis. Phasellus egestas purus a turpis tristique consectetur. Aliquam vitae leo ac lacus fermentum cursus in sit amet lacus. Pellentesque ut tellus pulvinar, fringilla lectus eu, dictum neque. Vivamus lacus orci, scelerisque quis mattis a, ultricies quis ligula. Quisque cursus cursus tincidunt. Quisque et mauris eget nibh hendrerit aliquam nec vitae quam. Sed risus tellus, vestibulum dignissim eros nec, fermentum viverra elit. Vestibulum sit amet dolor et tortor ullamcorper dapibus quis at odio. Fusce congue erat a purus volutpat laoreet eget vel odio. Etiam eu semper odio. Praesent bibendum accumsan quam eu scelerisque. Donec pellentesque tellus ut est venenatis, non feugiat odio malesuada. In hac habitasse platea dictumst.

Aliquam luctus odio ac eros lacinia, quis consectetur purus tincidunt. In lobortis viverra diam, id auctor massa blandit vitae. Etiam facilisis, massa sit amet aliquet feugiat, neque orci euismod velit, sed viverra enim enim ut massa. Phasellus non ligula posuere, maximus risus ac, porta ex. Vivamus eleifend venenatis bibendum. Aliquam consectetur facilisis dui a vehicula. Phasellus elementum lorem in nisl lobortis, ut posuere justo mattis. Maecenas tristique mauris nec leo placerat, id auctor tellus ultrices. Donec mattis sed ipsum id suscipit. In tellus lectus, pharetra quis imperdiet ac, molestie in nulla.

## Syntax Highlighting Test

```python
import RPi.GPIO as GPIO, time

# Tell the GPIO library to use
# Broadcom GPIO references
GPIO.setmode(GPIO.BCM)

# Define function to measure charge time
def RCtime (PiPin):
  measurement = 0
  # Discharge capacitor
  GPIO.setup(PiPin, GPIO.OUT)
  GPIO.output(PiPin, GPIO.LOW)
  time.sleep(0.1)

  GPIO.setup(PiPin, GPIO.IN)
  # Count loops until voltage across
  # capacitor reads high on GPIO
  while (GPIO.input(PiPin) == GPIO.LOW):
    measurement += 1

  return measurement

# Main program loop
while True:
    print (RCtime(4)) # Measure timing using GPIO4
```

## Markdown Table test

| Tables        | Are           | Cool  |    as   | Ice Cream |   and    |
|---------------|---------------|-------|---------|-----------|----------|
| col 3 is      | right-aligned | $1600 | $600000 |    Arun.  |   Arun.  |
| col 2 is      | centered      |   $12 |    $345 |     K.    |   Alwyn. |
| zebra stripes | are neat      |    $1 |    $200 |    Soman. |  Jestin. |

> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce rutrum ac felis ac tempor. Sed venenatis, nibh ut facilisis convallis, enim turpis congue ligula, quis suscipit libero ex eu justo. Pellentesque eget luctus mauris. Cras viverra, felis id venenatis mattis, nisi massa euismod leo, quis facilisis dolor orci at elit. Proin malesuada quam in sapien mattis, id iaculis leo pulvinar. Nunc nisl odio, lobortis id eleifend sit amet, mollis a nulla. Maecenas a elementum arcu, in malesuada tellus.

## Markdown List Test

* Sugar
* Bran
* Oil

1. Fuse
2. Battery 
3. Single strand wire
4. Bread board

## Tag Cloud Test

<ul class="tags">
  <li><a href="#" class="tag">HTML</a></li>
  <li><a href="#" class="tag">CSS</a></li>
  <li><a href="#" class="tag">JavaScript</a></li>
</ul>

## Related Posts lists

<ul class="cp-ul">
  <li>First post</li>
  <li>Second post</li>
  <li>Third Post</li>
</ul>

## Image Floating Test

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur quis quam vitae ipsum vehicula laoreet eget et turpis. Fusce dapibus vel magna in interdum. Sed euismod luctus lectus et fermentum. Sed efficitur tempor dui. Nulla malesuada risus nec mauris condimentum tempor. Phasellus nulla dolor, condimentum ut sollicitudin non, mattis mattis ipsum. Cras pharetra mi eu mauris aliquet, dignissim faucibus sapien lacinia. Cras at mi nisl. Phasellus ex ipsum, mattis vehicula egestas vehicula, pulvinar nec lorem. Phasellus accumsan lobortis magna, eu condimentum felis. Proin blandit est id nulla efficitur scelerisque. In vehicula nisi vel sapien venenatis, accumsan gravida ex fringilla. Mauris ac consectetur nibh.
<figure class="figure figure-right">
<amp-img src="https://unsplash.it/300/400?image=123" alt="chipprogrammer" width="320" height="200" layout="intrinsic"></amp-img>
  <figcaption>This image has a caption</figcaption>
</figure>
Etiam gravida risus nec ligula dictum ornare scelerisque vestibulum nulla. In eu dui hendrerit, hendrerit arcu in, fringilla turpis. Duis porttitor eros ut lacus tristique pulvinar. Aliquam rhoncus et elit non vulputate. Ut blandit id leo id bibendum. Nullam vel luctus mi. Mauris aliquam sem metus, et congue leo blandit at. Donec sit amet tortor justo. Proin pellentesque at risus in faucibus. Fusce ac augue non elit sollicitudin fermentum in vitae enim. Aenean eget iaculis risus. Pellentesque ultrices felis at dui ornare, at venenatis quam tincidunt.

Vestibulum viverra rutrum quam sit amet egestas. Aliquam venenatis nisi eu rhoncus laoreet. Donec convallis tellus tellus, at pulvinar velit pharetra id. Nullam varius massa eu felis placerat, vitae facilisis nibh laoreet. Maecenas posuere quam at semper cursus. Proin tempor massa non tellus bibendum venenatis. Phasellus diam ex, tempor sed lacus et, dapibus ullamcorper erat. Nam vel nisi at justo interdum faucibus. Etiam nec augue urna. Phasellus at turpis vel elit posuere lacinia. Duis tristique sapien ut lorem imperdiet, vitae efficitur augue varius. Nam porttitor nunc a sapien euismod, eu placerat elit venenatis. Curabitur ac elit faucibus odio auctor ornare vitae nec dui. Aliquam sed erat posuere, fringilla libero auctor, eleifend mauris. Vivamus sed convallis nisi. Integer rhoncus, odio ut ornare tempus, arcu magna pellentesque quam, at dictum velit metus a urna. Phasellus vitae pellentesque neque, ac auctor nulla. Nullam imperdiet vulputate urna ut lobortis. Aenean ac justo justo. Ut ut varius ligula. Fusce varius elit et erat sollicitudin laoreet. Integer iaculis ut felis eget efficitur. Aliquam vitae lorem nec lectus finibus faucibus in non nibh. Pellentesque sapien risus, vestibulum auctor erat vel, ultricies sodales orci. Donec id dignissim ipsum.
<figure class="figure figure-left">
<amp-img src="https://unsplash.it/300/400?image=123" alt="This is the alt text" height="200" width="320" layout="intrinsic"></amp-img>
  <figcaption>This image has a caption but also alt text</figcaption>
</figure>
Vestibulum viverra rutrum quam sit amet egestas. Aliquam venenatis nisi eu rhoncus laoreet. Donec convallis tellus tellus, at pulvinar velit pharetra id. Nullam varius massa eu felis placerat, vitae facilisis nibh laoreet. Maecenas posuere quam at semper cursus. Proin tempor massa non tellus bibendum venenatis. Phasellus diam ex, tempor sed lacus et, dapibus ullamcorper erat. Nam vel nisi at justo interdum faucibus. Etiam nec augue urna. Phasellus at turpis vel elit posuere lacinia. Duis tristique sapien ut lorem imperdiet, vitae efficitur augue varius. Nam porttitor nunc a sapien euismod, eu placerat elit venenatis. Curabitur ac elit faucibus odio auctor ornare vitae nec dui. Aliquam sed erat posuere, fringilla libero auctor, eleifend mauris. Vivamus sed convallis nisi.

Quisque volutpat purus arcu, sed vestibulum tortor varius at. Aliquam sagittis quis mauris a imperdiet. Proin sollicitudin nisl leo, quis dictum odio tristique et. Nulla nec malesuada est. Morbi a dignissim purus. Integer turpis urna, efficitur et elit ut, fermentum rhoncus quam. Donec sollicitudin neque mi, et hendrerit dui pellentesque vitae. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Proin ullamcorper enim nunc, non scelerisque ligula eleifend et. Praesent tincidunt eget augue eu vestibulum. Aenean lobortis vel nunc lobortis fermentum. Donec quis faucibus diam. Nullam id leo non ex elementum luctus ac ac risus. Ut commodo elit in bibendum euismod.

<figure class="figure figure-center">
<amp-img src="https://unsplash.it/800/400?image=123" alt="This image has alt text" width="320" height="200" layout="responsive"></amp-img>
  <figcaption>This image has also caption</figcaption>
</figure>
Quisque turpis arcu, lacinia quis odio vitae, pharetra porta ligula. Donec vel dolor vitae dui vulputate lacinia quis vestibulum nunc. Nam a libero laoreet, gravida magna sed, hendrerit velit. Nam lacinia vehicula vulputate. Sed venenatis erat id ante suscipit, vel viverra nibh vestibulum. Pellentesque vitae laoreet ante. Donec nec dictum enim. Phasellus sodales enim vel urna suscipit venenatis. Fusce eget quam purus. Fusce quis posuere dolor. Nam nisi risus, porta vel mollis nec, scelerisque maximus orci. Vestibulum non ligula vitae erat ullamcorper blandit. Cras commodo commodo tellus eget vestibulum. Suspendisse sollicitudin erat vitae nisl euismod venenatis.

## Pagination and Pager Test

<div class="pagination">
<a class="active" href="#" >Previous</a>
<a href="#" >1</a>
<a href="#" >2</a>
<a class="active" href="#" >3</a>
<a href="#" >4</a>
<a href="#" >5</a>
<a href="#" >6</a>
<a class="active" href="#" >Next</a>
</div>
<div class="clearfix">
<div class="pager mymt">
<a class="left" href="#">Previous</a>
<a class="right" href="#">Next</a>
</div>
</div>
