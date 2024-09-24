<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Server Busy Notification</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>
    <div id="loadingMessage">
        <h1>Loading...</h1>
    </div>
    <div id="notification" class="hidden">
        <h1 style="color: red;">⚠️ Server Busy</h1>
        <p style="color: red;">
            The server is currently busy due to high user activity. Please try again later. Thank you for your patience!
        </p>
        <button style="background-color: red; color: white; border: none; padding: 10px; cursor: pointer;">
            Try Again
        </button>
    </div>
    <script>
        // Wait for 100 seconds (100000 milliseconds) before showing the notification
        setTimeout(() => {
            document.getElementById('loadingMessage').classList.add('hidden'); // Hide loading message
            document.getElementById('notification').classList.remove('hidden'); // Show notification
        }, 100000); // 100 seconds
    </script>
</body>
</html>
