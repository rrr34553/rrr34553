<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Digital Profile - Raiyan Shike</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #6a11cb, #2575fc);
      color: #fff;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .profile-card {
      background: #ffffff;
      color: #333;
      border-radius: 10px;
      padding: 20px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      text-align: center;
      width: 300px;
    }
    .profile-card h1 {
      font-size: 24px;
      margin-bottom: 10px;
    }
    .profile-card p {
      margin: 5px 0;
    }
    .qr-code {
      margin-top: 20px;
    }
    a {
      text-decoration: none;
      color: #2575fc;
    }
  </style>
</head>
<body>
  <div class="profile-card">
    <h1>Raiyan Shike</h1>
    <p><strong>Tagline:</strong> Digital Creator</p>
    <p><strong>Phone:</strong> <a href="tel:01838070990">01838070990</a></p>
    <p><strong>Location:</strong> Narayanganj</p>
    <div class="qr-code" id="qrcode"></div>
    <p><a href="https://www.facebook.com/raiyan.sheak.2024?mibextid=ZbWKwL" target="_blank">Visit Facebook</a></p>
    <p><a href="https://www.tiktok.com/@raiyan.sk4?_t=ZS-8sBJLnUWjBg&_r=1" target="_blank">Visit TikTok</a></p>
    <p><a href="https://www.instagram.com/raiyansheak?igsh=YzljYTk1ODg3Zg==" target="_blank">Visit Instagram</a></p>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/qrcode/build/qrcode.min.js"></script>
  <script>
    const qrCodeContainer = document.getElementById('qrcode');
    QRCode.toCanvas(qrCodeContainer, 'https://www.facebook.com/raiyan.sheak.2024?mibextid=ZbWKwL', {
      width: 150,
      color: {
        dark: '#000000', // QR code color
        light: '#ffffff' // Background color
      }
    }, function (error) {
      if (error) console.error(error);
    });
  </script>
</body>
</html>
