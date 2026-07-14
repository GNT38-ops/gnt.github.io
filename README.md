# gnt.github.io.
[index](https://github.com/user-attachments/files/30014243/G.N.T.web.html)
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GNT - Génération Numérique Tissemsilt</title>
    <!-- استدعاء أيقونات FontAwesome للشبكات الاجتماعية -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* إعدادات الخلفية الرقمية المتطورة */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #02050a; /* أسود عميق متناسق مع خلفية الصورة */
            color: #ffffff;
            overflow: hidden;
            position: relative;
        }

        /* تأثير الرقمنة (خلفية مصفوفة البيانات الثنائية 0101) */
        .digital-matrix {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle, rgba(0, 114, 255, 0.12) 0%, transparent 80%);
            z-index: 1;
            pointer-events: none;
        }

        /* شبكة الرقمنة والخطوط المتقاطعة */
        .cyber-grid {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: 
                linear-gradient(0deg, transparent 24%, rgba(0, 198, 255, 0.04) 25%, rgba(0, 198, 255, 0.04) 26%, transparent 27%, transparent),
                linear-gradient(90deg, transparent 24%, rgba(0, 198, 255, 0.04) 25%, rgba(0, 198, 255, 0.04) 26%, transparent 27%, transparent);
            background-size: 50px 50px;
            z-index: 2;
            animation: gridScroll 30s linear infinite;
        }

        @keyframes gridScroll {
            0% { background-position: 0 0; }
            100% { background-position: 50px 50px; }
        }

        /* رموز الرقمنة المتساقطة في الخلفية */
        .matrix-binary {
            position: absolute;
            width: 100%;
            height: 100%;
            z-index: 3;
            opacity: 0.15;
            pointer-events: none;
            font-family: monospace;
            font-size: 14px;
            color: #00c6ff;
            line-height: 1;
            overflow: hidden;
        }

        .matrix-column {
            position: absolute;
            top: -100px;
            animation: fall 10s linear infinite;
        }

        @keyframes fall {
            0% { top: -10%; opacity: 0; }
            50% { opacity: 1; }
            100% { top: 100%; opacity: 0; }
        }

        /* حاوية المحتوى الزجاجية الفخمة */
        .container {
            position: relative;
            text-align: center;
            background: rgba(2, 5, 10, 0.92); /* خلفية داكنة لتندمج مع الصور تماماً */
            padding: 40px 30px;
            border-radius: 24px;
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.9), 0 0 30px rgba(0, 114, 255, 0.25);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px rgba(0, 198, 255, 0.25) solid;
            width: 90%;
            max-width: 440px;
            z-index: 10;
        }

        /* تصميم قسم الترحيب الكبير */
        .welcome-section {
            margin-bottom: 25px;
            border-bottom: 1px dashed rgba(0, 198, 255, 0.2);
            padding-bottom: 15px;
        }

        .welcome-ar {
            font-size: 28px;
            font-weight: 800;
            background: linear-gradient(135deg, #ffffff 30%, #a5bccc 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin: 0;
            letter-spacing: 0.5px;
        }

        .welcome-en {
            font-size: 16px;
            font-weight: 700;
            color: #00c6ff;
            text-transform: uppercase;
            letter-spacing: 3px;
            margin: 5px 0 0 0;
            text-shadow: 0 0 8px rgba(0, 198, 255, 0.4);
        }

        /* حاوية الصورة الدائرية (الحلقة المستديرة) */
        .photo-container {
            width: 170px;
            height: 170px;
            margin: 0 auto 25px auto;
            border-radius: 50%;
            position: relative;
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: 0 0 20px rgba(0, 114, 255, 0.5);
            background-color: #02050a;
        }

        /* تأثير التوهج النبضي الدائري حول الحلقة */
        .photo-container::after {
            content: '';
            position: absolute;
            top: -4px;
            left: -4px;
            right: -4px;
            bottom: -4px;
            border-radius: 50%;
            border: 2px solid #0072ff;
            box-shadow: 0 0 20px rgba(0, 198, 255, 0.7), inset 0 0 10px rgba(0, 114, 255, 0.4);
            animation: pulseRing 3s infinite ease-in-out;
            pointer-events: none;
        }

        @keyframes pulseRing {
            0% { transform: scale(1); opacity: 0.8; }
            50% { transform: scale(1.04); opacity: 1; box-shadow: 0 0 25px rgba(0, 198, 255, 0.8); }
            100% { transform: scale(1); opacity: 0.8; }
        }

        /* تصميم الشعار داخل الدائرة بشكل متناسق ومحتوى بالكامل */
        .personal-photo {
            width: 100%;
            height: 100%;
            border-radius: 50%;
            object-fit: contain; /* لضمان عدم اقتصاص أطراف الشعار وظهوره كاملاً */
            z-index: 3;
            background-color: #02050a; /* تندمج خلفية الشعار السوداء مع خلفية الدائرة */
            border: 2px solid rgba(255, 255, 255, 0.1);
        }

        /* الوصف العام للمحل */
        p.description {
            font-size: 15px;
            font-weight: 600;
            color: #a5bccc;
            margin-bottom: 25px;
            line-height: 1.6;
            letter-spacing: 0.5px;
        }

        /* حاوية الأزرار */
        .links-container {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        /* تصميم الأزرار العام */
        .link-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 15px;
            padding: 13px;
            text-decoration: none;
            color: white;
            font-size: 16px;
            font-weight: bold;
            border-radius: 50px;
            transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            position: relative;
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        /* تأثير لمعان السرعة */
        .link-btn::after {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.25), transparent);
            transition: 0.5s;
        }

        .link-btn:hover::after {
            left: 100%;
        }

        .link-btn:hover {
            transform: translateY(-4px);
            box-shadow: 0 8px 20px rgba(0, 114, 255, 0.5);
            border-color: rgba(0, 198, 255, 0.6);
        }

        /* الألوان الخاصة بالمنصات */
        .whatsapp { background: linear-gradient(135deg, #25D366, #128C7E); }
        .facebook { background: linear-gradient(135deg, #1877F2, #0050b3); }
        .instagram { background: linear-gradient(45deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%); }
        .gmail { background: linear-gradient(135deg, #EA4335, #C5221F); }

        .link-btn i {
            font-size: 20px;
            transition: transform 0.3s ease;
        }

        .link-btn:hover i {
            transform: scale(1.25);
        }
    </style>
</head>
<body>

    <!-- الخلفيات الرقمية وعلامات الرقمنة المتفاعلة والمتحركة -->
    <div class="digital-matrix"></div>
    <div class="cyber-grid"></div>
    
    <!-- مصفوفة الأرقام الثنائية للرقمنة -->
    <div class="matrix-binary">
        <div class="matrix-column" style="left: 5%; animation-delay: 0s;">01101010110</div>
        <div class="matrix-column" style="left: 15%; animation-delay: 3s;">10010110011</div>
        <div class="matrix-column" style="left: 25%; animation-delay: 1s;">01101001010</div>
        <div class="matrix-column" style="left: 75%; animation-delay: 5s;">11010101100</div>
        <div class="matrix-column" style="left: 85%; animation-delay: 2s;">01001011010</div>
        <div class="matrix-column" style="left: 95%; animation-delay: 4s;">10110100101</div>
    </div>

    <div class="container">
        <!-- قسم الترحيب الكبير والمميز باللغتين العربية والانجليزية -->
        <div class="welcome-section">
            <h1 class="welcome-ar">أهلاً وسهلاً بكم</h1>
            <h2 class="welcome-en">Welcome to GNT</h2>
        </div>

        <!-- الحلقة المستديرة: بداخلها شعار GNT مباشرة من الإنترنت ليعمل فوراً وبشكل رائع -->
        <div class="photo-container">
            <img src="https://i.imgur.com/W9IZETy.png" alt="GNT Logo" class="personal-photo">
        </div>
        
        <!-- الوصف العام للمحل -->
        <p class="description">Génération Numérique Tissemsilt<br>للإعلام الآلي والأعمال الرقمية والإدارية</p>

        <!-- أزرار وسائل التواصل الاجتماعي المحدثة بالكامل -->
        <div class="links-container">
            
            <!-- رابط واتس أب المباشر -->
            <a href="https://wa.me/213673899245?text=%D9%85%D8%B1%D8%AD%D8%A8%D8%A7%D9%8B%20GNT%D8%8C%20%D8%A3%D8%B1%D9%8I%D8%AF%20%D8%A7%D9%84%D8%A7%D8%B3%D8%AA%D9%81%D8%B3%D8%A7%D8%B1%20%D8%B9%D9%86%20%D8%AE%D8%AF%D9%85%D8%A7%D8%AA%D9%83%D9%85" target="_blank" class="link-btn whatsapp">
                <i class="fab fa-whatsapp"></i>
                تواصل معنا عبر واتساب
            </a>

            <!-- رابط صفحة فيسبوك -->
            <a href="https://www.facebook.com/profile.php?id=61580694640353" target="_blank" class="link-btn facebook">
                <i class="fab fa-facebook-f"></i>
                صفحتنا على فيسبوك
            </a>

            <!-- رابط حساب انستغرام المحدث -->
            <a href="https://www.instagram.com/libre_vent/" target="_blank" class="link-btn instagram">
                <i class="fab fa-instagram"></i>
                حسابنا على انستغرام
            </a>

            <!-- زر البريد الإلكتروني -->
            <a href="mailto:generation.numerical.38@gmail.com" class="link-btn gmail">
                <i class="fas fa-envelope"></i>
                ارسل لنا بريداً إلكترونياً
            </a>

        </div>
    </div>

</body>
</html
  <img width="1024" height="1024" alt="W9IZETy - Imgur" src="https://github.com/user-attachments/assets/41bcadbe-8d5f-4f4d-981e-792bd288beec" />
