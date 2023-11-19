# beequippeds.github.io
!DOCTYPE html>
<html lang="de">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>eBike Buchungsplattform</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f0f0f0;
        }

        header {
            text-align: center;
            padding: 10px;
            background-color: #333;
            color: white;
        }

        form {
            max-width: 400px;
            margin: 0 auto;
        }

        .bike-container {
            margin-bottom: 20px;
        }

        .bike-header {
            font-style: italic;
            font-weight: bold;
            color: violet;
        }

        label {
            color: violet; /* Lila Textfarbe für Labels */
        }

        .black-label {
            color: black; /* Schwarze Textfarbe für das Buchen-Label */
        }

        hr {
            border: 1px solid violet; /* Lila Linie */
        }

        footer {
            text-align: center;
            padding: 10px;
            background-color: #333;
            color: white;
        }
    </style>
</head>

<body>
    <header>
        <h1>eBike Buchung</h1>
    </header>

    <form action="booking.php" method="post">
        <label for="hotel_username">Hotel Benutzername:</label>
        <input type="text" id="hotel_username" name="hotel_username" required><br>

        <label for="hotel_password">Hotel Kennwort:</label>
        <input type="password" id="hotel_password" name="hotel_password" required><br>

        <hr>

        <div class="bike-container">
            <h2 class="bike-header">Mountain eBike</h2>
            <label for="mountain_bike_quantity">Anzahl der Mountain eBikes:</label>
            <input type="number" id="mountain_bike_quantity" name="mountain_bike_quantity" min="1" required><br>
        </div>

        <div class="bike-container">
            <h2 class="bike-header">City eBike</h2>
            <label for="city_bike_quantity">Anzahl der City eBikes:</label>
            <input type="number" id="city_bike_quantity" name="city_bike_quantity" min="1" required><br>
        </div>

        <div class="bike-container">
            <h2 class="bike-header">Touring eBike</h2>
            <label for="touring_bike_quantity">Anzahl der Touring eBikes:</label>
            <input type="number" id="touring_bike_quantity" name="touring_bike_quantity" min="1" required><br>
        </div>

        <label for="rental_days">Miettage:</label>
        <input type="number" id="rental_days" name="rental_days" min="1" required><br>

        <label class="black-label" for="booking">Buchen:</label>
        <input type="submit" value="Buchen">
    </form>

    <footer>
        <p>&copy; 2023 eBike Buchungsplattform. Alle Rechte vorbehalten.</p>
    </footer>
</body>

</html>
