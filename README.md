<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Un petit cadeau ❤️</title>

<style>
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    min-height: 100vh;
    background: #140d18;
    color: white;
    font-family: Georgia, serif;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 25px 15px;
}

.page {
    width: 100%;
    max-width: 430px;
    text-align: center;
    padding: 35px 20px;
}

.decor {
    color: #ff91b3;
    font-size: 25px;
    margin-bottom: 25px;
}

h1 {
    color: #ffabc5;
    font-size: 29px;
    font-weight: normal;
    margin-bottom: 18px;
}

.intro {
    color: #d9c4d1;
    font-size: 15px;
    line-height: 1.8;
    margin-bottom: 45px;
}

.card {
    background: linear-gradient(145deg, #302033, #211522);
    border: 1px solid #92516f;
    border-radius: 24px;
    padding: 35px 22px;
    box-shadow: 0 10px 40px #00000055;
}

.heart {
    font-size: 65px;
    color: #ff719e;
    margin-bottom: 20px;
    animation: heartbeat 1.8s infinite;
}

@keyframes heartbeat {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.12); }
}

button {
    border: none;
    background: linear-gradient(135deg, #ff91b3, #d94377);
    color: white;
    padding: 15px 25px;
    border-radius: 30px;
    font-size: 15px;
    font-family: Georgia, serif;
    cursor: pointer;
    margin-top: 20px;
}

button:active {
    transform: scale(.96);
}

.message {
    display: none;
    margin-top: 30px;
    padding-top: 25px;
    border-top: 1px solid #92516f;
    animation: show 1.2s ease;
}

@keyframes show {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.message h2 {
    color: #ffabc5;
    font-weight: normal;
    font-size: 24px;
    margin-bottom: 22px;
}

.message p {
    color: #f0dce6;
    font-size: 15px;
    line-height: 2;
}

.signature {
    color: #ffabc5;
    font-style: italic;
    margin-top: 25px;
    font-size: 17px;
}

footer {
    color: #94798a;
    font-size: 11px;
    letter-spacing: 2px;
    margin-top: 35px;
}

@media(max-width: 380px) {
    h1 { font-size: 25px; }
    .card { padding: 28px 17px; }
}
</style>
</head>

<body>

<div class="page">

    <div class="decor">✦ ♡ ✦</div>

    <h1>Un petit quelque chose pour toi</h1>

    <p class="intro">
        Ce n'est pas un grand cadeau...
        <br>
        Mais il vient d'un endroit très spécial.
    </p>

    <div class="card">

        <div class="heart">♥</div>

        <h1>Juste pour toi, Manmi</h1>

        <p class="intro">
            J'ai gardé une petite surprise ici.
            Elle n'attend que toi...
        </p>

        <button id="ouvrir" type="button">
            Découvrir ma surprise ❤️
        </button>

        <div class="message" id="message">

            <h2>Mon petit message pour toi 💌</h2>

            <p>
                Je voulais simplement te rappeler
                que certaines personnes rendent
                la vie plus belle sans même le savoir.
                <br><br>
                Tu es l'une de ces personnes.
                <br><br>
                Peu importe les jours, les distances
                ou les circonstances, n'oublie jamais
                que tu as une place particulière
                dans mon cœur.
                <br><br>
                Ce petit geste est simplement
                une façon de te dire :
                tu comptes énormément pour moi. ❤️
            </p>

            <div class="signature">
                Avec amour, Papi ❤️
            </div>

        </div>

    </div>

    <footer>
        CRÉÉ SPÉCIALEMENT POUR TOI · 10.11.2026
    </footer>

</div>

<script>
const bouton = document.getElementById("ouvrir");
const message = document.getElementById("message");

bouton.addEventListener("click", function() {
    message.style.display = "block";
    bouton.style.display = "none";

    setTimeout(function() {
        message.scrollIntoView({
            behavior: "smooth",
            block: "center"
        });
    }, 150);
});
</script>

</body>
</html>
