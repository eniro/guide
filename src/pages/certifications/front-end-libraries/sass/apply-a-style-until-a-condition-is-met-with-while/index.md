---
title: Apply a Style Until a Condition is Met with @while
---
## Apply a Style Until a Condition is Met with @while

First, define a variable $x and set it to 1. Next, use the @while directive and set $x to be less than 10.
<pre>
  $x: 1;
    @while $x < 10 {
</pre>

After setting the CSS rule for font-size, $x is incremented by 1 to avoid an infinite loop.
<pre>
  .text-#{$x} { font-size: 5px * $x; }
      $x: $x + 1;
</pre>

<h3>Solution</h3>

<pre>
  <style type='text/sass'>
  
  $x: 1;
  @while $x < 10 {
    .text-#{$x} { font-size: 5px * $x; }
    $x: $x + 1;
  }
  
  </style>

 
    <p class="text-1">Hello</p>
    <p class="text-2">Hello</p>
    <p class="text-3">Hello</p>
    <p class="text-4">Hello</p>
    <p class="text-5">Hello</p>
    <p class="text-6">Hello</p>
    <p class="text-7">Hello</p>
    <p class="text-8">Hello</p>
    <p class="text-9">Hello</p>
    <p class="text-10">Hello</p>

</pre>
