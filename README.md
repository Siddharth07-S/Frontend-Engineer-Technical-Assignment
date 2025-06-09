# Header & Profile Section
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Finance App</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="profile">
            <img src="profile-picture.jpg" alt="Profile Picture">
            <span>Welcome, User!</span>
        </div>
        <div class="savings-goal">
            <progress value="50" max="100"></progress>
            <span>Savings Goal: 50%</span>
        </div>
    </header>
    <!-- Other sections will go here -->
    <script src="script.js"></script>
</body>
</html>
/* styles.css */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #007bff;
    color: white;
    padding: 1em;
    text-align: center;
}

.profile img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
}

.savings-goal progress {
    width: 100%;
    height: 10px;
}
