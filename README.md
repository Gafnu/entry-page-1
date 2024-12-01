# entry-page-1<html>
<head><title>GAFNU@</title>
<meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <script>
        function checkLogin() {
            // Get values from the form
            const userID = document.getElementById("userID").value;
            const password = document.getElementById("password").value;

            // Hardcoded ID and password for demo
            if (userID === "student10" && password === "class10") {
                // Redirect to another page
                window.location.href = "welcome.html";
            } else {
                alert("Invalid ID or Password! Try again.");
            }
        }
    </script>
</head>
<body>
    <h2>Login Page</h2>
    <form onsubmit="checkLogin(); return false;">
        <!-- User ID Input -->
        <label for="userID">User ID:</label><br>
        <input type="text" id="userID" name="userID" required><br><br>

        <!-- Password Input -->
        <label for="password">Password:</label><br>
        <input type="password" id="password" name="password" required><br><br>

        <!-- Submit Button -->
        <button type="submit">Login</button>
    </form>
</body>
</html>


