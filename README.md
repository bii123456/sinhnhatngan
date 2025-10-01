<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thiệp Chúc Mừng Sinh Nhật - Tuổi Rắn</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(45deg, #fce4ec, #b3e5fc, #e1bee7, #fff9c4, #c8e6c9);
            background-size: 800%;
            font-family: 'Comic Sans MS', Arial, sans-serif;
            overflow: hidden;
            animation: gradient 10s ease infinite;
            perspective: 1000px; /* Giữ perspective cho hiệu ứng 3D */
        }
        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        .card {
            background: transparent;
            padding: 40px;
            border: 4px solid #fff9c4;
            border-radius: 25px;
            box-shadow: 0 0 20px #fce4ec, 0 0 40px #b3e5fc;
            text-align: center;
            max-width: 500px;
            width: 90%;
            position: relative;
            z-index: 10;
            animation: neon 1.5s ease-in-out infinite;
        }
        @keyframes neon {
            0%, 100% { box-shadow: 0 0 20px #fce4ec, 0 0 40px #b3e5fc; }
            50% { box-shadow: 0 0 30px #fce4ec, 0 0 50px #b3e5fc; }
        }
        h1 {
            font-size: 3.5em;
            margin: 0;
            text-shadow: 3px 3px 6px #c8e6c9, -2px -2px 4px #c8e6c9; /* Bóng đổ đậm hơn */
            -webkit-text-stroke: 2px #fff9c4; /* Viền chữ đậm hơn */
            color: black; /* Chữ màu đen */
            animation: colorChange 3s infinite;
        }
        @keyframes colorChange {
            0% { color: black; }
            33% { color: black; }
            66% { color: black; }
            100% { color: black; }
        }
        p {
            color: black; /* Chữ màu đen */
            font-size: 1.7em;
            margin: 15px 0;
            font-weight: bold;
            text-shadow: 2px 2px 5px #c8e6c9, -1px -1px 3px #c8e6c9; /* Bóng đổ đậm hơn */
            -webkit-text-stroke: 1px #fff9c4; /* Viền chữ đậm hơn */
            animation: colorChange 4s infinite;
        }
        .snake {
            position: absolute;
            font-size: 3.5em;
            animation: slither 8s ease-in-out infinite, colorChange 3s infinite;
            z-index: 5;
            text-shadow: 3px 3px 10px rgba(0, 0, 0, 0.3); /* Bóng đổ cho 3D */
        }
        @keyframes slither {
            0% { transform: translate3d(0, 0, 0) rotateX(0deg) rotateY(0deg) scale(1); }
            20% { transform: translate3d(200px, -150px, 80px) rotateX(45deg) rotateY(90deg) scale(1.2); }
            40% { transform: translate3d(350px, 100px, -80px) rotateX(90deg) rotateY(180deg) scale(0.8); }
            60% { transform: translate3d(150px, 200px, 120px) rotateX(135deg) rotateY(270deg) scale(1.1); }
            80% { transform: translate3d(-100px, -100px, -40px) rotateX(180deg) rotateY(360deg) scale(0.9); }
            100% { transform: translate3d(0, 0, 0) rotateX(0deg) rotateY(0deg) scale(1); }
        }
        .snake:nth-child(2) { animation: slither-reverse 7s ease-in-out infinite, colorChange 3s infinite; animation-delay: -0.8s; }
        .snake:nth-child(3) { animation: slither 9s ease-in-out infinite, colorChange 3s infinite; animation-delay: -1.6s; }
        .snake:nth-child(4) { animation: slither-reverse 8s ease-in-out infinite, colorChange 3s infinite; animation-delay: -2.4s; }
        .snake:nth-child(5) { animation: slither 10s ease-in-out infinite, colorChange 3s infinite; animation-delay: -3.2s; }
        .snake:nth-child(6) { animation: slither-reverse 7.5s ease-in-out infinite, colorChange 3s infinite; animation-delay: -4s; }
        .snake:nth-child(7) { animation: slither 8.5s ease-in-out infinite, colorChange 3s infinite; animation-delay: -4.8s; }
        .snake:nth-child(8) { animation: slither-reverse 9.5s ease-in-out infinite, colorChange 3s infinite; animation-delay: -5.6s; }
        .snake:nth-child(9) { animation: slither 7s ease-in-out infinite, colorChange 3s infinite; animation-delay: -6.4s; }
        .snake:nth-child(10) { animation: slither-reverse 8s ease-in-out infinite, colorChange 3s infinite; animation-delay: -7.2s; }
        @keyframes slither-reverse {
            0% { transform: translate3d(0, 0, 0) rotateX(360deg) rotateY(360deg) scale(1); }
            20% { transform: translate3d(-200px, 150px, -80px) rotateX(315deg) rotateY(270deg) scale(1.2); }
            40% { transform: translate3d(-350px, -100px, 80px) rotateX(270deg) rotateY(180deg) scale(0.8); }
            60% { transform: translate3d(-150px, -200px, -120px) rotateX(225deg) rotateY(90deg) scale(1.1); }
            80% { transform: translate3d(100px, 100px, 40px) rotateX(180deg) rotateY(0deg) scale(0.9); }
            100% { transform: translate3d(0, 0, 0) rotateX(360deg) rotateY(360deg) scale(1); }
        }
        .balloon {
            position: absolute;
            font-size: 3em;
            animation: float 4s ease-in-out infinite, colorChange 2s infinite;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-50px); }
        }
        .balloon:nth-child(11) { left: 5%; top: 10%; animation-delay: -0.5s; }
        .balloon:nth-child(12) { right: 5%; top: 15%; animation-delay: -1s; }
        .balloon:nth-child(13) { left: 10%; bottom: 15%; animation-delay: -1.5s; }
        .balloon:nth-child(14) { right: 10%; bottom: 10%; animation-delay: -2s; }
        .firework {
            position: absolute;
            width: 15px;
            height: 15px;
            border-radius: 50%;
            animation: firework 1.5s ease-out infinite;
            z-index: 2;
        }
        @keyframes firework {
            0% { transform: scale(0); opacity: 1; }
            100% { transform: scale(5); opacity: 0; }
        }
        .firework:nth-child(15) { left: 10%; top: 5%; animation-delay: -0.3s; background: #fce4ec; }
        .firework:nth-child(16) { right: 10%; top: 10%; animation-delay: -0.6s; background: #b3e5fc; }
        .firework:nth-child(17) { left: 20%; bottom: 10%; animation-delay: -0.9s; background: #e1bee7; }
        .firework:nth-child(18) { right: 20%; bottom: 5%; animation-delay: -1.2s; background: #fff9c4; }
        .firework:nth-child(19) { left: 15%; top: 15%; animation-delay: -1.5s; background: #c8e6c9; }
        .sparkle {
            position: absolute;
            font-size: 2.5em;
            color: #fff9c4;
            animation: sparkle 1s ease-in-out infinite;
        }
        @keyframes sparkle {
            0%, 100% { opacity: 0; transform: scale(0.5) rotate(0deg); }
            50% { opacity: 1; transform: scale(2) rotate(180deg); }
        }
        .sparkle:nth-child(20) { top: 5%; left: 5%; animation-delay: -0.2s; }
        .sparkle:nth-child(21) { bottom: 5%; right: 5%; animation-delay: -0.4s; }
        .sparkle:nth-child(22) { top: 15%; right: 15%; animation-delay: -0.6s; }
        .sparkle:nth-child(23) { bottom: 15%; left: 15%; animation-delay: -0.8s; }
        .sparkle:nth-child(24) { top: 10%; left: 20%; animation-delay: -1s; }
        .star {
            position: absolute;
            font-size: 2em;
            color: #ffffff;
            animation: shoot 2.5s linear infinite;
        }
        @keyframes shoot {
            0% { transform: translateX(-100vw); opacity: 1; }
            100% { transform: translateX(100vw); opacity: 0; }
        }
        .star:nth-child(25) { top: 20%; animation-delay: -0.5s; }
        .star:nth-child(26) { top: 40%; animation-delay: -1s; }
        .star:nth-child(27) { top: 60%; animation-delay: -1.5s; }
        .star:nth-child(28) { top: 80%; animation-delay: -2s; }
    </style>
</head>
<body>
    <audio autoplay loop>
        <source src="https://cdn.pixabay.com/audio/2023/03/20/audio_6b3f7b07b3.mp3" type="audio/mpeg">
    </audio>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="snake">🐍</div>
    <div class="balloon">🎈</div>
    <div class="balloon">🎈</div>
    <div class="balloon">🎈</div>
    <div class="balloon">🎈</div>
    <div class="firework"></div>
    <div class="firework"></div>
    <div class="firework"></div>
    <div class="firework"></div>
    <div class="firework"></div>
    <div class="sparkle">✨</div>
    <div class="sparkle">✨</div>
    <div class="sparkle">✨</div>
    <div class="sparkle">✨</div>
    <div class="sparkle">✨</div>
    <div class="star">⭐</div>
    <div class="star">⭐</div>
    <div class="star">⭐</div>
    <div class="star">⭐</div>
    <div class="card">
        <h1>Chúc Mừng Sinh Nhật Kim Ngân! 🐍🎉</h1>
        <p>Chúc chị tuổi mới nhiều niềm vui, bớt suy nghĩ nhe, xinh đẹp hơn, hạnh phúc hơn và nhiều tiền hơn nhe 🐍</p>
        <p> Chúc mọi điều tốt đẹp sẽ đến với chị trong tuổi mới🎈✨</p>
    </div>
</body>
</html>
