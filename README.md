<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title></s>selamat Malam</title>
<style>
    body {
        font-family: Arial, sans-serif;
        text-align: center;
        margin-top: 20vh;
        background-color: #000;
        padding: 20px;
        overflow: hidden;
        color: #fff;
    }
    h1 {
        font-size: 3em;
        text-shadow: 2px 2px 2px rgba(0, 0, 0, 0.5);
    }
    p {
        font-size: 1.5em;
        color: #ccc;
    }
    .stars {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        z-index: -1;
        pointer-events: none; /* Memastikan bintang-bintang tidak mengganggu interaksi dengan tombol */
    }
    .star {
        position: absolute;
        width: 1px;
        height: 1px;
        background-color: #fff;
        animation: twinkle 5s infinite, moveStar linear 30s infinite;
    }
    @keyframes twinkle {
        0% { opacity: 0; }
        50% { opacity: 1; }
        100% { opacity: 0; }
    }
    @keyframes moveStar {
        from { transform: translate(0, 0); }
        to { transform: translate(200vw, 200vh); }
    }
    button {
        margin: 10px;
        padding: 10px 20px;
        font-size: 1em;
        border: none;
        background-color: #333;
        color: #fff;
        cursor: pointer;
    }
</style>
</head>
<body>
    <div class="stars"></div>
    <h1>selamat malam sausann afsya ginanjar kesayangan nopall!</h1>
    <p>yaaa sudah malam dan ini adalah waktu istirahat kamuu sayangg, selamat malammm, selamat beristirahat, lupakan kejadian yang mungkin sekiranya buat kamu sedih saat ini, sekarang waktunya mengistirahatkan tubuh dan pikiran kamu dari hal hal duniaa, kamuu sudah melakukan banyak hal hebatt hari ini, proudd of you, nopall selaluu ingin berterimakasii sudah hadirr di kehidupan nopall, babayy semoga mimpii indah dan boboo nyenyakk..</p>
    <div id="buttons">
        <button id="sudahTidur">sudah boboo</button>
        <button id="belumTidur">belum boboo</button>
    </div>
    <p id="response"></p>
    <script>
        document.getElementById('sudahTidur').addEventListener('click', function() {
            document.getElementById('response').innerText = 'dadahh!';
        });

        document.getElementById('belumTidur').addEventListener('click', function() {
            document.getElementById('response').innerText = 'boboo cepatt!';
        });

        // Generate stars
        const numStars = 100;
        const starsContainer = document.querySelector('.stars');
        for (let i = 0; i < numStars; i++) {
            const star = document.createElement('div');
            star.className = 'star';
            star.style.left = `${Math.random() * 100}%`;
            star.style.top = `${Math.random() * 100}%`;
            star.style.animationDelay = `${Math.random() * 5}s`;
            starsContainer.appendChild(star);
        }
    </script>
</body>
</html>







