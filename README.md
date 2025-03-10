<script>
    const text = [
        "Initializing system...",
        "Checking user compatibility...",
        "Analyzing emotions...",
        "Processing love data...",
        "User detected: My Love ❤",
        "Executing final command...",
        "Will you marry me? 💍❤"
    ];

    let index = 0;
    function typeText() {
        if (index < text.length) {
            document.getElementById("output").innerHTML += text[index] + "\n";
            index++;
            setTimeout(typeText, 1000);
        } else {
            document.getElementById("yesBtn").style.display = "block";
        }
    }

    function showGif() {
        document.body.innerHTML = `
            <div style="text-align: center; margin-top: 50px;">
                <h1 style="color: limegreen; font-family: 'Courier New', monospace;">
                    Yay! You said YES! ❤
                </h1>
                <img src="https://media.giphy.com/media/3oz8xKaR836UJOYeOc/giphy.gif" 
                     alt="Happy GIF" 
                     style="width: 50%; max-width: 400px; border-radius: 10px;">
            </div>`;
    }

    document.getElementById("yesBtn").addEventListener("click", showGif);

    typeText();
</script>
