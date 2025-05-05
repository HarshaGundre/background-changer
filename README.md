<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Light On/Off Effect</title>
    <style>
        body {
            text-align: center;
            padding: 200px;
            transition: background 0.5s ease;
            background-repeat: no-repeat;
            background-position: center;
        }
        button {
            padding: 10px 20px;
            font-size: 16px;
            position: fixed;
            bottom: 20px;
            left: 50%;
        }
    </style>
</head>
<body>

    <button onclick="toggleLight()">Toggle Light</button>

    <script>
        const lightOn = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ4C30I8dqiGpXUkVdnlwOXIwRK3ntJbmhBQg&s"; 
        const lightOff = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQuC6Ba6FDwQ3CUC91G1XTYYvs9SED1W0zLAw&s"; 
        let isLightOn = false;

        function toggleLight() {
            isLightOn = !isLightOn;
            document.body.style.backgroundImage = isLightOn ? `url('${lightOn}')` : `url('${lightOff}')`;
        }
    </script>

</body>
</html>
