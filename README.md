<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ROX MUSIC - All Download Links</title>
    <style>
        /* Pure OLED Black */
        body { 
            font-family: 'Segoe UI', sans-serif; 
            background-color: #000; 
            color: #fff; 
            display: flex; 
            justify-content: center; 
            align-items: center; 
            min-height: 100vh; 
            margin: 0; 
        }
        .container { 
            width: 85%; 
            max-width: 400px; 
            background: #000; 
            padding: 40px 20px; 
            border-radius: 15px; 
            border: 1px solid #222; 
            text-align: center;
        }
        h1 { 
            font-size: 32px; 
            color: #fff; 
            margin: 0;
            letter-spacing: 3px;
        }
        .tagline { 
            color: #00ffcc; 
            font-size: 11px; 
            letter-spacing: 1px;
            margin-bottom: 30px;
            display: block;
            font-weight: bold;
        }
        input { 
            width: 100%; 
            padding: 15px; 
            margin-bottom: 20px; 
            border-radius: 8px; 
            border: 1px solid #333; 
            background: #050505; 
            color: #fff; 
            box-sizing: border-box; 
            outline: none;
            font-size: 16px;
            text-align: center;
        }
        input:focus { border-color: #00ffcc; }
        
        .search-btn { 
            background: #00ffcc; 
            color: #000; 
            border: none; 
            padding: 15px; 
            width: 100%; 
            border-radius: 8px; 
            font-weight: 800; 
            cursor: pointer; 
            font-size: 14px;
            text-transform: uppercase;
            transition: 0.2s;
        }
        .search-btn:hover { 
            background: #fff; 
            transform: scale(1.02);
        }
        .footer {
            margin-top: 40px;
            font-size: 10px;
            color: #333;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>ROX MUSIC</h1>
    <span class="tagline">FREE LINKS EDITION</span>

    <input type="text" id="songInput" placeholder="Enter Song Name...">
    <button class="search-btn" onclick="generateAllLinks()">Show All Download Links</button>

    <div class="footer">
        Powered by Google Search Engine
    </div>
</div>

<script>
    function generateAllLinks() {
        const song = document.getElementById('songInput').value;

        if(song.trim() === "") {
            alert("Bhai, pehle gaane ka naam toh likho!");
            return;
        }

        // Ye query Google ko batati hai ki sirf download sites (Pagalworld, Mr-Jatt, etc.) dikhaye
        const searchQuery = `${song} mp3 download pagalworld mr-jatt webmusic`;
        
        // Isse Google Search naye tab mein khulega saare links ke saath
        const finalUrl = `https://www.google.com/search?q=${encodeURIComponent(searchQuery)}`;
        
        window.open(finalUrl, '_blank');
    }
</script>

</body>
</html>
