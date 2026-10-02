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
            font-family: Arial, Helvetica, sans-serif;
            background: #eeeeee;
            color: #3d4148;
        }

        /* CONTAINER CV */
        .cv {
            width: 1000px;
            min-height: 1400px;
            margin: 30px auto;
            background: white;
            position: relative;
            overflow: hidden;
            padding: 60px 70px;
            box-shadow: 0 5px 25px rgba(0, 0, 0, 0.12);
        }

        /* =======================
           DEKORASI ATAS
        ======================= */

        .top-decoration {
            position: absolute;
            top: 0;
            right: 0;
            width: 500px;
            height: 130px;
            background: #c8a95f;
            clip-path: polygon(35% 0, 100% 0, 100% 100%);
        }

        .top-decoration::after {
            content: "";
            position: absolute;
            right: 0;
            top: 0;
            width: 330px;
            height: 100%;
            background: #293343;
            clip-path: polygon(55% 0, 100% 0, 100% 100%);
        }

        /* =======================
           HEADER
        ======================= */

        .header {
            position: relative;
            z-index: 2;

            display: flex;
            align-items: center;
            gap: 45px;

            margin-bottom: 45px;
        }

        .foto {
            width: 205px;
            height: 205px;

            object-fit: cover;

            border-radius: 28px;
            border: 4px solid #c8a95f;
        }

        .header-content {
            flex: 1;
        }

        .header-content h1 {
            font-size: 43px;
            font-weight: 400;
            letter-spacing: 1px;
            margin-bottom: 28px;
            color: #343941;
        }

        .kontak {
            display: flex;
            flex-direction: column;
            gap: 9px;

            font-size: 17px;
        }

        /* =======================
           SECTION
        ======================= */

        .section {
            position: relative;
            z-index: 2;
            margin-bottom: 25px;
        }

        .section-title {
            width: 405px;

            background: #3c4452;
            color: white;

            padding: 9px 25px;

            border-radius: 0 15px 15px 0;

            font-size: 25px;
            margin-bottom: 15px;
        }

        /* =======================
           DATA PRIBADI
        ======================= */

        .data-pribadi {
            display: grid;
            grid-template-columns: 260px 1fr;

            row-gap: 5px;

            font-size: 17px;
        }

        .data-pribadi .label::before {
            content: "•";
            margin-right: 12px;
            font-weight: bold;
        }

        .data-pribadi .isi::before {
            content: ": ";
        }

        /* =======================
           LIST
        ======================= */

        ul {
            list-style: none;
        }

        li {
            font-size: 17px;
            margin-bottom: 7px;
        }

        li::before {
            content: "•";
            margin-right: 12px;
            font-weight: bold;
        }

        /* =======================
           DEKORASI BAWAH
        ======================= */

        .bottom-decoration {
            position: absolute;

            right: 0;
            bottom: 0;

            width: 560px;
            height: 190px;

            background: #293343;

            clip-path: polygon(
                100% 0,
                100% 100%,
                0 100%
            );
        }

        .bottom-decoration::before {
            content: "";

            position: absolute;

            right: 0;
            bottom: 0;

            width: 500px;
            height: 70px;

            background: #c8a95f;

            clip-path: polygon(
                100% 0,
                100% 100%,
                0 100%
            );
        }

        /* =======================
           RESPONSIVE HP
        ======================= */

        @media (max-width: 1050px) {

            .cv {
                width: 95%;
                margin: 20px auto;
            }
        }

        @media (max-width: 700px) {

            .cv {
                width: 100%;
                min-height: 100vh;

                margin: 0;

                padding: 30px 25px 100px;
            }

            .header {
                flex-direction: column;
                align-items: flex-start;

                gap: 20px;
            }

            .foto {
                width: 160px;
                height: 160px;
            }

            .header-content h1 {
                font-size: 30px;
                line-height: 1.2;
            }

            .kontak {
                font-size: 14px;
            }

            .section-title {
                width: 100%;
                font-size: 21px;
            }

            .data-pribadi {
                display: block;
                font-size: 15px;
            }

            .data-pribadi .label {
                margin-top: 7px;
            }

            .data-pribadi .isi {
                padding-left: 24px;
            }

            li {
                font-size: 15px;
            }

            .top-decoration {
                width: 250px;
                height: 80px;
            }

            .bottom-decoration {
                width: 300px;
                height: 120px;
            }
        }

        /* PRINT */
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

        <!-- DEKORASI ATAS -->
        <div class="top-decoration"></div>


        <!-- HEADER -->
        <header class="header">

            <!--
                Letakkan foto dengan nama:
                foto-cv.jpg

                di folder yang sama dengan index.html
            -->
            <img 
                src="foto-cv.jpg"
                alt="Foto Rai Haidar Muhadzib"
                class="foto"
            >

            <div class="header-content">

                <h1>
                    RAI HAIDAR MUHADZIB
                </h1>

                <div class="kontak">

                    <div>
                        ☎ 0856-4793-4108
                    </div>

                    <div>
                        ✉ raihaidarmuhadzib@gmail.com
                    </div>

                </div>

            </div>

        </header>


        <!-- DATA PRIBADI -->
        <section class="section">

            <h2 class="section-title">
                Data Pribadi
            </h2>

            <div class="data-pribadi">

                <div class="label">
                    Nama
                </div>

                <div class="isi">
                    Rai Haidar Muhadzib
                </div>


                <div class="label">
                    Tanggal lahir
                </div>

                <div class="isi">
                    19 Juli 2006
                </div>


                <div class="label">
                    Alamat
                </div>

                <div class="isi">
                    Pengarasan, Kec. Bantarkawung,
                    Kab. Brebes, Jawa Tengah
                </div>


                <div class="label">
                    Usia
                </div>

                <div class="isi">
                    19 tahun
                </div>


                <div class="label">
                    Jenis kelamin
                </div>

                <div class="isi">
                    Laki-laki
                </div>


                <div class="label">
                    Status
                </div>

                <div class="isi">
                    Belum menikah
                </div>


                <div class="label">
                    Kewarganegaraan
                </div>

                <div class="isi">
                    Indonesia
                </div>

            </div>

        </section>


        <!-- PENDIDIKAN -->
        <section class="section">

            <h2 class="section-title">
                Pendidikan
            </h2>

            <ul>

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


        <!-- PENGALAMAN -->
        <section class="section">

            <h2 class="section-title">
                Pengalaman
            </h2>

            <ul>

                <li>
                    Mengikuti Praktek Kerja Lapangan (PKL)
                    di Rumah Mesin Yogyakarta
                </li>

                <li>
                    Bekerja di bagian gudang Wisma Kedoya
                    selama 9 bulan
                </li>

            </ul>

        </section>


        <!-- KEAHLIAN -->
        <section class="section">

            <h2 class="section-title">
                Keahlian
            </h2>

            <ul>

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


        <!-- DEKORASI BAWAH -->
        <div class="bottom-decoration"></div>

    </div>

</body>
</html>
