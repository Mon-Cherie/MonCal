<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mon Cheri Calculator</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            text-align: center;
            margin: 50px;
            background-color: #ffe6f2; /* Pink pastel background */
            color: #ff1a75; /* Dark pink text */
        }

        h2 {
            color: #ff66b2; /* Darker pink for headings */
        }

        p {
            font-size: 14px;
            color: #ff1a75; /* Dark pink text */
        }

        form {
            background-color: #ffd9e6; /* Light pink form background */
            padding: 20px;
            border-radius: 10px;
            display: inline-block;
            margin-top: 20px;
        }

        label, select, button {
            margin: 10px;
            font-size: 16px;
        }

        #result {
            margin-top: 20px;
            font-weight: bold;
        }

        .footer {
            font-size: 12px;
            margin-top: 30px;
        }
    </style>
</head>
<body>
    <h2>Mon Cheri Calculator</h2>
    <p>This Calculator is run by @PlatoNeeds on Twitter</p>
    
    <form id="calculatorForm">
        <label for="jenisItems">Jenis Items:</label>
        <select id="jenisItems" required>
            <option value="9">Items Shop</option>
            <option value="12">Items Rare (Harga 100-5000 coins)</option>
            <option value="13">Items Rare (Harga 5500-10000 coins)</option>
        </select>
        
        <label for="hargaItems">Harga Items:</label>
        <select id="hargaItems" required>
            <!-- Opsi harga items -->
            <!-- Anda dapat menambahkan lebih banyak opsi sesuai kebutuhan -->
            <option value="50">50 coins</option>
            <option value="100">100 coins</option>
            <option value="200">200 coins</option>
            <option value="250">250 coins</option>
            <option value="500">500 coins</option>
            <option value="750">750 coins</option>
            <option value="1000">1000 coins</option>
            <option value="1250">1250 coins</option>
            <option value="1500">1500 coins</option>
            <option value="1750">1750 coins</option>
            <option value="2000">2000 coins</option>
            <option value="2500">2500 coins</option>
            <option value="2750">2750 coins</option>
            <option value="3000">3000 coins</option>
            <option value="3500">3500 coins</option>
            <option value="4000">4000 coins</option>
            <option value="4500">4500 coins</option>
            <option value="5000">5000 coins</option>
            <option value="5500">5500 coins</option>
            <!-- Dan seterusnya sesuai kelipatan 500 hingga 20000 -->
            <option value="6000">6000 coins</option>
            <option value="6500">6500 coins</option>
            <option value="7000">7000 coins</option>
            <option value="7500">7500 coins</option>
            <option value="8000">8000 coins</option>
            <option value="8500">8500 coins</option>
            <option value="9000">9000 coins</option>
            <option value="9500">9500 coins</option>
            <option value="10000">10000 coins</option>
            <option value="10500">10500 coins</option>
            <option value="11000">11000 coins</option>
            <option value="11500">11500 coins</option>
            <option value="12000">12000 coins</option>
            <option value="12500">12500 coins</option>
            <option value="13000">13000 coins</option>
            <option value="13500">13500 coins</option>
            <option value="14000">14000 coins</option>
            <option value="14500">14500 coins</option>
            <option value="15000">15000 coins</option>
            <option value="15500">15500 coins</option>
            <option value="16000">16000 coins</option>
            <option value="16500">16500 coins</option>
            <option value="17000">17000 coins</option>
            <option value="17500">17500 coins</option>
            <option value="18000">18000 coins</option>
            <option value="18500">18500 coins</option>
            <option value="19000">19000 coins</option>
            <option value="19500">19500 coins</option>
            <option value="20000">20000 coins</option>
        </select>
        
        <button type="button" onclick="calculateTotal()">Hitung Total</button>
    </form>

    <div id="result"></div>

    <p>Kalkulator ini digunakan untuk memeriksa harga items Plato yang ingin customers beli. Jika ingin mengecek nama dan harga items lebih detail, bisa cek melalui web <a href="https://platopedia.com/items" target="_blank">platopedia.com/items</a> lalu jumlahkan di web ini.</p>
    <p class="footer">Last Update: 24/02/2024 | @PlatoNeeds</p>

    <script>
        // Fungsi untuk menghitung total dan menampilkan hasil
        function calculateTotal() {
            var jenisItems = parseInt(document.getElementById("jenisItems").value);
            var hargaItems = parseInt(document.getElementById("hargaItems").value);
            var totalHarga;

            // Menggunakan rumus sesuai dengan jenis items yang dipilih
            if (jenisItems === 9) {
                totalHarga = jenisItems * hargaItems;
            } else if (jenisItems === 12) {
                totalHarga = jenisItems * hargaItems;
            } else if (jenisItems === 13) {
                totalHarga = jenisItems * hargaItems;
            }

            // Tampilkan hasil
            var resultDiv = document.getElementById("result");
            resultDiv.textContent = `Total Harga: Rp${totalHarga.toLocaleString()}`;
        }
    </script>
</body>
</html>
