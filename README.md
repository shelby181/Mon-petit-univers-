Pour toi mon amour ❤🫂
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Juste pour toi ❤️</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    background: linear-gradient(145deg, #170d19, #351b30, #120b16);
    color: white;
    font-family: Georgia, serif;
    padding: 30px 18px;
}

.container {
    max-width: 450px;
    width: 100%;
    margin: 40px auto;
    text-align: center;
}

.top {
    color: #e7a5bc;
    letter-spacing: 4px;
    font-size: 11px;
    margin-bottom: 30px;
}

h1 {
    color: #ffabc5;
    font-size: 30px;
    font-weight: normal;
    margin-bottom: 15px;
}

.intro {
    color: #e0cad7;
    line-height: 1.9;
    font-size: 15px;
    margin-bottom: 35px;
}

.card {
    background: rgba(255,255,255,0.05);
    border: 1px solid #a95778;
    border-radius: 22px;
    padding: 25px 18px;
    box-shadow: 0 10px 35px #0005;
}

.heart {
    font-size: 45px;
    color: #ff7da5;
    margin-bottom: 20px;
}

button {
    width: 100%;
    padding: 16px 12px;
    margin: 10px 0;
    border: 1px solid #d87899;
    border-radius: 30px;
    background: linear-gradient(135deg, #a83d69, #e76b91);
    color: white;
    font-family: Georgia, serif;
    font-size: 15px;
    cursor: pointer;
    transition: .3s;
}

button:active {
    transform: scale(.96);
}

.message {
    display: none;
    background: #281a2b;
    border: 1px solid #81506c;
    border-radius: 16px;
    padding: 23px 18px;
    margin: 12px 0 20px;
    text-align: left;
    line-height: 1.9;
    color: #f2dce7;
    font-size: 15px;
    animation: appear 1s ease;
}

.message h2 {
    color: #ffabc5;
    text-align: center;
    font-size: 21px;
    font-weight: normal;
    margin-bottom: 18px;
}

@keyframes appear {
    from {
        opacity: 0;
        transform: translateY(15px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.signature {
    text-align: center;
    color: #ffabc5;
    font-style: italic;
    margin-top: 20px;
}

footer {
    color: #a88b9d;
    font-size: 11px;
    letter-spacing: 2px;
    margin-top: 35px;
}

</style>
</head>

<body>

<div class="container">

    <div class="top">UNE PETITE SURPRISE</div>

    <h1>Juste pour toi ❤️</h1>

    <p class="intro">
        J'ai quelque chose à te dire...
        <br>
        Mais je préfère te laisser le découvrir.
        <br>
        Ouvre chaque petit message. 💌
    </p>

    <div class="card">

        <div class="heart">♥</div>

        <button onclick="ouvrirMessage(1)">
            01 — Je t'aime ❤️
        </button>

        <div class="message" id="msg1">
            <h2>Je t'aime ❤️</h2>
            Trois petits mots, mais tellement de sentiments
            derrière eux.
        </div>

        <button onclick="ouvrirMessage(2)">
            02 — Et même si... 💗
        </button>

        <div class="message" id="msg2">
            <h2>Et même si... 💗</h2>
            Et même si je te l'ai dit 1 million de fois,
            je trouverai toujours une nouvelle façon
            de te le rappeler.
        </div>

        <button onclick="ouvrirMessage(3)">
            03 — Un message pour toi 💌
        </button>

        <div class="message" id="msg3">
            <h2>À toi, Manmi ❤️</h2>

            Je sais, que je te l'ai déjà dit un million
            de fois, mais je le pense sincèrement.

            Je suis tombé amoureux de chaque partie de toi.

            Je n'ai jamais connu un bonheur pareil à celui
            que je ressens quand nous sommes ensemble.

            Le simple fait de t'entendre parler ou de voir
            sourire fait briller quelque chose en moi,
            même dans mes journées les plus sombres.

            Je t'aime de tout mon cœur.

            <div class="signature">
                Avec amour, Papi ❤️
            </div>
        </div>

    </div>

    <footer>
        CRÉÉ SPÉCIALEMENT POUR TOI ❤️
        <br><br>
        10 NOVEMBRE 2026
    </footer>

</div>

<script>
function ouvrirMessage(numero) {

    const message = document.getElementById("msg" + numero);

    if (message.style.display === "block") {
        message.style.display = "none";
    } else {
        message.style.display = "block";

        setTimeout(function() {
            message.scrollIntoView({
                behavior: "smooth",
                block: "center"
            });
        }, 100);
    }
}
</script>

</body>
</html>
