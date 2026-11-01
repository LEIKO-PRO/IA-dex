# IA-dex
IA

<!DOCTYPE html>
<html lang="ht">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>IA dex</title>

  <style>
    body {
      background: #eaf0ff;
      font-family: Arial;
      padding: 15px;
    }

    h1 {
      text-align: center;
      color: blue;
    }

    #chat {
      background: white;
      padding: 15px;
      border-radius: 12px;
      min-height: 250px;
      margin-bottom: 15px;
    }

    input {
      width: 95%;
      padding: 12px;
      border-radius: 8px;
      border: 1px solid blue;
    }

    button {
      background: blue;
      color: white;
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      margin-top: 10px;
    }
  </style>
</head>

<body>

  <h1>IA dex</h1>

  <div id="chat">
    <p><b>IA dex:</b> Bonjou! Kijan mwen ka ede w?</p>
  </div>

  <input id="kesyon"
    type="text"
    placeholder="Ekri kesyon ou...">

  <button onclick="voye()">Voye</button>

  <script>
    function voye() {
      let kesyon =
        document.getElementById("kesyon").value;

      if (kesyon.trim() === "") return;

      let chat = document.getElementById("chat");

      chat.innerHTML +=
        "<p><b>Ou:</b> " + kesyon + "</p>";

      document.getElementById("kesyon").value = "";
    }
  </script>

</body>
</html>
