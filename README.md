
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <style>
           body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background: url('AZ.jpg'); /* Replace 'background-image.jpg' with the path to your background image */
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .login-container {
            background: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            width: 300px;
        }

        .login-container h2 {
            text-align: center;
        }

        .login-form {
            display: flex;
            flex-direction: column;
        }

        .form-group {
            margin-bottom: 15px;
        }

        .form-group label {
            font-weight: bold;
            margin-bottom: 5px;
        }

        .form-group input {
            padding: 8px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        .form-group input[type="submit"] {
            background-color: #4caf50;
            color: white;
            cursor: pointer;
        }
		/* Styles remain unchanged from the previous example */
    </style>
    <script>
        function validateForm() {
            var username = document.getElementById('username').value;
            var password = document.getElementById('password').value;

            // Check if the entered username and password are correct (replace with your logic)
            if (username === 'qqqq' && password === '1111') {
                // Redirect to the Google Form
                window.location.href = 'https://docs.google.com/forms/d/e/1FAIpQLSfM8YT93X9cnZLGUBLvce7wsjwddmlEWFjTXix8zGaxXD6X_w/viewform?usp=sf_link'; 
                return false; // Prevent form submission
            } else {
                alert('Incorrect username or password. Please try again.');
                return false; // Prevent form submission
            }
        }
    </script>
</head>
<body>

<div class="login-container">
    <h2>Login</h2>
    <form class="login-form" action="#" method="post" onsubmit="return validateForm()">
        <div class="form-group">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username" placeholder="Enter your username">
        </div>

        <div class="form-group">
            <label for="password">Password:</label>
            <input type="password" id="password" name="password" placeholder="Enter your password">
        </div>

        <div class="form-group">
            <input type="submit" value="Login">
        </div>
    </form>
</div>

</body>
</html>
