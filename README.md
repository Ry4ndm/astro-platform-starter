<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Properti Bali - Semi-Villa Dijual</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f9f9f9;
      color: #333;
    }

    header {
      background: url('https://via.placeholder.com/1200x600') no-repeat center center/cover;
      color: white;
      text-align: center;
      padding: 150px 20px;
      background-size: cover;
    }

    header h1 {
      font-size: 48px;
      margin: 0;
    }

    header p {
      font-size: 20px;
      margin: 10px 0;
    }

    section {
      padding: 40px 20px;
      max-width: 1200px;
      margin: auto;
    }

    .property-info {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
    }

    .property-info img {
      width: 100%;
      max-width: 600px;
      border-radius: 10px;
    }

    .property-details {
      flex: 1;
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }

    .property-details h2 {
      font-size: 30px;
      color: #333;
    }

    .property-details p {
      font-size: 18px;
      line-height: 1.6;
    }

    #map {
      width: 100%;
      height: 400px;
      border: 1px solid #ddd;
      margin-top: 40px;
      border-radius: 10px;
    }

    .contact {
      background: #f5f5f5;
      padding: 40px 20px;
      text-align: center;
    }

    .contact h3 {
      font-size: 30px;
      color: #333;
    }

    .contact p {
      font-size: 18px;
    }

    .contact a {
      background: #25d366;
      color: white;
      padding: 12px 24px;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <!-- Header dengan Gambar Properti -->
  <header>
    <h1>Semi-Villa Dijual di Bali</h1>
    <p>Temukan rumah impian Anda di pulau dewata</p>
  </header>

  <!-- Deskripsi Properti -->
  <section>
    <div class="property-info">
      <!-- Gambar Properti -->
      <img src="https://via.placeholder.com/600x400" alt="Semi-Villa di Bali" />

      <!-- Detail Properti -->
      <div class="property-details">
        <h2>Semi-Villa Mewah – Ubud, Bali</h2>
        <p><strong>Harga:</strong> Rp 1.500.000.000</p>
        <p><strong>Luas Tanah:</strong> 350 m²</p>
        <p><strong>Kamar Tidur:</strong> 3</p>
        <p><strong>Kamar Mandi:</strong> 2</p>
        <p><strong>Fasilitas:</strong> Kolam Renang, Taman, Akses Jalan Raya</p>
        <p><strong>Lokasi:</strong> Ubud, Bali – Dekat dengan tempat wisata terkenal.</p>
      </div>
    </div>
  </section>

  <!-- Peta Lokasi Properti -->
  <section>
    <h2>Lokasi Properti</h2>
    <div id="map"></div>
  </section>

  <!-- Kontak -->
  <section class="contact">
    <h3>Hubungi Kami</h3>
    <p>Untuk informasi lebih lanjut atau untuk jadwalkan kunjungan, hubungi kami melalui:</p>
    <a href="https://wa.me/6281234567890" target="_blank">Chat WhatsApp</a>
  </section>

  <!-- Script untuk Google Map -->
  <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap" async defer></script>
  <script>
    function initMap() {
      var location = { lat: -8.506, lng: 115.261 }; // Ganti dengan lokasi yang sesuai
      var map = new google.maps.Map(document.getElementById('map'), {
        zoom: 15,
        center: location
      });
      var marker = new google.maps.Marker({
        position: location,
        map: map,
        title: 'Semi-Villa di Ubud, Bali'
      });
    }
  </script>

</body>
</html>