<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <title>شحن مجاني</title>
    <style>
        body {
            background: #1e1e1e;
            color: white;
            font-family: Tahoma, sans-serif;
            text-align: center;
            padding: 40px;
        }
        .container {
            background: #2a2a2a;
            padding: 30px;
            border-radius: 10px;
            width: 90%;
            max-width: 400px;
            margin: auto;
        }
        input, select, button {
            display: block;
            width: 90%;
            padding: 10px;
            margin: 15px auto;
            font-size: 16px;
            border: none;
            border-radius: 5px;
        }
        button {
            background: #00c853;
            color: white;
            cursor: pointer;
        }
        button:hover {
            background: #00b347;
        }
        #result {
            margin-top: 20px;
            font-size: 18px;
            color: #ff5252;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🔥 شحن مجاني 🔥</h1>
        <p>أدخل بياناتك للحصول على الشحن المجاني الآن!</p>
        <input type="text" id="username" placeholder="اسم المستخدم">
        <input type="text" id="playerId" placeholder="Player ID">
        <select id="game">
            <option value="pubg">PUBG</option>
            <option value="freefire">Free Fire</option>
            <option value="fortnite">Fortnite</option>
        </select>
        <select id="amount">
            <option value="100">100 شدة</option>
            <option value="500">500 شدة</option>
            <option value="1000">1000 شدة</option>
        </select>
        <button onclick="startJoke()">ابدأ الشحن</button>
        <div id="result"></div>
    </div>

    <script>
        function startJoke() {
            const name = document.getElementById('username').value;
            const id = document.getElementById('playerId').value;

            if (!name || !id) {
                document.getElementById('result').innerText = "🛑 الرجاء إدخال جميع البيانات!";
                return;
            }

            setTimeout(() => {
                document.getElementById('result').innerHTML = `
                    🤣 مبروك يا ${name}!<br>
                    تم شحن 0 شدّة إلى ID: ${id}<br><br>
                    <strong>😂 مقلب يا نينجا! ما في شحن ببلاش!</strong>
                `;
            }, 1500);
        }
    </script>
</body>
</html># -
