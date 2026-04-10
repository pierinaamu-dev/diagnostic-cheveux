# diagnostic-cheveux
Mini projet de diagnostic capillaire en HTML,CSS et JavaScript 
<!DOCTYPE html>
<html>
<head>
    <title>Diagnostic capillaire</title>
    <style>
      body {
    background: linear-gradient(pink, white);
    color: navy;
    font-family: Arial;
    text-align: center;
    margin-top: 50px;
           }

     h1 {
    font-style: italic;
        }

    input {
    padding: 10px;
    border-radius: 10px;
    border: 1px solid gray;
          }

    button {
    background-color: green;
    color: yellow;
    padding: 10px 20px;
    margin-top: 10px;
    border-radius: 10px;
    border: none;
    cursor: pointer;
          }

    button:hover {
    background-color: darkgreen;
          }
    </style>
</head>
<body>

    <h1>Diagnostic capillaire de PierinAmu💇‍♀️</h1>

    <input type="text" id="cheveux" placeholder="Secs ou gras ?">
    <br>
    <button onclick="verifier()">Vérifier</button>

    <p id="resultat"></p>

    <script>
        function verifier() {
            let type = document.getElementById("cheveux").value.toLowerCase();
            let resultat = document.getElementById("resultat");

            if (type === "secs") {
                resultat.innerText = "Sans mentir, tes cheveux manquent d'hydratation, ils sont comme des plantes, ça demande de l'eau";
            } else if (type === "gras") {
                resultat.innerText = "Évite trop d'huile, tu exagères avec les huiles, hydrate de temps en temps tes cheveux";
            } else {
                resultat.innerText = "Désolé my friend le diagnostic de Pierina est limité 😅";
            }
        }
    </script>

</body>
</html>


