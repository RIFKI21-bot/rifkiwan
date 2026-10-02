<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CV Rai Haidar Muhadzib</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    background: #e9e9e9;
    font-family: Arial, Helvetica, sans-serif;
    color: #41444b;
}

/* =========================
   HALAMAN CV
========================= */

.cv {
    position: relative;
    width: 1000px;
    min-height: 1414px;
    margin: 30px auto;
    padding: 130px 100px 100px;
    background: #fff;
    overflow: hidden;
}

/* =========================
   DEKORASI ATAS
========================= */

.top-gold {
    position: absolute;
    width: 550px;
    height: 130px;
    right: 0;
    top: 0;
    background: #c9aa61;
    clip-path: polygon(20% 0,100% 0,100% 100%);
}

.top-dark {
    position: absolute;
    width: 370px;
    height: 130px;
    right: 0;
    top: 0;
    background: #293344;
    clip-path: polygon(58% 0,100% 0,100% 100%);
}

.top-light {
    position: absolute;
    width: 250px;
    height: 95px;
    right: 90px;
    top: 0;
    background: #e0c77f;
    clip-path: polygon(0 0,100% 0,100% 100%);
}

/* =========================
   TITIK-TITIK ATAS
========================= */

.dots-top {
    position: absolute;
    left: 40px;
    top: 27px;
    width: 420px;
    height: 60px;
}

.dots-top span,
.dots-right span {
    display: inline-block;
    width: 8px;
    height: 8px;
    margin-right: 30px;
    margin-bottom: 25px;
    background: #303030;
    border-radius: 50%;
}

/* =========================
   HEADER
========================= */

.header {
    position: relative;
    z-index: 5;

    display: flex;
    align-items: center;

    gap: 45px;
    margin-bottom: 48px;
}

.foto {
    width: 205px;
    height: 210px;

    object-fit: cover;

    border-radius: 30px;
    border: 4px solid #c8a75d;
}

.nama {
    flex: 1;
}

.nama h1 {
    font-size: 43px;
    font-weight: 400;
    color: #35383f;
    letter-spacing: 1px;
    white-space: nowrap;
    margin-bottom: 27px;
}

.kontak {
    font-size: 17px;
    line-height: 1.8;
}

.kontak div {
    display: flex;
    align-items: center;
}

/* =========================
   SECTION
========================= */

.section {
    position: relative;
    z-index: 5;
    margin-bottom: 22px;
}

.judul {
    width: 405px;
    height: 60px;

    display: flex;
    align-items: center;

    padding-left: 37px;

    margin-bottom: 14px;

    background: #3c4452;
    color: white;

    border-radius: 0 15px 15px 0;

    font-size: 28px;
    font-weight: 700;
}

/* =========================
   DATA PRIBADI
========================= */

.data {
    display: grid;

    grid-template-columns: 290px 1fr;

    row-gap: 5px;

    font-size: 18px;
    line-height: 1.45;
}

.data .label::before {
    content: "•";
    margin-right: 15px;
}

.data .isi::before {
    content: ": ";
}

/* =========================
   LIST
========================= */

.list {
    list-style: none;
    font-size: 18px;
    line-height: 1.55;
}

.list li {
    margin-bottom: 3px;
}

.list li::before {
    content: "•";
    margin-right: 15px;
}

/* =========================
   TITIK-TITIK KANAN
========================= */

.dots-right {
    position: absolute;
    right: 25px;
    top: 820px;
    width: 75px;
    z-index: 3;
}

.dots-right span {
    margin-right: 18px;
    margin-bottom: 28px;
}

/* =========================
   DEKORASI BAWAH
========================= */

.bottom-dark {
    position: absolute;
    right: 0;
    bottom: 0;

    width: 580px;
    height: 210px;

    background: #293344;

    clip-path: polygon(100% 0,100% 100%,0 100%);
}

.bottom-gold {
    position: absolute;
    right: 0;
    bottom: 0;

    width: 500px;
    height: 125px;

    background: #c8a75d;

    clip-path: polygon(100% 0,100% 100%,0 100%);
}

.bottom-line {
    position: absolute;
    right: 0;
    bottom: 65px;

    width: 520px;
    height: 12px;

    background: #c8a75d;

    transform: skewY(-24deg);
}

/* =========================
   RESPONSIVE
========================= */

@media (max-width: 1050px) {
    .cv {
        width: 95%;
    }
}

@media (max-width: 700px) {

    .cv {
        width: 100%;
        min-height: 100vh;

        margin: 0;

        padding: 100px 25px 160px;
    }

    .header {
        flex-direction: column;
        align-items: flex-start;
        gap: 20px;
    }

    .foto {
        width: 160px;
        height: 165px;
    }

    .nama h1 {
        font-size: 28px;
        white-space: normal;
    }

    .kontak {
        font-size: 14px;
    }

    .judul {
        width: 100%;
        height: 52px;
        font-size: 22px;
        padding-left: 25px;
    }

    .data {
        display: block;
        font-size: 15px;
    }

    .data .label {
        margin-top: 7px;
    }

    .data .isi {
        padding-left: 25px;
    }

    .list {
        font-size: 15px;
    }

    .top-gold {
        width: 300px;
        height: 90px;
    }

    .top-dark {
        width: 200px;
        height: 90px;
    }

    .dots-top {
        left: 20px;
        top: 20px;
        transform: scale(.65);
        transform-origin: left top;
    }

    .dots-right {
        display: none;
    }

    .bottom-dark {
        width: 330px;
        height: 140px;
    }

    .bottom-gold {
        width: 280px;
        height: 80px;
    }
}

/* =========================
   PRINT
========================= */

@media print {

    body {
        background: white;
    }

    .cv {
        margin: 0;
        width: 100%;
        box-shadow: none;
    }
}
</style>
</head>


<body>

<div class="cv">

    <!-- ======================
         DEKORASI ATAS
    ======================= -->

    <div class="top-gold"></div>
    <div class="top-light"></div>
    <div class="top-dark"></div>


    <!-- TITIK ATAS -->
    <div class="dots-top">

        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>

        <br>

        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>

    </div>


    <!-- ======================
         HEADER
    ======================= -->

    <div class="header">

        <img
            src="foto-cv.jpg"
            alt="Foto Rai Haidar Muhadzib"
            class="foto"
        >

        <div class="nama">

            <h1>
                RAI HAIDAR MUHADZIB
            </h1>

            <div class="kontak">

                <div>
                    ☎ &nbsp;0856-4793-4108
                </div>

                <div>
                    ✉ &nbsp;raihaidarmuhadzib@gmail.com
                </div>

            </div>

        </div>

    </div>


    <!-- ======================
         DATA PRIBADI
    ======================= -->

    <section class="section">

        <div class="judul">
            Data Pribadi
        </div>

        <div class="data">

            <div class="label">Nama</div>
            <div class="isi">Rai Haidar Muhadzib</div>

            <div class="label">Tanggal lahir</div>
            <div class="isi">19 Juli 2006</div>

            <div class="label">Alamat</div>
            <div class="isi">
                Pengarasan, Kec. Bantarkawung, Kab. Brebes,
                Jawa Tengah
            </div>

            <div class="label">Usia</div>
            <div class="isi">19 tahun</div>

            <div class="label">Jenis kelamin</div>
            <div class="isi">Laki-laki</div>

            <div class="label">Status</div>
            <div class="isi">Belum menikah</div>

            <div class="label">Kewarganegaraan</div>
            <div class="isi">Indonesia</div>

        </div>

    </section>


    <!-- ======================
         PENDIDIKAN
    ======================= -->

    <section class="section">

        <div class="judul">
            Pendidikan
        </div>

        <ul class="list">

            <li>
                SD Negeri 01 Pengarasan
            </li>

            <li>
                MTs Tarbiyatul Athfal Pengarasan
            </li>

            <li>
                SMK Al-Furqon Bantarkawung
            </li>

        </ul>

    </section>


    <!-- ======================
         PENGALAMAN
    ======================= -->

    <section class="section">

        <div class="judul">
            Pengalaman
        </div>

        <ul class="list">

            <li>
                Mengikuti Praktek Kerja Lapangan
                (PKL) Di Rumah Mesin Yogyakarta
            </li>

            <li>
                Bekerja Di Bagian Gudang Wisma
                Kedoya Selama 9 Bulan
            </li>

        </ul>

    </section>


    <!-- ======================
         KEAHLIAN
    ======================= -->

    <section class="section">

        <div class="judul">
            Keahlian
        </div>

        <ul class="list">

            <li>
                Manajemen Waktu
            </li>

            <li>
                Kerja Tim
            </li>

            <li>
                Kreativitas
            </li>

        </ul>

    </section>


    <!-- ======================
         TITIK KANAN
    ======================= -->

    <div class="dots-right">

        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>

    </div>


    <!-- ======================
         DEKORASI BAWAH
    ======================= -->

    <div class="bottom-dark"></div>
    <div class="bottom-gold"></div>
    <div class="bottom-line"></div>

</div>

</body>
</html>
