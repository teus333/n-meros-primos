# Avaliação processual
Números primos
<!DOCTYPE html>
<!-- Nome:Douglas Cauan N-6
     Nome:Gulherme Dias N-10
     Nome:Leonardo de Melo N- 19    3B
     Nome:Luan Calvi  N-
     Nome:Matheus Moura N-24 -->
    <html lang="pt-Br">
        <head>
            <meta charset="UTF-8">
            <title>Verificador de Numero primo</title>
            <script>
            function Primos(){
            var N1=parseInt(document.getElementById("numero1").value,10);
            var canvas=document.getElementById("MeuCanvas");
            var ctxt=canvas.getContext("2d");
            ctx.font="30pxArial";
            ctx.fillStyle="blue";
            var resultado='';
           
 
            if(N1<2){
                resultado=N1 +"nao é primo";
            }
            else{
                var primo=true;
           
            for(var contador=2;contador <=Math.sqrt(N1); contador++) {
         if (N1 % contador=== 0) {
            primo= false;
            break
          
         }
    }
 
    if(primo){
        resultado=N1+ "é primo";
    }
    else{
        resultado=N1+ "nao é primo";
           }
     }
 
 ctxt.fillStyle(resultado,80,160);
        }
     </script>
     <head>
    <body>
        <label for="numero1"> O número é primo ou não?</label>
        <input type="numero" id="numero1"><br><br>  
 
 <button onclick="Primos()">Calcular</button>
 
 <canvas id="MeuCanvas" width="200" height="200"  style="border:2px solid #000000; background-color: whitesmoke;"></canvas>
 </body>
</html>
