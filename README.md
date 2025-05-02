!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mahsulot Do‘koni</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #000000;
            color: #FFFF00;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #4B0082;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            margin: 0;
            color: #FFFF00;
        }
        main {
            padding: 20px;
        }
        .product {
            background-color: #4B0082;
            margin: 10px 0;
            padding: 15px;
            border-radius: 8px;
        }
        form {
            background-color: #4B0082;
            padding: 20px;
            border-radius: 8px;
            margin-top: 20px;
        }
        form input, form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 4px;
        }
        form button {
            background-color: #FFFF00;
            color: #000000;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <h1>Mahsulot Do‘koni</h1>
    </header>

    <main>
        <section class="products">
            <div class="product">
                <h2>Mahsulot 1</h2>
                <p>Bu yerda mahsulot haqida qisqacha ma'lumot yoziladi.</p>
            </div>
            <div class="product">
                <h2>Mahsulot 2</h2>
                <p>Bu yerda mahsulot haqida qisqacha ma'lumot yoziladi.</p>
            </div>
        </section>

        <section class="feedback">
            <h2>Taklif va surat yuboring</h2>
            <form>
                <input type="text" placeholder="Ismingiz" required>
                <input type="email" placeholder="Email manzilingiz" required>
                <textarea placeholder="Taklifingizni yozing" required></textarea>
                <input type="file" accept="image/*" required>
                <button type="submit">Yuborish</button>
            </form>
        </section>
    </main>

    <script>
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Rahmat! Taklifingiz va suratingiz qabul qilindi.');
        });
    </script>
</body>
</html>
