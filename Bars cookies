<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>bar’s cookies</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #fff8f2;
            color: #4b2e05;
            direction: rtl;
        }
        h1 {
            color: #c57b57;
        }
        .flavor {
            margin: 10px;
        }
        input[type="number"] {
            width: 60px;
            padding: 5px;
            font-size: 16px;
            text-align: center;
        }
        button {
            background-color: #c57b57;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            margin-top: 15px;
        }
        button:hover {
            background-color: #a96546;
        }
    </style>
</head>
<body>
    <h1>🍪 bar’s cookies 🍪</h1>
    <h3>בחרו כמה עוגיות תרצו מכל טעם (סה״כ 24)</h3>

    <div class="flavor">
        <label>אוראו: </label>
        <input type="number" id="oreo" min="0" max="24" value="0">
    </div>
    <div class="flavor">
        <label>לוטוס: </label>
        <input type="number" id="lotus" min="0" max="24" value="0">
    </div>
    <div class="flavor">
        <label>בואנו: </label>
        <input type="number" id="bueno" min="0" max="24" value="0">
    </div>
    <div class="flavor">
        <label>סמורס: </label>
        <input type="number" id="smores" min="0" max="24" value="0">
    </div>
    <div class="flavor">
        <label>פיסטוק פטל: </label>
        <input type="number" id="pistachio" min="0" max="24" value="0">
    </div>

    <button onclick="sendToWhatsApp()">שליחה</button>

    <script>
        function sendToWhatsApp() {
            const oreo = document.getElementById('oreo').value;
            const lotus = document.getElementById('lotus').value;
            const bueno = document.getElementById('bueno').value;
            const smores = document.getElementById('smores').value;
            const pistachio = document.getElementById('pistachio').value;
            
            const total = Number(oreo) + Number(lotus) + Number(bueno) + Number(smores) + Number(pistachio);
            if (total !== 24) {
                alert("נא לוודא שסך הכול יש בדיוק 24 עוגיות 🍪 (נכון לעכשיו יש " + total + ")");
                return;
            }

            const message = `היי! אני רוצה להזמין מארז של 24 עוגיות: %0Aאוראו: ${oreo}%0Aלוטוס: ${lotus}%0Aבואנו: ${bueno}%0Aסמורס: ${smores}%0Aפיסטוק פטל: ${pistachio}`;
            const phone = "972534287885";
            const url = `https://wa.me/${phone}?text=${message}`;
            window.open(url, '_blank');
        }
    </script>
</body>
</html>
