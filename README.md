<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Bootstrap demo</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet" 
    integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
    <style>
      /* Style the tab */
      .tab {
        overflow: hidden;
        /* border: 1px solid #ccc; */
        background-color: #f1f1f1;
        width: 540px;
      }

      /* Style the buttons inside the tab */
      .tab button {
        background-color: inherit;
        float: left;
        border: none;
        outline: none;
        cursor: pointer;
        margin-left: 15px;
        padding: 12px ;
        transition: 0.3s;
        font-size: 17px;
      }

      /* Change background color of buttons on hover */
      .tab button:hover {
        background-color: #ddd;
      }

      /* Create an active/current tablink class */
      .tab button.active {
        background-color: #ccc;
      }

      /* Style the tab content */
      .tabcontent {
        display: none;
        padding: 6px 12px;
        -webkit-animation: fadeEffect 1s;
        animation: fadeEffect 1s;
      }

      /* Fade in tabs */
      @-webkit-keyframes fadeEffect {
        from {opacity: 0;}
        to {opacity: 1;}
      }

      @keyframes fadeEffect {
        from {opacity: 0;}
        to {opacity: 1;}
      }

      #card {
        -webkit-animation: mover 2s infinite  alternate;
        animation: mover 2s infinite  alternate;
      }
      @-webkit-keyframes mover {
          0% { transform: translateY(0); }
          100% { transform: translateY(-20px); }
      }
      @keyframes mover {
          0% { transform: translateY(0); }
          100% { transform: translateY(-20px); }
      }
    </style>
  </head>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#" style="margin-left: 10px; font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">PEMROGRAMAN WEB</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="UTS_CV_Glisela.html">My CV<span class="sr-only">(current)</span></a>
        </li>
      </ul>
    </div>
  </nav>
  <body>
    <div style="background-image: url('Background.jpg'); height: 500px; position: relative;">
      <div class="card" id="card" style="width: 1000px; height: 550px; margin: 100px 150px 50px 180px; position: absolute;">
        <div style="margin: 20px 50px 20px 100px;">
          <br>  
          <div class="row">
            <img src="paper-clip.png" style="width: 10%; position: absolute; margin-left: -90px; margin-top: -30px;">
            <div class="col-lg-4">
              <img src="foto.jpg" style="width: 100%;" class="rounded-circle">
              <div style="margin-left: 65px;">
                <br>
                <a class="btn btn-danger" href="https://www.instagram.com/ales2806_12/?next=%2F&hl=id" target="_blank" role="button"><i class="fa fa-instagram" aria-hidden="true"></i></a>
                <a class="btn btn-success" href="https://api.whatsapp.com/send?phone=6283112112944&text=Chat%20Saya!" target="_blank" role="button"><i class="fa fa-whatsapp" aria-hidden="true"></i></a>
                <a class="btn btn-primary" href="https://mail.google.com/mail/u/0/?view=cm&tf=1&fs=1&to=gliseladilap@gmail.com" target="_blank" role="button"><i class="fa fa-envelope-o" aria-hidden="true"></i></a>
              </div>
            </div>
            <div class="col-lg-8" >
              <button type="button" class="btn btn-primary">MY CV</button>
              <br><br>
              <h4 style="font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;"> GLISELA DILA PRIATNA</h4>
              <h6 style="font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;"> Mahasiswa Universitas Nurtanio Bandung</h6>
              <br>
              <div class="tab">
                <button class="tablinks" onclick="openCity(event, 'Saya')" id="defaultOpen">Tentang Saya</button>
                <button class="tablinks" onclick="openCity(event, 'Pengalaman')">Pengalaman</button>
                <button class="tablinks" onclick="openCity(event, 'Pendidikan')">Pendidikan</button>
                <button class="tablinks" onclick="openCity(event, 'Keterampilan')">Keterampilan</button>
              </div>

              <div id="Saya" class="tabcontent active">
                <br>
                <p class="card-text"><b>Nama</b>: Glisela Dila Priatna</p>
                <p class="card-text"><b>Tempat, Tanggal Lahir</b> : Bandung, 16 Agustus 2003</p>
                <p class="card-text"><b>Alamat </b>: Jln. Maleber Utara GG Bhakti 6 RT 03 RW 08 Kecamatan Andir Kelurahan Maleber </p>
                <p class="card-text"><b>Jenis Kelamin </b>: Perempuan</p>
                <p class="card-text"><b>Kewarganegaraan </b>: WNI</p>
              </div>

              <div id="Pengalaman" class="tabcontent">
                <br>
                <p class="card-text"><b>Pengalaman Bekerja</b></p>
                <p class="card-text">Carry Salon <br> April - Mei 2020</p>
                <p class="card-text"><b>Pengalaman Berorganisasi</b></p>
                <p class="card-text">Organisasi Pramuka</p>
                <p class="card-text">Organisasi BEM FIKI UNNUR</p>
              </div>
              
              <div id="Pendidikan" class="tabcontent">
                <br>
                <p class="card-text"> <b>SDN Karang Taruna 1</b><br> (2012 - 2017)</p>
                <p class="card-text"> <b>SMPN 41 Bandung</b><br> (2017- 2019)</p>
                <p class="card-text"><b>SMK Kimia Dharma Bhakti Bandung </b><br> (2019 - 2021)</p>
                <p class="card-text"><b>Universitas Nurtanio Bandung </b><br> (2021 - Sekarang) </p>
              </div>

              <div id="Keterampilan" class="tabcontent">
                <br>
                <p class="card-text"> <b>Analisis Data </b><br> Mampu Membuat Flowchart, algoritma dengan metode deskripsi.</p>
                <p class="card-text"> <b>Pembelajaran </b><br> Pernah belajar CPP, C#, dan HTML</p>
                <p class="card-text"> <b>Menulis </b><br> Dapat menulis sebuah cerita.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <br><br><br><br><br><br><br><br><br><br>
  <script>
    function openCity(evt, cityName) {
      var i, tabcontent, tablinks;
      tabcontent = document.getElementsByClassName("tabcontent");
      for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
      }
      tablinks = document.getElementsByClassName("tablinks");
      for (i = 0; i < tablinks.length; i++) {
        tablinks[i].className = tablinks[i].className.replace(" active", "");
      }
      document.getElementById(cityName).style.display = "block";
      evt.currentTarget.className += " active";
    }
    document.getElementById("defaultOpen").click();
    </script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js" 
    integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe" crossorigin="anonymous"></script>
</body>
</html>
