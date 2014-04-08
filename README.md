GWD238_Lab1
Using a form to transform a box.

<!doctype html>
<html>
<head>
<meta charset="UTF-8">
<title>Sydney Carter's Lab 1</title>

<style>
#box{
    border: 3px solid black;
    width: 100px;
    height: 100px;
}
</style>

</head>

<body>
<div id="box">div 1</div>
<form>
    <fieldset>
        <legend>Change Box</legend>
        <input type="text" id="user_info" />
        <input type="button" id="button1" value="change box" />
     </fieldset>
</form>

<script>
//ADD EVENT HANDLER TO OUR FORM BUTTON
document.getElementById('button1').onclick = function (){
    
    //CREATE VARIABLES TO STORE OUR INFO
    var text = document.getElementById('user_info').value;
    //MODIFY INPUT FOR MATHEMATICS FOR DIFFERENT HEIGHT
    var num = parseInt(text) / 2;
    //CONVERT NUMBER TO CSS VALUE
    var height = num + 'px';
    
    //CHANGE PROPERTIES OF OUR BOX
    document.getElementById('box').style.width = text;
    document.getElementById('box').style.height = height;
}
//BASIC STRUCTURE FOR EVERYTHING WE WILL DO IN JAVA
</script>

</body>
</html>

