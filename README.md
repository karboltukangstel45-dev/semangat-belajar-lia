<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Semangat Sayang!</title>
    <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@500;700&family=Pacifico&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: #ffe9f3;
            font-family: 'Quicksand', sans-serif;
            overflow: hidden;
            text-align: center;
        }

        .container {
            background: rgba(255, 255, 255, 0.8);
            padding: 30px;
            border-radius: 25px;
            box-shadow: 0 10px 30px rgba(255, 105, 180, 0.2);
            z-index: 10;
            max-width: 80%;
            animation: fadeIn 1.5s ease-out;
        }

        h1 {
            color: #ff4d94;
            font-family: 'Pacifico', cursive;
            font-size: 2.5rem;
            margin-bottom: 10px;
            animation: bounce 2s infinite;
        }

        p {
            color: #666;
            font-size: 1.1rem;
            line-height: 1.6;
        }

        .gombal {
            font-style: italic;
            color: #ff75a0;
            font-weight: bold;
            margin-top: 20px;
        }

        /* Animasi Hati Melayang */
        .heart {
            position: absolute;
            color: #ff4d94;
            font-size: 20px;
            user-select: none;
            pointer-events: none;
            animation: moveHearts 4s linear infinite;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        @keyframes moveHearts {
            0% { transform: translateY(100vh) scale(0); opacity: 1; }
            100% { transform: translateY(-10vh) scale(1.5); opacity: 0; }
        }

        .sticker {
            width: 150px;
            margin: 0 auto 20px;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="sticker">
            <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOHIyeGZ1N3Bicmt6ZzR0amN3Z3R4YWJ4eG94eG94eG94eG94eG94JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1z/3o7TKoWXlo3M1nKS6A/giphy.gif" alt="Cute Cat" width="100%">
        </div>

        <h1>Semangat Sayangg Belajarnyaaa! ✨</h1>
        
        <p>Jangan capek-capek ya belajarnya, ingat ada masa depan kita yang harus kita bangun bareng-bareng. ❤️</p>

        <div class="gombal">
            "Kamu tau gak bedanya kamu sama buku pelajaran?<br>
            Kalau buku pelajaran itu jendela dunia,<br>
            kalau kamu itu seluruh duniaku!" 🌹
        </div>
    </div>

    <script>
        // Script untuk bikin hujan hati yang smooth
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('heart');
            heart.innerHTML = '❤️';
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = Math.random() * 2 + 3 + 's';
            heart.style.fontSize = Math.random() * 20 + 10 + 'px';
            document.body.appendChild(heart);

            setTimeout(() => {
                heart.remove();
            }, 5000);
        }

        setInterval(createHeart, 300);
    </script>
</body>
</html>
bikin link website nya agar bisa di akses ke semua orang
