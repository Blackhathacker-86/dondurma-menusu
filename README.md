<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dondurma Menüsü</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* Genel Ayarlar */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #fcf9f2; /* Dondurma dükkanına uygun krem rengi arka plan */
            color: #333;
            line-height: 1.6;
            padding: 20px;
        }
        .container {
            max-width: 800px;
            margin: 0 auto;
        }

        /* Başlık Alanı */
        header {
            text-align: center;
            margin-bottom: 40px;
            padding: 20px 0;
            border-bottom: 2px dashed #ff9a9e;
        }
        header h1 {
            font-size: 2.5rem;
            color: #ff6b81; /* Çilek pembesi */
            margin-bottom: 5px;
        }
        header p {
            color: #777;
            font-size: 1.1rem;
        }

        /* Kategori Başlıkları */
        .category-title {
            font-size: 1.5rem;
            color: #2f3542;
            margin: 30px 0 15px 0;
            padding-left: 10px;
            border-left: 4px solid #ff6b81;
        }

        /* Menü Grid Yapısı (Telefonda alt alta, PC'de yan yana) */
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        /* Dondurma Kartları */
        .menu-item {
            background-color: #fff;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .menu-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
        }

        /* Fotoğraf Alanı */
        .item-image {
            width: 100%;
            height: 200px;
            object-fit: cover;
            background-color: #eee; /* Fotoğraf yüklenene kadar görünecek renk */
        }

        /* İçerik Alanı */
        .item-content {
            padding: 15px;
        }
        .item-title {
            font-size: 1.2rem;
            font-weight: 600;
            color: #ff4757;
            margin-bottom: 8px;
            display: flex;
            justify-content: space-between;
        }
        .item-desc {
            font-size: 0.9rem;
            color: #57606f;
        }

        /* Alt Bilgi */
        footer {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            font-size: 0.9rem;
            color: #a4b0be;
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>🍦 Dondurma Menüsü</h1>
        <p>Serinleten taze lezzetler</p>
    </header>

    <!-- 1. KATEGORİ -->
    <h2 class="category-title">Klasik & Yoğun Lezzetler</h2>
    <div class="menu-grid">
        
        <div class="menu-item">
            <!-- İNTERNETTEN BULDUĞUN FOTOĞRAFIN LİNKİNİ src="..." İÇİNE YAPIŞTIR -->
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTYi6KeD9c9IEIomyfU4wsZX7-3tX4_6wEwRg&s" alt="Kaymak" class="item-image">
            <div class="item-content">
                <div class="item-title">Kaymak</div>
                <div class="item-desc">Sütün en saf, en zengin hali. Pürüzsüz dokusuyla tek başına bir şölen.</div>
            </div>
        </div>

        <div class="menu-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRmKV0CSj6F6aX8a2v5zx0fgfHwy1NzL-w1Qg&s" alt="Çikolata" class="item-image">
            <div class="item-content">
                <div class="item-title">Çikolata</div>
                <div class="item-desc">Yüksek kakao notalarının getirdiği zengin aroma ve ipeksi yapı.</div>
            </div>
        </div>

        <div class="menu-item">
            <img src="https://cdn.cimri.io/market/260x260/kartepe-40-gr-sut-karamelli-dondurma-_1030549.jpg" alt="Karamel" class="item-image">
            <div class="item-content">
                <div class="item-title">Karamel</div>
                <div class="item-desc">Karamelize şekerin derin notaları ve kremamsı yapısıyla efsanevi lezzet.</div>
            </div>
        </div>
    </div>

    <!-- 2. KATEGORİ -->
    <h2 class="category-title">Taze & Ferah Meyveliler</h2>
    <div class="menu-grid">
        
        <div class="menu-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTJrBrFRyZVNWhTCUc_wE3DLCtGHSBDJQxJNw&s" alt="Limon" class="item-image">
            <div class="item-content">
                <div class="item-title">Limon</div>
                <div class="item-desc">Canlı asiditesi ve narenciye ferahlığıyla damağı temizleyen serinlik.</div>
            </div>
        </div>

        <div class="menu-item">
            <img src="https://cdn2.karaca.com/karaca-cms-uploads/thumbnail_evde_cilekli_dondurma_yapimi_f147f18c69.jpg" alt="Çilek" class="item-image">
            <div class="item-content">
                <div class="item-title">Çilek</div>
                <div class="item-desc">Taze çileklerin doğal tatlılığı ve hafif mayhoş aroması.</div>
            </div>
        </div>

        <div class="menu-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRCSJh5BKSs_5BWhPx56uFu5D-XwIuo1NE97w&s" alt="Karadut" class="item-image">
            <div class="item-content">
                <div class="item-title">Karadut</div>
                <div class="item-desc">Buruk-tatlı dengesi ve yoğun koyu rengiyle karakteristik bir lezzet.</div>
            </div>
        </div>

    </div>

    <!-- 3. KATEGORİ -->
    <h2 class="category-title">Çıtır Dokulu & Kuruyemişliler</h2>
    <div class="menu-grid">
        
        <div class="menu-item">
            <img src="https://static.ticimax.cloud/cdn-cgi/image/width=0,quality=85/73065/uploads/urunresimleri/buyuk/serez-gurme-dondurma-antep-fistigi-500-9188ef.jpg" alt="Antep Fıstık" class="item-image">
            <div class="item-content">
                <div class="item-title">Antep Fıstık</div>
                <div class="item-desc">Kavrulmuş birinci sınıf fıstıkların derin aroması ve yoğun dokusu.</div>
            </div>
        </div>

        <div class="menu-item">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS3KRlsrtjv-eMZ4lIIteSZK00FhUkCZ0qC2w&s" alt="Oreo" class="item-image">
            <div class="item-content">
                <div class="item-title">Oreo</div>
                <div class="item-desc">Sütlü dondurma tabanında yoğun kakao bisküvisi parçacıkları.</div>
            </div>
        </div>

    </div>

    <!-- 4. KATEGORİ -->
    <h2 class="category-title">Eğlenceli & Renkli Tatlar</h2>
    <div class="menu-grid">
        
        <div class="menu-item">
            <img src="data:image/jpeg;base64,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4dWmmCvn39rq0jaXD5/yut4TiP8AGBBmbiCI71S5aJcky+FRbaQzWmFAw7CdVZU8rYJkqWPE2+yu8nwvZ6wLQwBrLBogAKwa1rtRBXL/ANxNNxztcBJgxbW110HDcY1+4K9DR3LjaWze6gQvdGvFjotPEK8WHiodHEQJJtMR16LjkyvE2tovmgLaxqhYV/kVPYFUzObGhe15C9KBwIiIAiIgCwsogNbmrW5i3rELp0iuprU6kppasFi7sbK51BanYUclZli8mmu7O8iodgG8lpdwxvJXZprBpps7zZQO4U3kvB4Q3kuh9UseqXRzZz44Q3kvQ4WOSvfVJ6pNjmyhPCm8l6HDWjZXfqlg00HNlQMNChY4kOjoP3XQmkouM4aH940UpaTLsORTW2U4q3giRGhXuhhqc5gCx36DE+Gi91sC8GSJ7lra0hWbTNypNdM2cQry4DWwk8zGqrKtSFuxr7k/mi98O4e6o4Oc05db2zfwjeiDpQjo8E05Wz8LfoFZUloosUljVnbPMb2z2FlEUTgREQBERAEREAREQGISFlEB5hYyr2sIDxlWMq2JC6DVlTKtsLEJsGrKsZVuhITYNOVYyLdCQmwaciyGLbCzCbOmk0lpq4BjtQFMhE2dVNeis/stKZy3Gkkn5FS2YUBSUTbDpv2eGsXuFlFwiEREAREQBERAEREAREQBERAEREAREQBERAEREBhFlEBhFlEBhZREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQBERAEREAREQH/2Q==" alt="Bubble Gum" class="item-image">
            <div class="item-content">
                <div class="item-title">Bubble Gum</div>
                <div class="item-desc">Nostaljik kokusu ve rengarenk yapısıyla genç damaklara hitap eden neşe.</div>
            </div>
        </div>

        <div class="menu-item">
            <img src="https://digimenu.com.tr/Assets/uploads/urun_12_6926c3b3109a8.png" alt="Blue Sky" class="item-image">
            <div class="item-content">
                <div class="item-title">Blue Sky</div>
                <div class="item-desc">Gökyüzü mavisi rengiyle dikkat çeken, hafif ve ferahlatıcı reçete.</div>
            </div>
        </div>

    </div>

    <footer>
        <p>Afiyet olsun!</p>
    </footer>
</div>

</body>
</html>
