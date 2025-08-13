<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <h2>Kalkulator Sederhana</h2>
    <input type="number" id="angka1" placeholder="Angka 1">
    <select id="operator">
        <option value="+">+</option>
        <option value="-">-</option>
        <option value="*">*</option>
        <option value="/">/</option>
    </select>
    <input type="number" id="angka2" placeholder="Angka 2">
    <button onclick="hitung()">Hitung</button>
    <p>Hasil: <span id="hasil"></span></p>

    <script>
    function hitung() {
        var angka1 = Number(document.getElementById('angka1').value);
        var angka2 = Number(document.getElementById('angka2').value);
        var operator = document.getElementById('operator').value;
        var hasil;

        if (operator == "+") {
            hasil = angka1 + angka2
         } else if (operator == "-") {
            hasil = angka1 - angka2
        } else if (operator == "*") {
            hasil = angka1 * angka2
        } else if (operator == "/") {
             hasil = angka1 / angka2
        }
        document.getElementById('hasil').innerText = hasil;
    }
    </script>
</body>
</html>
