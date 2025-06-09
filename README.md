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
<!-- Add this inside the body tag after the header -->
<section class="financial-overview">
    <div class="card">
        <h2>Total Account Balance</h2>
        <p>$10,000</p>
    </div>
    <div class="card">
        <h2>Monthly Income</h2>
        <p>$5,000</p>
    </div>
    <div class="card">
        <h2>Monthly Expenses</h2>
        <p>$3,000</p>
    </div>
    <div class="card">
        <h2>Savings Ratio</h2>
        <p>60%</p>
    </div>
</section>
// script.js
const ctx = document.getElementById('myChart').getContext('2d');
const myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Red', 'Blue', 'Yellow', 'Green', 'Purple', 'Orange'],
        datasets: [{
            label: '# of Votes',
            data: [12, 19, 3, 5, 2, 3],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            y: {
                beginAtZero: true
            }
        }
    }
});
