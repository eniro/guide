---
title: Apply a Style Until a Condition is Met with @while
---
## Apply a Style Until a Condition is Met with @while

<h3>Solution</h3>

<pre>
  <style type='text/sass'>
  
  $x: 1;
  @while $x < 13 {
    .text-#{$x} { font-size: 5px * $x; }
    $x: $x + 1;
  }
  
  </style>

  <figure>
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
  </figure>
</pre>
