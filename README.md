<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pour Ibtihal</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background-color: #ffe6e6; margin: 50px; }
        .container { background: white; padding: 20px; border-radius: 10px; box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1); display: inline-block; }
        .hidden { display: none; }
        button { background-color: #ff4d4d; color: white; border: none; padding: 10px 20px; border-radius: 5px; cursor: pointer; font-size: 16px; margin-top: 20px; }
        button:hover { background-color: #cc0000; }
        img { width: 200px; height: auto; border-radius: 10px; margin: 10px; display: block; }
    </style>
</head>
<body>
    <div class="container" id="introPage">
        <button id="introButton">Chère Ibtihal</button>
        <p id="introMessage" class="hidden">Salut Ibtihal, si tu lis ça, c'est que j’ai réussi à faire le petit site internet. Je tenais à te faire cette petite surprise, cette petite attention à distance, parce qu’on ne pourra pas se voir le jour de la Saint-Valentin, et l’idée que j’avais de base était un peu trop risquée, que ça soit envers tes parents ou même avec le timing, etc. J’espère que ça te fera plaisir tout de même. Je t’avoue que je ne suis pas très bon, mdr. J'irai faire des recherches sur comment coder un site, mais j’espère faire un truc potable qui te fera plaisir. Si je fais tout ça, c’est parce que je t’aime. Sérieux, Ibtihal, je t’aime tellement, j’ai toujours envie de faire plus pour toi, de donner plus, de te faire des surprises, de te faire plaisir. Je suis sincère quand je dis ça : j’adore te voir sourire, surtout quand ça vient de moi, te voir sourire parce que je t’ai fait rire, parce que t’as aimé quelques choses que j’ai pu dire ou faire, te voir sourire après qu’on se soit embrassé ou après un câlin. Tu mérites que du bien, Ibtihal, tu mérites tout ce que ce monde possède, et j’espère réussir à toujours te le prouver dans les années qui suivront. Je t’aime, Ibtihal, tu es véritablement la personne la plus chère de ma vie, celle que j’aime le plus. J’ai si hâte qu’on vive ensemble, dans notre appartement ou maison avec notre chien, notre chat, notre chèvre, notre singe, notre tigre, notre renard, notre lapin, notre hamster, notre cheval et tout le reste, mdrrr. Sérieux. Je t’aime, Ibtihal, j’ai hâte de te revoir, qu’on passe encore des moments ensemble. J’ai hâte d’être avec toi en bord de mer, au bord de la plage. Je n’arrête pas de nous imaginer, de te voir dans mes pensées et je tiens à dire que tu es si belle. Tu es si magnifique, Ibtihal, si ravissante, charmante, éblouissante. J’adore te contempler, me dire que tu es mienne, me sentir spécial à tes côtés. Tu es unique, Ibtihal. Tu es ce qu'il me faut, tu es la personne avec qui je vais finir, avec qui je dois finir. Je t’aime, Ibtihal, j’espère que tu le sens, que tu le sais, que je te fais sentir spécial, que je te montre à quel point tu es splendide, à quel point tu m’importes, à quel point je t’aime, à quel point je suis sincère avec toi. Tu es si gentille, si attentionnée, si parfaite, ton amour est si chaleureux, si doux, tes lèvres sont si douces, tes câlins si purs. Merci d’être là, sincèrement merci d’être là. Tu es drôle, généreuse, passionnée, intelligente, réfléchie, instruite, attirante, irremplaçable, unique, douce. Je pourrais te décrire et rajouter des trucs si longtemps. J’adore l’idée que tu sois mienne, que tu sois dans ma vie. J’adore tes yeux, j’adore ton regard innocent rempli d’amour, j’adore t’entendre, t’écouter parler, que ça soit de ta journée ou de te plaindre sur quelqu’un ou quelque chose, j’adore regarder des trucs avec toi, découvrir de nouveaux trucs avec toi, discuter avec toi, dormir avec toi, marcher avec toi, manger avec toi, sortir avec toi. Ah Ibtihal, je t’aime et merci. </p>
        <button id="loveButton" class="hidden">Je t'aime</button>
    </div>

    <div class="container hidden" id="mainPage">
        <p id="question">Voudrais-tu être ma valentine ? </p>
        <button id="yesButton">Oui</button>
        <button id="noButton">Non</button>
    </div>

    <div class="container hidden" id="activitiesPage">
        <h2>Choisis une activité </h2>
        <button onclick="chooseActivity('Cinéma')">Cinéma</button>
        <button onclick="chooseActivity('Bowling')">Bowling</button>
        <button onclick="chooseActivity('Escape Room')">Escape Room</button>
        <button onclick="chooseActivity('Arcade')">Arcade</button>
        <button onclick="chooseActivity('Resto')">Resto</button>
        <button onclick="chooseActivity('Musée')">Musée</button>
        <button onclick="chooseActivity('Spa')">Spa</button>
        <button onclick="chooseActivity('Massage')">Massage</button>
    </div>

    <div class="container hidden" id="datePage">
        <h2>Quand es-tu libre pour notre date ? </h2>
        <input type="date" id="dateInput">
        <button id="dateButton">Valider</button>
    </div>

    <div class="container hidden" id="foodPage">
        <h2>T'aimerais manger quoi ce jour-là ? (T'inquiète, j'invite) </h2>
        <button onclick="chooseFood('Sushi')">Sushi</button>
        <button onclick="chooseFood('Ramen')">Ramen</button>
        <button onclick="chooseFood('Pâtes')">Pâtes</button>
        <button onclick="chooseFood('Fruits de mer')">Fruits de mer</button>
        <button onclick="chooseFood('BBQ coréen')">BBQ coréen</button>
        <button onclick="chooseFood('Chicken street')">Chicken street</button>
    </div>

    <div class="container hidden" id="confirmationPage">
        <h2> Confirmation de ta date </h2>
        <p id="confirmationText"></p>
        <p><strong>Numéro de commande :</strong> #TonMecEnOr</p>
        <p> Une seule condition s'applique : Tu dois jurer de toujours aimer Anis Arous et de le remercier avec un câlin </p>
    </div>

    <script>
        let selectedActivity = "";
        let selectedDate = "";
        let selectedFood = "";

        document.getElementById("introButton").addEventListener("click", function() {
            document.getElementById("introMessage").classList.remove("hidden");
            document.getElementById("loveButton").classList.remove("hidden");
            document.getElementById("introButton").classList.add("hidden");
        });

        document.getElementById("loveButton").addEventListener("click", function() {
            document.getElementById("introPage").classList.add("hidden");
            document.getElementById("mainPage").classList.remove("hidden");
        });

        document.getElementById("yesButton").addEventListener("click", function() {
            document.getElementById("mainPage").classList.add("hidden");
            document.getElementById("activitiesPage").classList.remove("hidden");
        });

        document.getElementById("noButton").addEventListener("click", function() {
            document.getElementById("question").textContent = "Je pense que tu t'es trompée haha ^^ Voudrais-tu être ma valentine ? ❤️";
        });

        function chooseActivity(activity) {
            selectedActivity = activity;
            document.getElementById("activitiesPage").classList.add("hidden");
            document.getElementById("datePage").classList.remove("hidden");
        }

        document.getElementById("dateButton").addEventListener("click", function() {
            selectedDate = document.getElementById("dateInput").value;
            document.getElementById("datePage").classList.add("hidden");
            document.getElementById("foodPage").classList.remove("hidden");
        });

        function chooseFood(food) {
            selectedFood = food;
            document.getElementById("foodPage").classList.add("hidden");
            document.getElementById("confirmationPage").classList.remove("hidden");
            document.getElementById("confirmationText").innerHTML = `🎉 Activité : ${selectedActivity} <br> 📅 Date : ${selectedDate} <br> 🍽️ Repas : ${selectedFood}`;
        }
    </script>
</body>
</html>
