---
id: bad87fee1348bd9aed808826
title: Disable an Element Using jQuery
challengeType: 6
videoUrl: ''
localeTitle: Desativar um elemento usando jQuery
---

## Description
<section id="description"> Você também pode alterar as propriedades não CSS dos elementos HTML com jQuery. Por exemplo, você pode desativar os botões. Quando você desativa um botão, ele fica cinza e não pode mais ser clicado. jQuery tem uma função chamada <code>.prop()</code> que permite ajustar as propriedades dos elementos. Veja como você desabilitaria todos os botões: <code>$(&quot;button&quot;).prop(&quot;disabled&quot;, true);</code> Desativar apenas o botão <code>target1</code> . </section>

## Instructions
<section id="instructions">
</section>

## Tests
<section id='tests'>

```yml
tests:
  - text: Desativar o seu botão <code>target1</code> .
    testString: 'assert($("#target1") && $("#target1").prop("disabled") && code.match(/[""]disabled[""],( true|true)/g), "Disable your <code>target1</code> button.");'
  - text: Não desabilite nenhum outro botão.
    testString: 'assert($("#target2") && !$("#target2").prop("disabled"), "Do not disable any other buttons.");'
  - text: Use apenas o jQuery para adicionar essas classes ao elemento.
    testString: 'assert(!code.match(/disabled[^<]*>/g), "Only use jQuery to add these classes to the element.");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
