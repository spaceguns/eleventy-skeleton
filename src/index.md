---
layout: layouts/base.njk
lang: en-us
oglocale: en_US
website_URL: https://www.example.com
title: Hello World
description: Description Text
images:
    - SlothA.jpg
    - SlothA.jpg
images-width: 300px
---

<p id="id1" class="center large dottedborder roundedborder">CONTENT FROM MARKDOWN PAGE</p>

<p class="font-effect-neon">next line</p> <br /> <p>break</p>

<h2>&#128512;</h2>

<i class="material-icons">computer</i>
<i class="material-icons">cloud</i>
<i class="material-icons">favorite</i>
<i class="material-icons">attachment</i>
<i class="material-icons">computer</i>

<p><div class="clearfix"><img src="img/SlothA.jpg" alt=" float right" id="float-right" width="150px" class="opacity">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus imperdiet, nulla et dictum interdum, nisi lorem egestas odio, vitae scelerisque enim ligula venenatis dolor. Maecenas nisl est, ultrices nec congue eget, auctor vitae massa. Fusce luctus vestibulum augue ut aliquet. Mauris ante ligula, facilisis sed ornare eu, lobortis in odio. Praesent convallis urna a lacus interdum ut hendrerit risus congue. Nunc sagittis dictum nisi, sed ullamcorper ipsum dignissim ac. In at libero sed nunc venenatis imperdiet sed ornare turpis. Donec vitae dui eget tellus gravida venenatis. Integer fringilla congue eros non fermentum. Sed dapibus pulvinar nibh tempor porta. Cras ac leo purus. Mauris quis diam velit.</div></p>

<div class="center">
  <p>Hello World!</p>
</div>

<!-- comment etc -->
<pre>
 _._     _,-'""`-._
(,-.`._,'(       |\`-/|
    `-.-' \ )-`( , o o)
          `-    \`_`"'-
</pre>

<p> 
<form>
  <label for="favcolor" class="font-effect-fire">Select a color:</label>
  <input type="color" id="favcolor" name="favcolor"> <br />
  <input type="date" id="birthday" name="birthday"> <br />
  <input type="email" id="email" name="email" placeholder="example@example.com" required="required" autofocus="autofocus" autocomplete="on"> <br />
  <input type="file" id="myfile" name="myfile"> <br />
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form> 
</p>

<p>
<form>
  <label for="fname">First Name</label>
  <input type="text" id="fname" name="fname">
  <label for="lname">Last Name</label>
  <input type="text" id="lname" name="lname">
</form>
</p>

<a href="sdasdsadasd">unclicked link</a>

<div id="grad1" style="text-align:center;margin:auto;color:#888888;font-size:40px;font-weight:bold">
Rainbow Background
</div>
<p><div id="grad2"></div></p>

<p>A repeating linear gradient with solid stripes:</p>
<div id="grad5"></div>

{% for filename in images %}   
    <img src="img/{{ filename }}" alt="{{ filename }}" width="{{ images-width }}" /> <a href="img/{{ filename | url_encode }}">{{ filename }}</a>  
{% endfor %}