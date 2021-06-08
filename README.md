<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CALUCULATOR</title>
    <link rel="stylesheet" href="css/Ass1.css">
</head>
<body>
    <h1>CALCULATOR</h1>
    <table>
        <thead>
         <tr>
          <td colspan="4" id="inputLable" >0</td>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td><button onclick="pushBtn(this);">7</button></td>
            <td><button onclick="pushBtn(this);">8</button></td>
            <td><button onclick="pushBtn(this);">9</button></td>
            <td><button onclick="pushBtn(this);">+</button></td>
        </tr>
        <tr>
            <td><button onclick="pushBtn(this);">4</button></td>
            <td><button onclick="pushBtn(this);">5</button></td>
            <td><button onclick="pushBtn(this);">6</button></td>
            <td><button onclick="pushBtn(this);">-</button></td>
        </tr>
    </tr>
    <tr>
        <td><button onclick="pushBtn(this);">1</button></td>
        <td><button onclick="pushBtn(this);">2</button></td>
        <td><button onclick="pushBtn(this);">3</button></td>
        <td><button onclick="pushBtn(this);">*</button></td>
    </tr>
    <tr>
        <td><button onclick="pushBtn(this);">0</button></td>
        <td><button onclick="pushBtn(this);">.</button></td>
        <td><button onclick="pushBtn(this);">/</button></td>
        <td><button onclick="pushBtn(this);">=</button></td>
    </tr>
</tbody>
<tfoot>
<tr>
    <td colspan="4"><button onclick="pushBtn(this)">Clear</button></td>
</tr>
</tfoot>
 </table>
 <script>
     var inputLable = document.getElementById('inputLable');
       function pushBtn(obj){
         var pushed = obj.innerHTML;
         if(pushed=='='){
           inputLable.innerHTML = eval(inputLable.innerHTML);
           }else if(pushed == 'Clear'){
               inputLable.innerHTML = '0';
         } else{
             if(inputLable.innerHTML =='0'){
                 inputLable.innerHTML = pushed;
             }else{
                 inputLable.innerHTML += pushed;
             }
         }           
        }
 </script>    
</body>
</html>
