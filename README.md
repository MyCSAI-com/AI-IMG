<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Server Busy Notification</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f8d7da; /* Light red background */
            color: #721c24; /* Dark red text color */
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh; /* Full viewport height */
        }
        .notification-container {
            background-color: #f8d7da; /* Light red background */
            border: 2px solid #dc3545; /* Red border */
            border-radius: 10px; /* Rounded corners */
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Shadow effect */
            padding: 20px; /* Padding */
            text-align: center;
            max-width: 500px; /* Max width */
            margin: 20px; /* Margin */
        }
        .notification-message h1 {
            color: #dc3545; /* Red color for heading */
            font-size: 24px; /* Font size */
        }
        .notification-message p {
            font-size: 16px; /* Font size */
            margin: 10px 0; /* Margin */
        }
        .try-again-btn {
            background-color: #dc3545; /* Red button */
            color: #fff; /* White text */
            border: none; /* No border */
            border-radius: 5px; /* Rounded corners */
            padding: 10px 20px; /* Padding */
            cursor: pointer; /* Pointer cursor */
            font-size: 16px; /* Font size */
            margin-top: 10px; /* Margin */
        }
        .try-again-btn:hover {
            background-color: #c82333; /* Darker red on hover */
        }
    </style>
</head>
<body>
    <div class="notification-container">
        <div class="notification-message">
            <h1>⚠️ Server Busy</h1>
            <p>The server is currently busy due to high user activity. Please try again later. Thank you for your patience!</p>
            <button class="try-again-btn" onclick="retryAction()">Try Again</button>
        </div>
    </div>
    <script>
        function retryAction() {
            alert("Retrying..."); // Simulate retry action
            // Here you can add logic to retry the action, e.g., making a network request
        }
    </script>
</body>
</html>
