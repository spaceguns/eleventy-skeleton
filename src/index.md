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

<p id="id1" class="center large">CONTENT FROM MARKDOWN PAGE</p>

next line <br /> break

<h2>&#128512;</h2>

<!-- comment etc -->
<pre>
 _._     _,-'""`-._
(,-.`._,'(       |\`-/|
    `-.-' \ )-`( , o o)
          `-    \`_`"'-
</pre>

<p> 
<form>
  <label for="favcolor">Select a color:</label>
  <input type="color" id="favcolor" name="favcolor"> <br />
  <input type="date" id="birthday" name="birthday"> <br />
  <input type="email" id="email" name="email" placeholder="example@example.com" required="required" autofocus="autofocus" autocomplete="on"> <br />
  <input type="file" id="myfile" name="myfile"> <br />
  <input type="number" id="quantity" name="quantity" min="1" max="5">
</form> 
</p>

<a href="sdasdsadasd">unclicked link</a>

{% for filename in images %}   
    <img src="img/{{ filename }}" alt="{{ filename }}" width="{{ images-width }}" /> <a href="img/{{ filename | url_encode }}">{{ filename }}</a>  
{% endfor %}