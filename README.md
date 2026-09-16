<!DOCTYPE html>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

```
<title>Pranshu Shukla | GitHub</title>

<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    body {
        min-height: 100vh;
        background: #0b0f14;
        color: #ffffff;
        font-family: Arial, Helvetica, sans-serif;

        display: flex;
        justify-content: center;
        align-items: center;

        overflow: hidden;
    }

    /* Background glow */
    body::before {
        content: "";
        position: fixed;
        width: 500px;
        height: 500px;
        background: #5865f2;
        filter: blur(180px);
        opacity: 0.12;
        top: -200px;
        left: -150px;
        z-index: -1;
    }

    body::after {
        content: "";
        position: fixed;
        width: 450px;
        height: 450px;
        background: #00d4ff;
        filter: blur(180px);
        opacity: 0.08;
        bottom: -200px;
        right: -150px;
        z-index: -1;
    }

    .container {
        width: 90%;
        max-width: 850px;
        text-align: center;
        padding: 60px 30px;
    }

    /* Name */
    .name {
        font-size: clamp(40px, 7vw, 72px);
        font-weight: 800;
        letter-spacing: -2px;
        margin-bottom: 15px;
    }

    .name span {
        background: linear-gradient(90deg, #ffffff, #8ab4ff);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    /* Subtitle */
    .subtitle {
        font-size: 18px;
        color: #9ca3af;
        letter-spacing: 2px;
        margin-bottom: 45px;
    }

    /* Typewriter */
    .typewriter {
        font-size: clamp(22px, 4vw, 38px);
        font-weight: 600;
        margin-bottom: 18px;

        min-height: 48px;
    }

    .typewriter-text {
        color: #ffffff;
    }

    .cursor {
        display: inline-block;
        width: 3px;
        height: 35px;
        background: #7c9cff;
        margin-left: 5px;
        vertical-align: middle;

        animation: blink 0.8s infinite;
    }

    @keyframes blink {
        0%, 50% {
            opacity: 1;
        }

        51%, 100% {
            opacity: 0;
        }
    }

    /* Description */
    .description {
        color: #8b949e;
        font-size: 16px;
        line-height: 1.7;
        max-width: 600px;
        margin: 0 auto 35px;
    }

    /* Social buttons */
    .links {
        display: flex;
        justify-content: center;
        gap: 14px;
        flex-wrap: wrap;
    }

    .links a {
        text-decoration: none;
        color: #ffffff;

        padding: 12px 22px;
        border: 1px solid #30363d;
        border-radius: 10px;

        background: rgba(255, 255, 255, 0.03);

        transition: 0.25s ease;
    }

    .links a:hover {
        transform: translateY(-3px);
        border-color: #7c9cff;
        background: rgba(124, 156, 255, 0.1);
        box-shadow: 0 8px 30px rgba(124, 156, 255, 0.12);
    }

    /* Footer */
    .footer {
        margin-top: 55px;
        font-size: 13px;
        color: #555d66;
    }

    /* Mobile */
    @media (max-width: 600px) {

        .container {
            padding: 40px 20px;
        }

        .subtitle {
            font-size: 14px;
        }

        .description {
            font-size: 14px;
        }

        .cursor {
            height: 25px;
        }
    }
</style>
```

</head>

<body>

```
<main class="container">

    <!-- YOUR NAME -->
    <h1 class="name">
        <span>Pranshu Shukla</span>
    </h1>

    <!-- YOUR ROLE -->
    <p class="subtitle">
        Tech Enthusiast | Aspiring Web Developer
    </p>

    <!-- TYPEWRITER -->
    <div class="typewriter">
        <span class="typewriter-text"></span>
        <span class="cursor"></span>
    </div>

    <!-- DESCRIPTION -->
    <p class="description">
        Exploring technology, learning new things, and building my skills
        one step at a time.
    </p>

    <!-- LINKS -->
    <div class="links">

        <a href="https://github.com/PranshuuShuklaa" target="_blank">
            GitHub
        </a>

        <a href="https://www.linkedin.com/in/pranshushukla8408/" target="_blank">
            LinkedIn
        </a>

        <a href="mailto:pranshushukla842008@gmail.com">
            Email
        </a>

    </div>

</main>


<script>

    /* =========================================
       TYPEWRITER EFFECT
       ========================================= */

    const text = "Learning Every Piece Of Tech Exists.";
    const typewriter = document.querySelector(".typewriter-text");

    let index = 0;

    function typeEffect() {

        if (index < text.length) {

            typewriter.textContent += text.charAt(index);

            index++;

            setTimeout(typeEffect, 75);

        }

    }

    typeEffect();

</script>
```

</body>
</html>
