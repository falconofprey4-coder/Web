<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مفاجأة من يوسف إلى روان</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(45deg, #ff4e50, #f9d423);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow: hidden;
            perspective: 1000px;
        }
        
        .container {
            width: 90%;
            max-width: 600px;
            text-align: center;
            position: relative;
        }
        
        /* شاشة الدخول */
        #entry-screen {
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            transition: all 0.5s ease;
        }
        
        h1 {
            color: #e84393;
            margin-bottom: 20px;
            font-size: 32px;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.1);
        }
        
        p {
            color: #636e72;
            line-height: 1.6;
            margin-bottom: 25px;
            font-size: 18px;
        }
        
        .input-group {
            margin: 25px 0;
        }
        
        input {
            width: 100%;
            padding: 15px;
            border: 2px solid #fd79a8;
            border-radius: 10px;
            font-size: 18px;
            text-align: center;
            margin-bottom: 20px;
            outline: none;
            transition: all 0.3s;
        }
        
        input:focus {
            border-color: #e84393;
            box-shadow: 0 0 15px rgba(232, 67, 147, 0.3);
        }
        
        .btn {
            background: linear-gradient(to right, #e84393, #fd79a8);
            color: white;
            border: none;
            padding: 15px 35px;
            border-radius: 50px;
            font-size: 20px;
            cursor: pointer;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(232, 67, 147, 0.3);
            display: inline-block;
            margin: 10px;
        }
        
        .btn:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(232, 67, 147, 0.4);
        }
        
        /* الصينية */
        .tray {
            width: 400px;
            height: 400px;
            position: relative;
            margin: 0 auto;
            transform-style: preserve-3d;
            transition: transform 1.5s ease-in-out;
            display: none;
        }
        
        .tray.open {
            transform: rotateX(80deg);
        }
        
        .tray .lid {
            position: absolute;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: 0 0 30px rgba(0, 0, 0, 0.2);
            backface-visibility: hidden;
            cursor: pointer;
        }
        
        .tray .lid .heart-icon {
            font-size: 80px;
            color: white;
            animation: heartbeat 1.5s infinite;
        }
        
        .tray .content {
            position: absolute;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #ff9a9e 0%, #fad0c4 100%);
            border-radius: 50%;
            transform: rotateX(180deg);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 30px;
            backface-visibility: hidden;
            color: #e84393;
        }
        
        .tray .content h2 {
            margin-bottom: 20px;
            font-size: 28px;
        }
        
        .tray .content p {
            font-size: 20px;
            margin-bottom: 15px;
        }
        
        /* تأثيرات الطيران */
        .fly-effect {
            position: fixed;
            pointer-events: none;
            font-size: 24px;
            z-index: 1000;
            animation: fly 4s forwards;
            opacity: 0;
        }
        
        @keyframes fly {
            0% {
                transform: translateY(0) rotate(0deg);
                opacity: 1;
            }
            100% {
                transform: translateY(-100vh) rotate(360deg);
                opacity: 0;
            }
        }
        
        /* تأثير نبضات القلب */
        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }
        
        /* المراحل */
        .stage {
            display: none;
            background: rgba(255, 255, 255, 0.95);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            margin-top: 30px;
        }
        
        .message {
            background: #f8f5f5;
            padding: 20px;
            border-radius: 15px;
            margin: 20px 0;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .signature {
            margin-top: 30px;
            font-style: italic;
            color: #e84393;
            font-weight: bold;
            font-size: 22px;
        }
        
        .flowers {
            font-size: 40px;
            margin: 20px 0;
            color: #e84393;
        }
        
        .fireworks {
            position: fixed;
            width: 8px;
            height: 8px;
            border-radius: 50%;
            pointer-events: none;
            opacity: 0;
        }
        
        /* تصميم متجاوب */
        @media (max-width: 768px) {
            .tray {
                width: 300px;
                height: 300px;
            }
            
            h1 {
                font-size: 28px;
            }
            
            .btn {
                padding: 12px 25px;
                font-size: 18px;
            }
        }
        
        @media (max-width: 480px) {
            .tray {
                width: 250px;
                height: 250px;
            }
            
            .tray .content {
                padding: 15px;
            }
            
            .tray .content h2 {
                font-size: 22px;
            }
            
            .tray .content p {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- شاشة الدخول -->
        <div id="entry-screen">
            <h1>أهلاً بكِ في عالمنا السحري!</h1>
            <p>هذه هدية رقمية من يوسف خصيصاً لكِ يا روان</p>
            <p>أدخلي اسمكِ لتبدأ المفاجأة...</p>
            
            <div class="input-group">
                <input type="text" id="name-input" placeholder="اسمكِ الجميل هنا...">
                <button class="btn" onclick="startExperience()">
                    <i class="fas fa-gift"></i> ابدأ المفاجأة
                </button>
            </div>
        </div>
        
        <!-- الصينية -->
        <div class="tray" id="tray">
            <div class="lid">
                <div class="heart-icon">❤</div>
            </div>
            <div class="content">
                <h2>مفاجأة!</h2>
                <p>كل عام وأنتِ منورة حياتي يا <span id="name-placeholder">روان</span></p>
                <p>أنتِ أجمل شيء حدث لي في الحياة</p>
                <div class="flowers">🌹 🌸 💐 🌷</div>
            </div>
        </div>
        
        <!-- المراحل -->
        <div class="stage" id="stage1">
            <h2>المرحلة الأولى: ذكرى لقائنا</h2>
            <div class="message">
                <p>يا روان، منذ أن دخلتِ حياتي أصبح كل شيء أجمل</p>
                <p>أتذكر أول مرة رأيتكِ فيها، وكأنها كانت بالأمس</p>
                <p>عيناكِ أضاءت حياتي وقلبي</p>
            </div>
            <button class="btn" onclick="showStage(2)">
                <i class="fas fa-arrow-right"></i> التالي
            </button>
        </div>
        
        <div class="stage" id="stage2">
            <h2>المرحلة الثانية: لماذا أحبكِ؟</h2>
            <div class="message">
                <p>أحببتكِ لأنكِ:</p>
                <p>❥ تجعلينني أفضل version من نفسي</p>
                <p>❥ تضحكتكِ هي أجمل موسيقى في حياتي</p>
                <p>❥ طيبتكِ لا توصف وجمالكِ لا يُقارن</p>
                <p>❥ وببساطة لأنكِ أنتِ</p>
            </div>
            <button class="btn" onclick="showStage(3)">
                <i class="fas fa-arrow-right"></i> التالي
            </button>
        </div>
        
        <div class="stage" id="stage3">
            <h2>المرحلة الثالثة: مستقبلنا</h2>
            <div class="message">
                <p>أتمنى أن أمضي كل حياتي إلى جانبكِ</p>
                <p>أن أسعدكِ كما تسعديني</p>
                <p>وأن أكون شريك حياتكِ إلى الأبد</p>
            </div>
            <button class="btn" onclick="flyAway()">
                <i class="fas fa-heart"></i> اضغطي للطيران من الفرحة
            </button>
            
            <p class="signature">مع كل حبي، يوسف</p>
        </div>
    </div>

    <script>
        function startExperience() {
            let name = document.getElementById('name-input').value.trim();
            if (name === '') {
                name = 'روان';
            }
            
            // تحديث الاسم في الرسالة
            document.getElementById('name-placeholder').textContent = name;
            
            // إخفاء شاشة الدخول وإظهار الصينية
            document.getElementById('entry-screen').style.display = 'none';
            document.getElementById('tray').style.display = 'block';
            
            // فتح الصينية بعد ثانيتين
            setTimeout(() => {
                document.getElementById('tray').classList.add('open');
                
                // بعد فتح الصينية، عرض المرحلة الأولى
                setTimeout(() => {
                    document.getElementById('tray').style.display = 'none';
                    showStage(1);
                    createFireworks();
                }, 2000);
            }, 2000);
        }
        
        function showStage(stageNumber) {
            // إخفاء جميع المراحل
            document.querySelectorAll('.stage').forEach(stage => {
                stage.style.display = 'none';
            });
            
            // إظهار المرحلة المطلوبة
            document.getElementById('stage' + stageNumber).style.display = 'block';
            
            // إضافة تأثيرات جميلة
            if (stageNumber === 3) {
                createHearts();
            }
        }
        
        function createHearts() {
            for (let i = 0; i < 15; i++) {
                setTimeout(() => {
                    let heart = document.createElement('div');
                    heart.innerHTML = '❤';
                    heart.classList.add('fly-effect');
                    heart.style.left = Math.random() * window.innerWidth + 'px';
                    heart.style.fontSize = (Math.random() * 30 + 20) + 'px';
                    heart.style.color = getRandomColor();
                    document.body.appendChild(heart);
                    
                    // إزالة القلوب بعد انتهاء التحليق
                    setTimeout(() => {
                        heart.remove();
                    }, 4000);
                }, i * 300);
            }
        }
        
        function createFireworks() {
            for (let i = 0; i < 50; i++) {
                setTimeout(() => {
                    let firework = document.createElement('div');
                    firework.classList.add('fireworks');
                    firework.style.left = Math.random() * window.innerWidth + 'px';
                    firework.style.top = Math.random() * window.innerHeight + 'px';
                    firework.style.background = getRandomColor();
                    document.body.appendChild(firework);
                    
                    // تأثير firework
                    setTimeout(() => {
                        firework.style.transition = 'all 0.5s ease-out';
                        firework.style.opacity = '1';
                        firework.style.transform = 'scale(20)';
                        firework.style.opacity = '0';
                        
                        // إزالة firework بعد انتهاء التأثير
                        setTimeout(() => {
                            firework.remove();
                        }, 500);
                    }, 10);
                }, i * 100);
            }
        }
        
        function flyAway() {
            // إخفاء المرحلة الحالية
            document.getElementById('stage3').style.display = 'none';
            
            // إنشاء تأثير الطيران
            for (let i = 0; i < 50; i++) {
                setTimeout(() => {
                    let text = document.createElement('div');
                    text.classList.add('fly-effect');
                    text.innerHTML = 'أنا أطير من الفرحة! ';
                    text.style.left = Math.random() * window.innerWidth + 'px';
                    text.style.fontSize = (Math.random() * 25 + 15) + 'px';
                    text.style.color = getRandomColor();
                    document.body.appendChild(text);
                    
                    // إزالة النص بعد انتهاء التحليق
                    setTimeout(() => {
                        text.remove();
                    }, 4000);
                }, i * 200);
            }
            
            // إعادة العرض بعد انتهاء التحليق
            setTimeout(() => {
                document.getElementById('stage3').style.display = 'block';
            }, 5000);
        }
        
        function getRandomColor() {
            const colors = ['#e84393', '#fd79a8', '#6c5ce7', '#00cec9', '#ff9a9e', '#fdcb6e', '#e17055'];
            return colors[Math.floor(Math.random() * colors.length)];
        }
        
        // لجعل التجربة أكثر تفاعلية عند الضغط على Enter في حقل الإدخال
        document.getElementById('name-input').addEventListener('keypress', function(e) {
            if (e.key === 'Enter') {
                startExperience();
            }
        });
    </script>
</body>
</html>
