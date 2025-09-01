<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>روبو الحب - من أجل روان</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            color: white;
        }
        
        .container {
            background: rgba(0, 0, 0, 0.7);
            border-radius: 20px;
            box-shadow: 0 0 50px rgba(255, 105, 180, 0.5);
            width: 95%;
            max-width: 600px;
            padding: 25px;
            text-align: center;
            position: relative;
            overflow: hidden;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 105, 180, 0.3);
        }
        
        .container::before {
            content: '';
            position: absolute;
            top: -10px;
            left: -10px;
            right: -10px;
            bottom: -10px;
            background: linear-gradient(45deg, #ff0099, #493240, #ff0099);
            z-index: -1;
            filter: blur(20px);
            opacity: 0.7;
        }
        
        h1 {
            color: #ff5e94;
            margin-bottom: 20px;
            text-shadow: 0 0 10px #ff5e94;
            font-size: 2.5rem;
        }
        
        .robot-container {
            position: relative;
            width: 100%;
            height: 250px;
            margin: 20px 0;
            perspective: 1000px;
        }
        
        .robot {
            position: absolute;
            width: 150px;
            height: 150px;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
            transition: all 1s ease;
        }
        
        .head {
            width: 120px;
            height: 120px;
            background: linear-gradient(135deg, #6e8efb, #a777e3);
            border-radius: 50%;
            margin: 0 auto;
            position: relative;
            box-shadow: 0 0 20px rgba(167, 119, 227, 0.8);
            animation: floating 3s ease-in-out infinite;
            overflow: hidden;
        }
        
        .head::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(to bottom right, rgba(255,255,255,0.2), rgba(255,255,255,0));
            transform: rotate(45deg);
        }
        
        .eyes {
            display: flex;
            justify-content: space-around;
            padding-top: 35px;
            transition: all 0.5s ease;
        }
        
        .eye {
            width: 25px;
            height: 25px;
            background-color: #fff;
            border-radius: 50%;
            position: relative;
            animation: blink 4s infinite;
            overflow: hidden;
            box-shadow: 0 0 10px rgba(255, 255, 255, 0.8);
        }
        
        .pupil {
            width: 12px;
            height: 12px;
            background: radial-gradient(circle, #000, #333);
            border-radius: 50%;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            transition: all 0.3s ease;
        }
        
        .mouth {
            width: 40px;
            height: 10px;
            background: linear-gradient(to right, #ff5e94, #ff2e63);
            border-radius: 10px;
            margin: 15px auto 0;
            transition: all 0.5s ease;
            box-shadow: 0 0 10px rgba(255, 46, 99, 0.8);
        }
        
        .speaking .mouth {
            animation: speak 0.5s infinite alternate;
        }
        
        .chat-container {
            background: rgba(0, 0, 0, 0.5);
            border-radius: 15px;
            padding: 15px;
            margin: 20px 0;
            height: 200px;
            overflow-y: auto;
            text-align: right;
            box-shadow: inset 0 0 10px rgba(255, 105, 180, 0.5);
            border: 1px solid rgba(255, 105, 180, 0.3);
        }
        
        .message {
            margin: 10px 0;
            padding: 10px 15px;
            border-radius: 15px;
            max-width: 80%;
            display: inline-block;
            animation: fadeIn 0.5s;
            position: relative;
        }
        
        .bot-message {
            background: linear-gradient(135deg, #6e8efb, #a777e3);
            color: white;
            text-align: right;
            margin-left: auto;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .user-message {
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            color: #333;
            text-align: left;
            margin-right: auto;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .input-container {
            display: flex;
            margin-top: 15px;
            position: relative;
        }
        
        input {
            flex: 1;
            padding: 15px;
            border: none;
            border-radius: 30px;
            background: rgba(255, 255, 255, 0.1);
            outline: none;
            font-size: 16px;
            color: white;
            box-shadow: inset 0 0 10px rgba(255, 105, 180, 0.3);
            border: 1px solid rgba(255, 105, 180, 0.5);
            transition: all 0.3s ease;
        }
        
        input:focus {
            box-shadow: inset 0 0 15px rgba(255, 105, 180, 0.5), 0 0 20px rgba(255, 105, 180, 0.5);
        }
        
        input::placeholder {
            color: rgba(255, 255, 255, 0.6);
        }
        
        button {
            background: linear-gradient(135deg, #ff5e94, #ff2e63);
            color: white;
            border: none;
            border-radius: 30px;
            padding: 15px 25px;
            margin-right: 10px;
            cursor: pointer;
            font-weight: bold;
            transition: all 0.3s ease;
            box-shadow: 0 0 15px rgba(255, 46, 99, 0.5);
        }
        
        button:hover {
            transform: scale(1.05);
            box-shadow: 0 0 20px rgba(255, 46, 99, 0.8);
        }
        
        .hearts {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .heart {
            position: absolute;
            font-size: 20px;
            color: #ff5e94;
            opacity: 0;
            animation: float 6s linear infinite;
            text-shadow: 0 0 10px #ff5e94;
        }
        
        .phase-indicator {
            display: flex;
            justify-content: center;
            margin-top: 15px;
        }
        
        .phase {
            width: 15px;
            height: 15px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 50%;
            margin: 0 8px;
            transition: all 0.5s ease;
            box-shadow: 0 0 10px rgba(255, 105, 180, 0.5);
        }
        
        .phase.active {
            background: linear-gradient(135deg, #ff5e94, #ff2e63);
            transform: scale(1.5);
            box-shadow: 0 0 15px rgba(255, 46, 99, 0.8);
        }
        
        .welcome-text {
            font-size: 1.2rem;
            margin-bottom: 20px;
            color: #a777e3;
            text-shadow: 0 0 5px #a777e3;
        }
        
        .romantic-phase {
            display: none;
            animation: fadeIn 1s;
        }
        
        .romantic-phase.active {
            display: block;
        }
        
        .phase-title {
            font-size: 1.8rem;
            color: #ff5e94;
            margin: 15px 0;
            text-shadow: 0 0 10px #ff5e94;
        }
        
        .phase-content {
            background: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 15px;
            margin: 15px 0;
            box-shadow: inset 0 0 10px rgba(255, 105, 180, 0.3);
            border: 1px solid rgba(255, 105, 180, 0.3);
        }
        
        .stars {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -2;
        }
        
        .star {
            position: absolute;
            background: white;
            border-radius: 50%;
            animation: twinkle 5s infinite;
        }
        
        @keyframes blink {
            0%, 40%, 80%, 100% {
                height: 25px;
            }
            20%, 60% {
                height: 5px;
            }
        }
        
        @keyframes speak {
            from {
                height: 5px;
            }
            to {
                height: 15px;
            }
        }
        
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-100px) rotate(360deg);
                opacity: 0;
            }
        }
        
        @keyframes floating {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-15px);
            }
        }
        
        @keyframes twinkle {
            0%, 100% {
                opacity: 0.2;
            }
            50% {
                opacity: 1;
            }
        }
        
        @keyframes moveAround {
            0% {
                left: 50%;
            }
            25% {
                left: 30%;
            }
            50% {
                left: 50%;
            }
            75% {
                left: 70%;
            }
            100% {
                left: 50%;
            }
        }
        
        @keyframes surprise {
            0%, 100% {
                transform: translate(-50%, -50%) scale(1);
            }
            50% {
                transform: translate(-50%, -50%) scale(1.2);
            }
        }
        
        .surprise {
            animation: surprise 0.5s ease-in-out;
        }
        
        .move-around {
            animation: moveAround 5s ease-in-out infinite;
        }
        
        .looking-around .pupil {
            animation: lookAround 3s ease-in-out infinite;
        }
        
        @keyframes lookAround {
            0%, 100% {
                transform: translate(-50%, -50%);
            }
            25% {
                transform: translate(-70%, -50%);
            }
            50% {
                transform: translate(-50%, -70%);
            }
            75% {
                transform: translate(-30%, -50%);
            }
        }
        
        .fireworks {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }
        
        .firework {
            position: absolute;
            border-radius: 50%;
            opacity: 0;
        }
        
        @keyframes explode {
            0% {
                transform: translate(-50%, -50%) scale(0);
                opacity: 1;
            }
            100% {
                transform: translate(var(--tx), var(--ty)) scale(1);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>روبو الحب <i class="fas fa-heart"></i></h1>
        <div class="welcome-text" id="welcome-text">مرحباً بك في عالم الرومانسية</div>
        
        <div class="robot-container">
            <div class="robot" id="robot">
                <div class="head">
                    <div class="eyes">
                        <div class="eye"><div class="pupil"></div></div>
                        <div class="eye"><div class="pupil"></div></div>
                    </div>
                    <div class="mouth"></div>
                </div>
            </div>
        </div>
        
        <div class="phase-indicator">
            <div class="phase" id="phase1"></div>
            <div class="phase" id="phase2"></div>
            <div class="phase" id="phase3"></div>
        </div>
        
        <div id="phase1-content" class="romantic-phase active">
            <div class="chat-container" id="chat">
                <!-- الرسائل ستظهر هنا -->
            </div>
            
            <div class="input-container">
                <input type="text" id="user-input" placeholder="اكتبي رسالتك هنا...">
                <button id="send-btn"><i class="fas fa-paper-plane"></i> إرسال</button>
            </div>
        </div>
        
        <div id="phase2-content" class="romantic-phase">
            <div class="phase-title">المرحلة الثانية: رحلة إلى القلب</div>
            <div class="phase-content">
                <p>الآن وقد عرفتكِ يا روان، دعينا نبدأ رحلتنا الرومانسية</p>
                <p>أخبريني، ما هو أكثر شيء تحبينه في الحب؟</p>
            </div>
            <div class="input-container">
                <input type="text" id="phase2-input" placeholder="ما هو أكثر شيء تحبينه في الحب؟">
                <button id="phase2-btn"><i class="fas fa-heart"></i> تابعي</button>
            </div>
        </div>
        
        <div id="phase3-content" class="romantic-phase">
            <div class="phase-title">المرحلة الثالثة: الوصول إلى القلعة</div>
            <div class="phase-content">
                <p>تهانينا يا روان! لقد وصلتي إلى القلعة الرومانسية</p>
                <p>هنا حيث تتحقق الأحلام وتزهر المشاعر</p>
                <p>أنتِ شخص استثنائي، وأنا سعيد بأنني أستطيع مشاركة هذه اللحظات معك</p>
            </div>
            <button id="restart-btn"><i class="fas fa-redo"></i> بدء رحلة جديدة</button>
        </div>
    </div>
    
    <div class="hearts" id="hearts"></div>
    <div class="stars" id="stars"></div>
    <div class="fireworks" id="fireworks"></div>
    
    <audio id="background-music" loop>
        <source src="https://cdn.pixabay.com/download/audio/2021/10/25/audio_172d7dec90.mp3?filename=soft-romantic-background-music-6986.mp3" type="audio/mpeg">
    </audio>
    
    <audio id="sound-effect">
        <source src="" type="audio/mpeg">
    </audio>
    
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const chatContainer = document.getElementById('chat');
            const userInput = document.getElementById('user-input');
            const sendBtn = document.getElementById('send-btn');
            const robot = document.getElementById('robot');
            const mouth = document.querySelector('.mouth');
            const heartsContainer = document.getElementById('hearts');
            const starsContainer = document.getElementById('stars');
            const fireworksContainer = document.getElementById('fireworks');
            const phases = document.querySelectorAll('.phase');
            const welcomeText = document.getElementById('welcome-text');
            const backgroundMusic = document.getElementById('background-music');
            const soundEffect = document.getElementById('sound-effect');
            const phase1Content = document.getElementById('phase1-content');
            const phase2Content = document.getElementById('phase2-content');
            const phase3Content = document.getElementById('phase3-content');
            const phase2Input = document.getElementById('phase2-input');
            const phase2Btn = document.getElementById('phase2-btn');
            const restartBtn = document.getElementById('restart-btn');
            
            let currentPhase = 1;
            let conversationStep = 0;
            let userName = "";
            
            // إنشاء النجوم في الخلفية
            function createStars() {
                for (let i = 0; i < 100; i++) {
                    const star = document.createElement('div');
                    star.classList.add('star');
                    star.style.width = Math.random() * 3 + 'px';
                    star.style.height = star.style.width;
                    star.style.left = Math.random() * 100 + 'vw';
                    star.style.top = Math.random() * 100 + 'vh';
                    star.style.animationDelay = Math.random() * 5 + 's';
                    starsContainer.appendChild(star);
                }
            }
            
            // رسائل الروبوت لكل مرحلة
            const messages = {
                phase1: [
                    "مرحباً! من هناك؟ هل هناك أحد؟",
                    "أرى أن هناك شخصاً ما قد دخل! من أنت؟",
                    "أنتِ إنسانة، أليس كذلك؟ أخبريني ما اسمك!",
                    "يجب أن تخبريني باسمك الحقيقي، لا تكذبي عليّ!",
                    "أوه، روان! يا للروعة! هذا اسم جميل!",
                    "حسناً يا روان، هل أنت مستعدة لبدء رحلتنا الرومانسية؟"
                ]
            };
            
            // إنشاء رسالة في الدردشة
            function addMessage(text, isUser = false) {
                const messageDiv = document.createElement('div');
                messageDiv.classList.add('message');
                messageDiv.classList.add(isUser ? 'user-message' : 'bot-message');
                messageDiv.textContent = text;
                chatContainer.appendChild(messageDiv);
                chatContainer.scrollTop = chatContainer.scrollHeight;
            }
            
            // جعل الروبوت يتحدث
            function robotSpeak(text, callback) {
                mouth.parentElement.classList.add('speaking');
                addMessage(text);
                
                // محاكاة الصوت باستخدام Web Speech API
                try {
                    const speech = new SpeechSynthesisUtterance(text);
                    speech.lang = 'ar-SA';
                    speech.rate = 0.9;
                    speech.pitch = 1.2;
                    speech.onend = function() {
                        mouth.parentElement.classList.remove('speaking');
                        if (callback) callback();
                    };
                    window.speechSynthesis.speak(speech);
                } catch (e) {
                    // إذا لم يعمل Web Speech API، ننتظر قليلاً ثم ننفذ callback
                    setTimeout(() => {
                        mouth.parentElement.classList.remove('speaking');
                        if (callback) callback();
                    }, text.length * 100);
                }
            }
            
            // إنشاء قلوب متحركة
            function createHearts() {
                for (let i = 0; i < 15; i++) {
                    setTimeout(() => {
                        const heart = document.createElement('div');
                        heart.classList.add('heart');
                        heart.innerHTML = '❤️';
                        heart.style.left = Math.random() * 100 + 'vw';
                        heart.style.animationDuration = (Math.random() * 4 + 3) + 's';
                        heartsContainer.appendChild(heart);
                        
                        setTimeout(() => {
                            heart.remove();
                        }, 6000);
                    }, i * 400);
                }
            }
            
            // إنشاء ألعاب نارية
            function createFireworks() {
                for (let i = 0; i < 20; i++) {
                    setTimeout(() => {
                        const firework = document.createElement('div');
                        firework.classList.add('firework');
                        firework.style.left = Math.random() * 100 + 'vw';
                        firework.style.top = Math.random() * 100 + 'vh';
                        firework.style.width = Math.random() * 8 + 2 + 'px';
                        firework.style.height = firework.style.width;
                        firework.style.background = `radial-gradient(circle, 
                            ${getRandomColor()}, 
                            ${getRandomColor()})`;
                        firework.style.setProperty('--tx', (Math.random() * 100 - 50) + 'px');
                        firework.style.setProperty('--ty', (Math.random() * 100 - 50) + 'px');
                        firework.style.animation = `explode ${Math.random() * 1 + 0.5}s ease-out forwards`;
                        fireworksContainer.appendChild(firework);
                        
                        setTimeout(() => {
                            firework.remove();
                        }, 2000);
                    }, i * 300);
                }
            }
            
            function getRandomColor() {
                const colors = ['#ff5e94', '#6e8efb', '#a777e3', '#ff2e63', '#00ffff', '#ffff00'];
                return colors[Math.floor(Math.random() * colors.length)];
            }
            
            // حركة الروبوت المفاجئة
            function surpriseMovement() {
                robot.classList.add('surprise');
                setTimeout(() => {
                    robot.classList.remove('surprise');
                }, 500);
            }
            
            // حركة التطلع حوله
            function lookAround() {
                document.querySelector('.eyes').classList.add('looking-around');
                setTimeout(() => {
                    document.querySelector('.eyes').classList.remove('looking-around');
                }, 3000);
            }
            
            // حركة التنقل في الشاشة
            function moveAround() {
                robot.classList.add('move-around');
                setTimeout(() => {
                    robot.classList.remove('move-around');
                }, 5000);
            }
            
            // تغيير المرحلة
            function setPhase(phaseNum) {
                currentPhase = phaseNum;
                phases.forEach((phase, index) => {
                    if (index + 1 === phaseNum) {
                        phase.classList.add('active');
                    } else {
                        phase.classList.remove('active');
                    }
                });
                
                // إخفاء وإظهار محتوى المراحل
                phase1Content.classList.remove('active');
                phase2Content.classList.remove('active');
                phase3Content.classList.remove('active');
                
                if (phaseNum === 1) {
                    phase1Content.classList.add('active');
                } else if (phaseNum === 2) {
                    phase2Content.classList.add('active');
                } else if (phaseNum === 3) {
                    phase3Content.classList.add('active');
                    createFireworks();
                }
                
                conversationStep = 0;
            }
            
            // معالجة إرسال الرسائل
            function handleSendMessage() {
                const message = userInput.value.trim();
                if (message === '') return;
                
                addMessage(message, true);
                userInput.value = '';
                
                // في المرة الأولى نأخذ الاسم
                if (conversationStep === 0) {
                    userName = message;
                    setTimeout(() => {
                        surpriseMovement();
                        robotSpeak("أوه! " + userName + "! يا له من اسم جميل!", () => {
                            conversationStep = 1;
                            setTimeout(() => {
                                robotSpeak("هل هذا اسمك الحقيقي؟ يجب أن تكوني صادقة معي!", () => {
                                    conversationStep = 2;
                                });
                            }, 1000);
                        });
                    }, 1000);
                } 
                // التأكد من الاسم
                else if (conversationStep === 2) {
                    if (message.toLowerCase().includes("نعم") || message.includes("صحيح") || message.includes("ايوه")) {
                        setTimeout(() => {
                            moveAround();
                            robotSpeak("أحسنت! الصدق هو مفتاح القلب!", () => {
                                conversationStep = 3;
                                setTimeout(() => {
                                    robotSpeak("والآن يا " + userName + "، هل أنت مستعدة لبدء رحلتنا الرومانسية؟", () => {
                                        conversationStep = 4;
                                    });
                                }, 1000);
                            });
                        }, 1000);
                    } else {
                        setTimeout(() => {
                            robotSpeak("لا تكذبي عليّ! أخبريني اسمك الحقيقي!", () => {
                                conversationStep = 0;
                            });
                        }, 1000);
                    }
                } 
                // بدء الرحلة الرومانسية
                else if (conversationStep === 4) {
                    if (message.toLowerCase().includes("نعم") || message.includes("موافق") || message.includes("ابدا")) {
                        setTimeout(() => {
                            robotSpeak("رائع! لنبدأ الرحلة!", () => {
                                setPhase(2);
                                createHearts();
                            });
                        }, 1000);
                    } else {
                        setTimeout(() => {
                            robotSpeak("لا بأس، سأنتظر حتى تكوني مستعدة...", () => {
                                conversationStep = 3;
                            });
                        }, 1000);
                    }
                }
            }
            
            // الانتقال إلى المرحلة الثالثة
            phase2Btn.addEventListener('click', function() {
                const message = phase2Input.value.trim();
                if (message === '') return;
                
                setPhase(3);
                createHearts();
                createFireworks();
            });
            
            // إعادة البدء
            restartBtn.addEventListener('click', function() {
                setPhase(1);
                conversationStep = 0;
                userName = "";
                chatContainer.innerHTML = "";
                phase2Input.value = "";
                
                // إعادة بدء المحادثة
                setTimeout(() => {
                    lookAround();
                    robotSpeak("مرحباً! من هناك؟ هل هناك أحد؟", () => {
                        conversationStep = 0;
                    });
                }, 1000);
            });
            
            // إضافة event listeners
            sendBtn.addEventListener('click', handleSendMessage);
            userInput.addEventListener('keypress', function(e) {
                if (e.key === 'Enter') {
                    handleSendMessage();
                }
            });
            
            // بدء المحادثة عند تحميل الصفحة
            setTimeout(() => {
                createStars();
                lookAround();
                setTimeout(() => {
                    moveAround();
                    robotSpeak("مرحباً! من هناك؟ هل هناك أحد؟", () => {
                        conversationStep = 0;
                    });
                }, 1000);
                
                // حاول تشغيل الموسيقى الخلفية
                try {
                    backgroundMusic.volume = 0.3;
                    backgroundMusic.play();
                } catch (e) {
                    console.log("تعذر تشغيل الموسيقى الخلفية");
                }
            }, 1000);
        });
    </script>
</body>
</html>
