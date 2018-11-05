<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">


<h1>This week's menu</h1>
<h2>Welcome!</h2>
<p>Please enter your budget first. Then confirm afterwards.</p>

<meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="index.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
  </form>
         <input type="button" onclick="myFunction('userInput')" value="Confirm">
         
         <input type="button" onclick="document.getElementById('userInput').value = ''" value= "Clear">
  </form>
 
  
  <script>
 //Seite 1: Aufforderung zur Budget Eingabe mittels Prompt oder Textfeld
function myFunction() {
    document.getElementById('userMsg').style.color = 'green';}

var userInput = document.getElementById('userInput').value

function showMsg(){
 var userInput = document.getElementById('userInput').value 

 document.getElementById('userMsg').innerHTML = "Your budget is " + userInput + " CHF.";
}


</script>

<input type="input" maxlength="40" id="userInput" onkeyup="showMsg()" placeholder="Type budget here...">

<p id="userMsg"></p>


<p>Please select your nutrition.</p>
<script>
//Seite 2: Auswahl der Nutrition



</script>

<form id="myForm" name="myForm" action="">
  <label>
    <input type="radio" name="nutrition" value="Meat"> Meat
  </label>
  <label>
    <input type="radio" name="nutrition" value="Vegetarian"> Vegetarian
  </label>
  <label>
    <input type="radio" name="nutrition" value="Vegan"> Vegan
  </label>
</form>



<br>
<script>

//Seite 4: Menüauswahl
 var meals = [
  {main: 'Chicken Curry',
   side: 'Rice',
   price: 12 + "CHF", 
   vegetarian: false,
   vegan:false,
   cuisine: "Asian"
  },
  {main: 'OLMA Bratwurst',
   side: 'Rösti',
   price: 13.50 + "CHF", 
   vegetarian: false,
   vegan:false,
   cuisine: "SWISS"
  },
  {main: 'Ravioli',
   side: 'Tomatosauce',
   price: 8 + "CHF", 
   vegetarian: true,
   vegan: false,
   cuisine: "Italian"}];

  for(i = 0; i < meals.length; i++) {
   if (meals[i].vegetarian == true) {
   	document.write(meals[i].main + " with " + meals[i].side  + " is suitable for vegetarians." + "<br>")
  }
   else if(meals[i].vegetarian == false) {
   	document.write(meals[i].main + " with " + meals[i].side  + " is not a vegetarian dish." + "<br>")
  }
  }



</script>
</body>
</html>
