<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>车主信息</title>
    <style>
        /* 全局样式 */
        body {
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #6e7c8a, #b8c9d3);
            margin: 0;
            padding: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .container {
            width: 100%;
            max-width: 450px;
            background-color: #fff;
            padding: 25px;
            border-radius: 15px;
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
        }

        h2 {
            color: #333;
            font-size: 26px;
            margin-bottom: 20px;
        }

        .info {
            margin: 15px 0;
            text-align: left;
        }

        .info label {
            font-weight: 600;
            color: #444;
            font-size: 16px;
            margin-bottom: 5px;
        }

        .info span {
            font-size: 18px;
            color: #555;
            display: block;
        }

        /* 按钮样式 */
        .btn {
            display: inline-block;
            width: 100%;
            max-width: 250px; /* 限制按钮的最大宽度 */
            padding: 15px;
            background-color: #4CAF50;
            color: white;
            font-size: 18px;
            font-weight: bold;
            text-decoration: none;
            border-radius: 10px;
            transition: background-color 0.3s, transform 0.2s ease-in-out;
            margin: 20px auto 0 auto; /* 使用 margin: auto 实现居中 */
        }

        .btn:hover {
            background-color: #45a049;
            transform: translateY(-2px);
        }

        /* 响应式样式 */
        @media (max-width: 600px) {
            body {
                padding: 10px;
            }
            .container {
                padding: 20px;
                width: 90%;
            }
            h2 {
                font-size: 22px;
            }
            .info span {
                font-size: 16px;
            }
            .btn {
                font-size: 16px;
                padding: 12px;
                max-width: 100%; /* 在手机端确保按钮宽度占满 */
            }
        }
    </style>
</head>
<body>

    <div class="container">
        <h2>车主信息</h2>

        <div class="info">
            <label for="licensePlate">车牌号:</label>
            <span id="licensePlate">粤A12345</span>
        </div>

        <div class="info">
            <label for="phoneNumber">车主电话:</label>
            <span id="phoneNumber">13812345678</span>
        </div>

        <div class="info">
            <label for="customText">自定义文字:</label>
            <span id="customText">请在需要时与车主联系。</span>
        </div>

        <a href="tel:13812345678" class="btn">一键拨打电话</a>
    </div>

</body>
</html>
