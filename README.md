<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Can We Just Be Friends? 🌸</title>

<style>

/* =========================
   BASIC
========================= */

* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    font-family: Arial, sans-serif;

    background: linear-gradient(
        135deg,
        #ffe4f0,
        #fff8fc
    );

    display: flex;
    justify-content: center;
    align-items: center;

    overflow: hidden;
}


/* =========================
   FLOWERS
========================= */

.flower {
    position: fixed;
    font-size: 32px;
    z-index: 1;

    animation: float 3s ease-in-out infinite;
    user-select: none;
}

.f1 {
    top: 8%;
    left: 8%;
}

.f2 {
    top: 10%;
    right: 8%;
    animation-delay: 0.5s;
}

.f3 {
    bottom: 10%;
    left: 10%;
    animation-delay: 1s;
}

.f4 {
    bottom: 8%;
    right: 10%;
    animation-delay: 1.5s;
}

@keyframes float {

    0%, 100% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(-10px);
    }

}


/* =========================
   CARD
========================= */

.card {
    width: 90%;
    max-width: 450px;

    padding: 38px 25px;

    background: white;

    border-radius: 25px;

    text-align: center;

    box-shadow:
        0 10px 30px rgba(255, 105, 180, 0.25);

    position: relative;
    z-index: 5;

    animation: appear 0.8s ease;
}

@keyframes appear {

    from {
        opacity: 0;
        transform: scale(0.9);
    }

    to {
        opacity: 1;
        transform: scale(1);
    }

}


/* =========================
   TEXT
========================= */

.icon {
    font-size: 42px;
    margin-bottom: 8px;
}

h1 {
    color: #df5798;

    font-size: 29px;

    margin: 10px 0 18px;
}

p {
    color: #666;

    font-size: 16px;

    line-height: 1.7;

    margin: 0;
}

.question {
    color: #d94f91;

    font-size: 21px;

    font-weight: bold;

    margin: 25px 0 20px;
}


/* =========================
   BUTTON AREA
========================= */

.button-area {
    width: 100%;
    height: 60px;

    display: flex;

    justify-content: center;
    align-items: center;

    gap: 25px;
}


/* =========================
   BUTTONS
========================= */

button {
    width: 105px;
    height: 46px;

    padding: 0;

    border: none;
    border-radius: 25px;

    font-size: 16px;
    font-weight: bold;

    cursor: pointer;

    flex-shrink: 0;
}


/* =========================
   YES
========================= */

.yes {
    background: #ff69b4;
    color: white;

    transition: 0.2s;
}

.yes:hover {
    background: #e7549b;
    transform: scale(1.07);
}


/* =========================
   NO
========================= */

.no {
    position: static;

    background: #eeeeee;
    color: #777;

    transition:
        left 0.25s ease,
        top 0.25s ease,
        transform 0.2s ease;

    z-index: 20;
}


/*
   After NO is clicked,
   it becomes a floating button.
*/

.no.running {
    position: fixed;
}


/* =========================
   SUCCESS
========================= */

#success {
    display: none;
}

#success.show {
    display: block;

    animation: appear 0.7s ease;
}

.message {
    background: #fff0f7;

    padding: 20px;

    border-radius: 18px;

    color: #555;

    font-size: 16px;

    line-height: 1.7;
}

.back {
    display: inline-block;

    margin-top: 20px;

    color: #df5798;

    text-decoration: none;

    font-weight: bold;
}


/* =========================
   MOBILE
========================= */

@media (max-width: 500px) {

    .card {
        width: 92%;
        padding: 30px 20px;
    }

    h1 {
        font-size: 25px;
    }

    p {
        font-size: 15px;
    }

    .question {
        font-size: 19px;
    }

    .button-area {
        gap: 18px;
    }

    button {
        width: 100px;
    }

    .flower {
        font-size: 27px;
    }

}

</style>
</head>


<body>


<!-- =========================
     FLOWERS
========================= -->

<div class="flower f1">🌸</div>
<div class="flower f2">🌷</div>
<div class="flower f3">🌼</div>
<div class="flower f4">🌸</div>


<!-- =========================
     MAIN CARD
========================= -->

<div class="card" id="main">

    <div class="icon">
        🌸💗🌸
    </div>

    <h1>
       Hi Km!!!
    </h1>

    <p>

    🌷🌷🌷🌷🌷

        <br><br>

        I know things between us didn't turn out
        the way we once hoped, and I respect
        everything that happened.

        <br><br>

        I'm not asking to bring back the past
        or make things complicated.

        I just genuinely hope that someday,
        we can be okay with each other again.

    </p>


    <div class="question">

        can we just be friends? 🌷

    </div>


    <!-- BUTTONS -->

    <div class="button-area">

        <button
            class="yes"
            id="yesButton"
            onclick="sayYes()">

            YES 🌸

        </button>


        <button
            class="no"
            id="noButton"
            onclick="moveNo()">

            NO

        </button>

    </div>

</div>



<!-- =========================
     SUCCESS CARD
========================= -->

<div class="card" id="success">

    <div class="icon">
        🌸💗🌷
    </div>

    <h1>
        YEEEHEEEEYYY Thank You, Kiyyy!!🥳🥳
    </h1>


    <div class="message">

        I really appreciate it, bunjing. 💗

        <br><br>

        I know we're not the same as before,
        and I'm not asking for anything more
        than friendship.

        <br><br>

        I just want us to be comfortable around
        each other again, without any bad feelings
        or awkwardness.

        <br><br>

        Whatever happened between us is already
        part of the past.

        I still value the memories we had,
        and I hope we can make new ones someday,
        this time, as friends.

        <br><br>

        No pressure. I just wanted you to know. 🌷

    </div>


    <a
        href="#"
        class="back"
        onclick="goBack(); return false;">

        ← Go back

    </a>

</div>



<script>

/* =========================
   ELEMENTS
========================= */

const noButton =
    document.getElementById("noButton");

const mainCard =
    document.getElementById("main");

const successCard =
    document.getElementById("success");


/* =========================
   MOVE NO BUTTON
========================= */

function moveNo() {

    /*
       Make NO a floating button.
    */

    noButton.classList.add("running");


    /*
       Get button size.
    */

    const buttonWidth =
        noButton.offsetWidth;

    const buttonHeight =
        noButton.offsetHeight;


    /*
       Safe distance from screen edges.
    */

    const padding = 20;


    /*
       Calculate maximum
       possible position.
    */

    const maxX =
        window.innerWidth -
        buttonWidth -
        padding;

    const maxY =
        window.innerHeight -
        buttonHeight -
        padding;


    /*
       Generate random position.
    */

    const x =
        Math.floor(
            Math.random() *
            Math.max(1, maxX - padding)
        ) + padding;


    const y =
        Math.floor(
            Math.random() *
            Math.max(1, maxY - padding)
        ) + padding;


    /*
       Move NO.
    */

    noButton.style.left = x + "px";
    noButton.style.top = y + "px";

}


/* =========================
   YES BUTTON
========================= */

function sayYes() {

    /*
       Hide main card.
    */

    mainCard.style.display = "none";


    /*
       Hide NO button.
    */

    noButton.style.display = "none";


    /*
       Show success card.
    */

    successCard.classList.add("show");

}


/* =========================
   GO BACK
========================= */

function goBack() {

    /*
       Hide success card.
    */

    successCard.classList.remove("show");


    /*
       Show main card.
    */

    mainCard.style.display = "block";


    /*
       Show NO again.
    */

    noButton.style.display = "block";


    /*
       Return NO to its original
       perfectly aligned position.
    */

    noButton.classList.remove("running");

    noButton.style.left = "";
    noButton.style.top = "";

}

</script>

</body>
</html>
