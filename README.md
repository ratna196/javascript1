# javascript1 This implementation is all about Arithmetic calcuation captcha as seen in various websites
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript Arrays</h2>

<p>JavaScript array elements are accessed using numeric indexes (starting from 0).</p>

  
<!-- span and div tag   span is used for inline styling... in same line while div is block level element...-->
<input id="txt1"><span> + </span><input id="txt2"><span> = </span><input id ="sum"> <button id ="check" onclick="check()">


<script>

var arr1 = [1, 3, 5];  
var arr2 = [2,4,6];
var index=0;
document.getElementById("txt1").value = arr1[index];  
document.getElementById("txt2").value = arr2[index];
function check(){
var a,b,c;
a= Number(document.getElementById("txt1").value)
b= Number(document.getElementById("txt2").value)
c=Number(document.getElementById("sum").value)
if(c!=a+b)
{
alert("wrong an.. retype again")
document.getElementById("sum").value = ""
index=index+1 
if(index>2)
{
index=0;
}
document.getElementById("txt1").value = arr1[index];
document.getElementById("txt2").value = arr2[index];

}
}
</script>

</body>
</html>
