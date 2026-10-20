

<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Favorite Streamer</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            min-height: 100vh;
            background: linear-gradient(
                135deg,
                #69bfff,
                #1493ff,
                #b6e5ff
            );
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            overflow-x: hidden;
        }

        .container {
            background: rgba(255, 255, 255, 0.96);
            max-width: 650px;
            width: 100%;
            padding: 40px 25px;
            border-radius: 30px;
            text-align: center;
            box-shadow: 0 10px 35px rgba(0, 80, 150, 0.3);
            border: 3px solid white;
            animation: muncul 1.2s ease;
        }

        .heart {
            font-size: 65px;
            animation: detak 1s infinite;
        }

        h1 {
            color: #1493ff;
            font-size: 32px;
            margin: 20px 0;
        }

        h2 {
            color: #1769aa;
            font-size: 23px;
            margin-bottom: 20px;
        }

        .pesan {
            color: #285078;
            font-size: 17px;
            line-height: 1.9;
            margin: 20px 0;
        }

        .bestfriend {
            color: #1493ff;
            font-size: 27px;
            font-weight: bold;
            margin: 25px 0;
            text-shadow: 1px 1px 3px #b6e5ff;
        }

        .tombol {
            background: linear-gradient(45deg, #1493ff, #69bfff);
            color: white;
            border: none;
            padding: 14px 28px;
            border-radius: 30px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: 0.3s;
            box-shadow: 0 5px 15px #b6e5ff;
        }

        .tombol:hover {
            transform: scale(1.08);
            background: #0066cc;
        }

        #kejutan {
            display: none;
            margin-top: 25px;
            color: #1493ff;
            font-size: 20px;
            font-weight: bold;
            line-height: 1.8;
        }

        .footer {
            color: #1769aa;
            margin-top: 30px;
            font-size: 14px;
        }

        @keyframes detak {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.2);
            }
        }

        @keyframes muncul {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 26px;
            }

            h2 {
                font-size: 20px;
            }

            .pesan {
                font-size: 15px;
            }

            .bestfriend {
                font-size: 23px;
            }
        }
    </style>
</head>

<body>

    <div class="container">

        <h1>CONGRATULATIONS!</h1>

        <h2>Selamat, Streamer Favoritku!</h2>

        <div class="pesan">
            Selamat yaaa!<br>
            Kamu sudah menjadi streamer favoritku!

            <br><br>

            Terima kasih sudah hadir dengan semua
            keseruan, hiburan, dan kebahagiaanmu.
            Semoga kamu semakin sukses, semakin
            banyak yang mendukungmu, dan semua
            impianmu bisa tercapai.

            <br><br>
             Semoga sehat selalu ya jal aku sebagai viewermu senang udah bisa liat lo streamer pake komputer lagi semangat ya jal 
        </div>

        <div class="bestfriend">
            YOUR BEST FRIEND
        </div>

        <button class="tombol" onclick="kejutan()">
            Klik untuk Pesan Spesial
        </button>

        <div id="kejutan">
            You are my favorite streamer!<br>
            You are an amazing friend!<br>
            Thank you for being here!
            <br><br>
            Semangat terus yaaa!<br>
            Aku akan selalu mendukungmu!
        </div>

        <div class="footer">
           
        </div>

    </div>

    <script>
        function kejutan() {
            const pesan = document.getElementById("kejutan");

            if (pesan.style.display === "block") {
                pesan.style.display = "none";
            } else {
                pesan.style.display = "block";
            }
        }
    </script>

</body>
</html>
