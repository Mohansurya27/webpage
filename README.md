<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Student Registration Form</title>
<script>
  var s1,s2,s3,s4,s5,s8;
function fun1(){
if(form1.name.value=="")
{
alert("enter the name");
form1.name.focus();}
else{
var l=form1.name.value.length;
s1=new String(form1.name.value);
for(i=0;i<I;i++) {
if(!((s1.charAt(i)>='a'||s1.charAt(i)>='A') && (s1.charAt(i)<='z'||s1.charAt(i)<='Z'))){
alert("Please enter the correct name");
form1.name.focus();
break;
}}}
}
function fun2(){
if(form1.email.value==""){
alert("enter the email");
form1.email.focus();}
else{
var c1=0;
var c2=0;
var l=form1.email.value.length;
s2=new String(form1.email.value);
for(i=0;i<=l;i++){
if(s2.charAt(i)=='@'){
c1=c1+1;
var j=i;}}
if(c1==1){
for(i=j;i<=l;i++){
if(s2.charAt(i)=='.')
c2=c2+1;} }
if(!((c1==1) && (c2==1))){
alert("enter the correct e-mail id");
form1.email.focus();}}}
function fun3()
{
s3=form1.age.value;
if((s3=="")||isNaN(s3)) //isNaN() function determines whether a value is an illegal number
{
alert("enter the age");
form1.age.focus();
}
}

function fun4()
{
s4=form1.addresss.value;
if(s4=="")
{
alert("enter the address");
form1.addresss.focus();
}
}
function fun5()
{
s5=form1.phno.value;
l=form1.phno.value.length;
if((s5=="") || isNaN(s5)|| l!=10)
{
alert("Invalid phone number");
form1.phno.focus();
}
}

function fun9(){
w1=window.open('Order Conformation.html');
w1.document.writeln("<h1><center>");
w1.document.writeln("Order Conformation Details");
w1.document.writeln("</h1></center>"); 
w1.document.writeln("<br>");
w1.document.writeln("Name:",s1);
w1.document.writeln("<br>");
w1.document.writeln("Email:",s2);
w1.document.writeln("<br>");
w1.document.writeln("age:",s3);
w1.document.writeln("<br>");
w1.document.writeln("Address:",s4);
w1.document.writeln("<br>");
w1.document.writeln("Phone:",s5);
w1.document.writeln("<br>");





  
</script>
<style type="text/css">
th {
	color: #FFF;
	font-size: 24px;
	font-weight: bold;
	text-align: left;
}
body {
	background-color:#993333;
	color:white;
  font-family:verdana;
}

</style>


</head>

<body>
<form action="#">
<table border="0" align="center" cellpadding="0" cellspacing="10">
  <tr>
    <th width="25%" height="60">&nbsp;</th>
    <th><p>Student Registration Form</p></th>
    <th width="10%">&nbsp;</th>
  </tr>

  <tr>
    <td><strong>Name:</strong></td>
    <td><input name="name" type="text" onfocus="fun1()" required/></td>
  </tr>

  <tr>
    <td><strong>DOB:</strong></td>
    <td><input type="date" name="num" onfocus="" required/></td>
    
  </tr>
 
  <tr>
    <td><strong>Age:</strong></td>
    <td><input type="text" name="age" onfocus="fun3()" required/></td>
    
  </tr>

  <tr>
    <td><strong>Gender:</strong></td>
    <td><input type="radio" name="gender" value="male" required>Male
    	<input type="radio" name="gender" value="female">Female</td>
  </tr>

  <tr>
    <td><strong>Email:</strong></td>
    <td><input type="text" name="email" onfocus="fun2" size="30" required/></td>
  </tr>
  
  <tr>
    <td><strong>Password:</strong></td>
    <td><input type="Password" name="num"   required/></td>
    
  </tr>



  <tr>
    <td><strong>Address:</strong></td>
    <td><input type="text" name="address" textarea rows="6" cols="30" onfocus="fun4()" required></textarea></td>
    
  </tr>

  <tr>
    <td><strong>City:</strong></td>
    <td><input type="text" name="city" id="name" required/></td>
    
  </tr>

  <tr>
    <td><strong>State:</strong></td>
    <td><input type="text" name="state" id="name" required/></td>
    
  </tr>

  <tr>
    <td><strong>Country:</strong></td>
    <td><input type="text" name="country" id="name" required/></td>
    
  </tr>
  
  <tr>
    <td><strong>Pincode:</strong></td>
    <td><input type="text" name="pin" min="6"  required/></td>
    
  </tr>
 
 
  <tr>
    <td><strong>Mobile Number:</strong></td>
    <td><input name="phno" type="text" onfocus="fun5()"size="10"/></td>
    
  </tr>



  <tr>
    <td><input type="reset" /></td>
    <td><input type="button" value="Submit" onfocus="fun9()" onclick="fun9()"></td>
    
  </tr>
</table>
</form>
  <script src="script.js"></script>
</body>

</html>
