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
}
            function resetInputs() {
                lengthObj.value = '';
                girthObj.value = '';
                weightObj.innerHTML = '';
            }
            function calcWeight() {
                var length = new Number(lengthObj.value);
                var girth = new Number(girthObj.value);
                weightObj.innerHTML = '';
                if(isNaN(length) || isNaN(girth)) {
                    alert('Invalid length or girth');
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
