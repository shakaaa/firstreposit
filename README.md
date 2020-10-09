# firstreposit
Aquarium1
  <!DOCTYPE html>
	<html>
	<head>
	
	<p>Use this to calculate the mass of the fish. This site uses cookies and may be tracking yor personal data such as location and social security number.<p>
	
        <title></title>
        <script type="text/javascript">
         window.onload=function() {
    lengthObj = document.getElementById('txtLength');
    heightObj = document.getElementById('txtHeight');
    widthObj = document.getElementById('txtWidth');
	costObj = document.getElementById('tdCost');
    document.getElementById('btnReset').onclick = resetInputs;
    document.getElementById('btnCalcCost').onclick = calcCost;
function resetInputs() {
    lengthObj.value = '';
    heightObj.value = '';
    widthObj.value = '';
	costObj.innerHTML = '';	
           function calcCost()
	   {
    var length = new Number(lengthObj.value);
    var height = new Number(heightObj.value);
	var width = new Number(widthObj.value);
    costObj.innerHTML = '';
    if(isNaN(length) || isNaN(height) || isNaN(width)) {
        alert('Invalid length or height or width');
        return;
    }
                weightObj.innerHTML = length*Math.pow(girth,2)/800;
            }
        </script>
    </head>
    <body>
        <table>
            <tr>
                <td><label for="txtLength">Length (inches)</label></td>
                <td><input type="text" id="txtLength" /></td>
            </tr>
            <tr>
                <td><label for="txtGirth">Girth (inches)</label></td>
                <td><input type="text" id="txtGirth" /></td>
            </tr>
            <tr>
                <td>Weight</td>
                <td id="tdWeight"></td>
            </tr>
            <tr>
                <td></td>
                <td><button id="btnReset">Reset</button><button id="btnCalc">Calculate</button></td>
            </tr>
        </table>
    </body>
</html>
