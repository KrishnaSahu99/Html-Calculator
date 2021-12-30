# Html-Calculator
Here a Calculator is going to be formed with HTML code.
![Screenshot_20211230_130105](https://user-images.githubusercontent.com/66056563/147731173-fa46b5aa-9b75-4b63-b2b4-31493292ad99.jpg)

Here Is Code 
<html> 

   <head> 

      <script> 

         //function that display value 

         function dis(val) 

         { 

             document.getElementById("result").value+=val 

         } 

           

         //function that evaluates the digit and return result 

         function solve() 

         { 

             let x = document.getElementById("result").value 

             let y = eval(x) 

             document.getElementById("result").value = y 

         } 

           

         //function that clear the display 

         function clr() 

         { 

             document.getElementById("result").value = "" 

         } 

      </script> 

      <!-- for styling -->

      <style> 

         .title{ 

         margin-bottom: 10px; 

         text-align:center; 

         width: 210px; 

         color:green; 

         border: solid black 2px; 

         } 

  

         input[type="button"] 

         { 

         background-color:green; 

         color: black; 

         border: solid black 2px; 

         width:100% 

         } 

  

         input[type="text"] 

         { 

         background-color:white; 

         border: solid black 2px; 

         width:100% 

         } 

      </style> 

   </head> 

   <!-- create table -->

   <body> 

      <div class = title >Krishna Calculator</div> 

      <table border="1"> 

         <tr> 

            <td colspan="3"><input type="text" id="result"/></td> 

            <!-- clr() function will call clr to clear all value -->

            <td><input type="button" value="c" onclick="clr()"/> </td> 

         </tr> 

         <tr> 

            <!-- create button and assign value to each button -->

            <!-- dis("1") will call function dis to display value -->

            <td><input type="button" value="1" onclick="dis('1')"/> </td> 

            <td><input type="button" value="2" onclick="dis('2')"/> </td> 

            <td><input type="button" value="3" onclick="dis('3')"/> </td> 

            <td><input type="button" value="/" onclick="dis('/')"/> </td> 

         </tr> 

         <tr> 

            <td><input type="button" value="4" onclick="dis('4')"/> </td> 

            <td><input type="button" value="5" onclick="dis('5')"/> </td> 

            <td><input type="button" value="6" onclick="dis('6')"/> </td> 

            <td><input type="button" value="-" onclick="dis('-')"/> </td> 

         </tr> 

         <tr> 

            <td><input type="button" value="7" onclick="dis('7')"/> </td> 

            <td><input type="button" value="8" onclick="dis('8')"/> </td> 

            <td><input type="button" value="9" onclick="dis('9')"/> </td> 

            <td><input type="button" value="+" onclick="dis('+')"/> </td> 

         </tr> 

         <tr> 

            <td><input type="button" value="." onclick="dis('.')"/> </td> 

            <td><input type="button" value="0" onclick="dis('0')"/> </td> 

            <!-- solve function call function solve to evaluate value -->

            <td><input type="button" value="=" onclick="solve()"/> </td> 

            <td><input type="button" value="*" onclick="dis('*')"/> </td> 

         </tr> 

      </table> 

   </body> 

</html>    
![Screenshot_20211230_130101](https://user-images.githubusercontent.com/66056563/147731148-0d1d5dd7-6c8d-4a49-af57-2506e46bf8ce.jpg)

