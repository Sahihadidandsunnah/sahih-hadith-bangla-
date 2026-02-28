# sahih-hadith-bangla-
Assalamualaikum 
index.html
<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sahih Hadith Bangla</title>

<style>
body {
    margin: 0;
    font-family: 'Segoe UI', sans-serif;
    background: #f0fdf4;
}

header {
    background: #064e3b;
    color: white;
    text-align: center;
    padding: 20px;
}

nav {
    background: #065f46;
    display: flex;
    justify-content: center;
    gap: 15px;
    padding: 10px;
}

nav a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

.container {
    padding: 20px;
    max-width: 900px;
    margin: auto;
}

.search-box {
    text-align: center;
    margin-bottom: 20px;
}

input {
    width: 70%;
    padding: 10px;
    border-radius: 5px;
    border: 1px solid #ccc;
}

.hadith-card {
    background: white;
    padding: 20px;
    margin-bottom: 20px;
    border-left: 5px solid #10b981;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.reference {
    font-weight: bold;
    color: #065f46;
    margin-top: 10px;
}

footer {
    background: #064e3b;
    color: white;
    text-align: center;
    padding: 15px;
}
</style>

<script>
function searchHadith() {
    let input = document.getElementById("searchInput").value.toLowerCase();
    let cards = document.getElementsByClassName("hadith-card");

    for (let i = 0; i < cards.length; i++) {
        let text = cards[i].innerText.toLowerCase();
        if (text.includes(input)) {
            cards[i].style.display = "block";
        } else {
            cards[i].style.display = "none";
        }
    }
}
</script>

</head>
<body>

<header>
    <h1>📖 সহিহ হাদিস বাংলা</h1>
    <p>কুরআন ও সুন্নাহ ভিত্তিক সহিহ হাদিস</p>
</header>

<nav>
    <a href="#">সহিহ বুখারি</a>
    <a href="#">সহিহ মুসলিম</a>
    <a href="#">রিয়াদুস সালেহীন</a>
    <a href="#">দৈনিক সুন্নাহ</a>
</nav>

<div class="container">

<div class="search-box">
    <input type="text" id="searchInput" onkeyup="searchHadith()" placeholder="হাদিস খুঁজুন...">
</div>

<div class="hadith-card">
    <p>আবু হুরায়রা (রাঃ) হতে বর্ণিত, রাসূলুল্লাহ ﷺ বলেছেন:
    “পাঁচ ওয়াক্ত সালাত, এক জুম‘আ থেকে অন্য জুম‘আ এবং এক রমযান থেকে অন্য রমযান—মাঝের গুনাহসমূহের কাফফারা।”</p>
    <div class="reference">সহিহ মুসলিম: 233</div>
</div>

<div class="hadith-card">
    <p>রাসূলুল্লাহ ﷺ বলেছেন:
    “তোমাদের মধ্যে সর্বোত্তম ব্যক্তি সেই, যে কুরআন শিক্ষা করে এবং শিক্ষা দেয়।”</p>
    <div class="reference">সহিহ বুখারি: 5027</div>
</div>

</div>

<footer>
    © 2026 Sahih Hadith Bangla | Developed for Islamic Knowledge
</footer>

</body>
</html>
