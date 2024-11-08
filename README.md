<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>حاسبة تكاليف إيجار النقل البري</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            direction: rtl;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }
        .header {
            background-color: #003366;
            color: white;
            padding: 15px;
            text-align: center;
        }
        .container {
            display: flex;
            justify-content: space-around;
            margin: 20px;
            padding: 20px;
            background-color: #ffffff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .form-section {
            width: 45%;
        }
        .form-section h3 {
            margin-bottom: 15px;
            color: #003366;
        }
        .input-group {
            margin-bottom: 15px;
        }
        .input-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
        .input-group input, .input-group select {
            width: 100%;
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            padding: 10px 20px;
            background-color: #003366;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
        }
        button:hover {
            background-color: #002244;
        }
        .results {
            margin-top: 20px;
            padding: 10px;
            background-color: #e0f7fa;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>حاسبة تكاليف إيجار النقل البري</h1>
    </div>
    <div class="container">
        <div class="form-section">
            <h3>إدخال البيانات</h3>
            <div class="input-group">
                <label for="truckType">نوع الشاحنة:</label>
                <select id="truckType">
                    <option value="open_truck">شاحنة مفتوحة</option>
                    <option value="closed_truck">شاحنة مغلقة</option>
                    <option value="refrigerated_truck">شاحنة مبردة</option>
                    <option value="frozen_truck">شاحنة مجمدة</option>
                </select>
            </div>
            <div class="input-group">
                <label for="truckSize">حجم الشاحنة:</label>
                <select id="truckSize">
                    <option value="5M">5M</option>
                    <option value="6M">6M</option>
                    <option value="7M">7M</option>
                </select>
            </div>
            <div class="input-group">
                <label for="rentalType">نوع الإيجار:</label>
                <select id="rentalType">
                    <option value="half_month">نصف شهري</option>
                    <option value="monthly">شهري</option>
                </select>
            </div>
            <div class="input-group">
                <label for="dailyKm">الكيلومترات اليومية:</label>
                <input type="number" id="dailyKm" placeholder="أدخل الكيلومترات">
            </div>
            <div class="input-group">
                <label for="dailyHours">عدد الساعات اليومية:</label>
                <input type="number" id="dailyHours" placeholder="أدخل عدد الساعات">
            </div>
            <button onclick="calculateCost()">احسب</button>
            <div class="results" id="results"></div>
        </div>
    </div>

    <script>
        function calculateCost() {
            // هنا يتم تضمين منطق حساب التكلفة مثل الكود السابق
            // سيتم استخدام القيم المدخلة لحساب التكلفة وعرض النتائج
            document.getElementById('results').innerHTML = `
                <p>إجمالي التكلفة: <strong>مثال على تكلفة إجمالية</strong> ريال</p>
            `;
        }
    </script>
</body>
</html>
