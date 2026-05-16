<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>نموذج تسجيل البيانات</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f7f6;
            margin: 0;
            padding: 20px;
        }
        .form-container {
            max-width: 600px;
            background: #ffffff;
            margin: 0 auto;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }
        h2 {
            text-align: center;
            color: #333;
            margin-bottom: 25px;
        }
        .form-group {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #555;
        }
        input[type="text"],
        input[type="email"],
        input[type="number"],
        input[type="url"],
        select,
        textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 14px;
        }
        button {
            width: 100%;
            padding: 12px;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
            font-weight: bold;
        }
        button:hover {
            background-color: #218838;
        }
    </style>
</head>
<body>

<div class="form-container">
    <h2>نموذج تسجيل البيانات</h2>
    
    <form action="https://formspree.io/f/mqenrgba" method="POST">
        
        <div class="form-group">
            <label for="fullname">الاسم الكامل:</label>
            <input type="text" id="fullname" name="Full_Name" required placeholder="أدخل الاسم الثلاثي أو الرباعي">
        </div>

        <div class="form-group">
            <label for="email">البريد الإلكتروني للاتصال:</label>
            <input type="email" id="email" name="Email_Address" required placeholder="example@email.com">
        </div>

        <div class="form-group">
            <label for="image_url">رابط الصورة الشخصية أو الهوية (رابط مباشر):</label>
            <input type="url" id="image_url" name="Identity_Image_URL" placeholder="https://example.com/image.jpg">
        </div>

        <div class="form-group">
            <label for="id_number">رقم الهوية / جواز السفر:</label>
            <input type="number" id="id_number" name="ID_or_Passport_Number" required placeholder="أدخل الرقم الوطني أو رقم الجواز">
        </div>

        <div class="form-group">
            <label for="main_phone">رقم الهاتف الرئيسي:</label>
            <input type="number" id="main_phone" name="Primary_Phone" required placeholder="05xxxxxxxx">
        </div>

        <div class="form-group">
            <label for="alt_phone">رقم هاتف بديل / واتساب:</label>
            <input type="number" id="alt_phone" name="Whatsapp_Phone" placeholder="05xxxxxxxx">
        </div>

        <div class="form-group">
            <label for="address">مكان الإقامة الحالي / العنوان الحالي بالتفصيل:</label>
            <textarea id="address" name="Detailed_Address" rows="3" required placeholder="المدينة، الحي، الشارع، المعالم القريبة..."></textarea>
        </div>

        <div class="form-group">
            <label for="family_members">عدد أفراد الأسرة:</label>
            <input type="number" id="family_members" name="Family_Members_Count" min="1" required placeholder="أدخل عدد الأفراد">
        </div>

        <div class="form-group">
            <label for="family_status">حالة الأسرة:</label>
            <select id="family_status" name="Family_Condition" required>
                <option value="" disabled selected>اختر الحالة من القائمة...</option>
                <option value="نازح">نازح</option>
                <option value="أسرة شهيد">أسرة شهيد</option>
                <option value="حالة مرضية">حالة مرضية</option>
                <option value="تعطل عن العمل">تعطل عن العمل</option>
                <option value="أخرى">وضع مستقر / أخرى</option>
            </select>
        </div>

        <button type="submit">إرسال البيانات</button>
        
    </form>
</div>

</body>
</html>
