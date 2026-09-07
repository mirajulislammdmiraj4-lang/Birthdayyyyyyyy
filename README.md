<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Juthi 🤍</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600;700&display=swap" rel="stylesheet">
</head>
<body>

    <!-- Hanging Banner Decor -->
    <div class="bunting"></div>

    <div class="card-wrapper">
        <!-- Step 1: Title Section -->
        <div id="step-1" class="step-box hidden">
            <h1 class="main-title">
                Happy<br>
                <span>Birthday</span>
            </h1>
        </div>

        <!-- Step 2: Date Badge -->
        <div id="step-2" class="step-box hidden">
            <div class="date-badge">3 November 2009</div>
        </div>

        <!-- Step 3: Bear Avatar & Name -->
        <div id="step-3" class="step-box hidden">
            <div class="avatar-box">
                <div class="bear-emoji">🧸</div>
            </div>
            <div class="name-tag">Juthi! 🤍</div>
        </div>

        <!-- Step 4: Click Here Button -->
        <div id="step-4" class="step-box hidden">
            <button class="click-btn" onclick="openWishLetter()">Click here 🤍</button>
            <div class="smile">😊</div>
        </div>
    </div>

    <!-- Step 5: Popup Wish Modal -->
    <div id="wishModal" class="modal-overlay">
        <div class="modal-card">
            <span class="close-btn" onclick="closeWishLetter()">&times;</span>
            <div class="modal-header">
                <h3>Happy Birthday, Juthi 🤍✨</h3>
            </div>
            <div class="modal-body">
                <div class="decor-emoji">🧸🎈</div>
                <div class="letter-text">
                    <p>If I had to describe what you mean to me, I don't think a few words would ever be enough. You are not just someone I talk to every day; you are someone whose happiness genuinely matters to me. 🥹🤍</p>

                    <p>Life won't always be easy. There will be good days, difficult days, misunderstandings, stressful moments, and days when everything feels too much. But I hope that no matter how difficult life becomes, we never forget the importance of standing beside each other. ✨</p>

                    <p>I want you to know that whenever you need someone, I will try my best to be that person for you. And I hope that whenever I need you, you will hold my hand and remind me that I am not alone. 🤍🫶🏻</p>

                    <p>Let's promise to support each other's dreams, respect each other's feelings, and stay beside each other through every difficult chapter. Because sometimes the greatest gift isn't being together only on the happiest days—it's choosing to stay when things aren't easy. 🌷✨</p>

                    <p>On your birthday, I wish you endless happiness, success, peace, and countless beautiful memories.</p>

                    <p><b>Happy Birthday, Juthi. 🎂🤍✨</b><br>
                    No matter how life changes, I hope we always find our way back to each other.</p>

                    <p>Stay beside me, and I promise I'll keep standing beside you too. Through every high and every low, we'll face life together. 🤍✨</p>
                </div>
            </div>
        </div>
    </div>

    <script src="script.js"></script>
</body>
</html>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Fredoka', sans-serif;
}

body {
    background-color: #fbe3eb;
    background-image: radial-gradient(#f7cee0 1.5px, transparent 1.5px);
    background-size: 20px 20px;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    position: relative;
}

.bunting {
    position: absolute;
    top: 0;
    width: 100%;
    height: 45px;
    background: repeating-linear-gradient(
        -45deg,
        #ff94b9 0px,
        #ff94b9 15px,
        transparent 15px,
        transparent 30px
    );
    opacity: 0.7;
}

.card-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 15px;
    z-index: 2;
}

.hidden {
    display: none !important;
}

.show-step {
    display: flex !important;
    flex-direction: column;
    align-items: center;
    animation: zoomIn 0.6s cubic-bezier(0.175, 0.885, 0.32, 1.275) forwards;
}

@keyframes zoomIn {
    0% {
        opacity: 0;
        transform: scale(0.5) translateY(20px);
    }
    100% {
        opacity: 1;
        transform: scale(1) translateY(0);
    }
}

.main-title {
    font-size: 3rem;
    color: #ffffff;
    text-shadow: -2px -2px 0 #ff5c8d, 2px -2px 0 #ff5c8d, -2px 2px 0 #ff5c8d, 2px 2px 0 #ff5c8d, 4px 4px 0px #e64a75;
    line-height: 1.1;
    text-align: center;
}

.main-title span {
    color: #ff5c8d;
    text-shadow: -2px -2px 0 #fff, 2px -2px 0 #fff, -2px 2px 0 #fff, 2px 2px 0 #fff, 3px 3px 0px #d6406c;
}

.date-badge {
    background-color: #ff85a2;
    color: #fff;
    padding: 6px 18px;
    border-radius: 20px;
    font-size: 0.9rem;
    box-shadow: 0 4px 6px rgba(0,0,0,0.05);
}

.avatar-box {
    width: 120px;
    height: 120px;
    background-color: #ffffff;
    border: 3px solid #ff85a2;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 55px;
    box-shadow: 0 6px 12px rgba(0,0,0,0.08);
}

.name-tag {
    background-color: #ff5c8d;
    color: white;
    padding: 4px 16px;
    border-radius: 12px;
    font-size: 0.85rem;
    margin-top: -12px;
    text-align: center;
}

.click-btn {
    background-color: #ff5c8d;
    color: white;
    border: none;
    padding: 8px 20px;
    border-radius: 20px;
    font-size: 0.95rem;
    font-weight: 600;
    cursor: pointer;
    box-shadow: 0 4px 10px rgba(255, 92, 141, 0.3);
    transition: transform 0.2s;
}

.click-btn:hover {
    transform: scale(1.08);
}

.smile {
    font-size: 1.4rem;
    text-align: center;
    margin-top: 5px;
}

/* Floating White Hearts 🤍 */
.white-heart {
    position: absolute;
    font-size: 1.3rem;
    user-select: none;
    pointer-events: none;
    animation: floatUp 4s linear infinite;
}

@keyframes floatUp {
    0% {
        transform: translateY(100vh) scale(0.5);
        opacity: 0.9;
    }
    100% {
        transform: translateY(-10vh) scale(1.2);
        opacity: 0;
    }
}

/* Modal Popup Window */
.modal-overlay {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.4);
    justify-content: center;
    align-items: center;
    z-index: 10;
}

.modal-card {
    background: #ffffff;
    padding: 20px;
    border-radius: 20px;
    width: 90%;
    max-width: 420px;
    max-height: 80vh;
    border: 3px dashed #ff85a2;
    position: relative;
    box-shadow: 0 10px 25px rgba(0,0,0,0.15);
    animation: popIn 0.3s ease-out;
    display: flex;
    flex-direction: column;
}

@keyframes popIn {
    from { transform: scale(0.7); opacity: 0; }
    to { transform: scale(1); opacity: 1; }
}

.close-btn {
    position: absolute;
    top: 10px;
    right: 15px;
    font-size: 24px;
    cursor: pointer;
    color: #ff85a2;
}

.modal-header h3 {
    color: #ff5c8d;
    font-size: 1.3rem;
    text-align: center;
    margin-top: 5px;
}

.modal-body {
    margin-top: 10px;
    text-align: center;
    overflow-y: auto;
    padding-right: 5px;
}

.decor-emoji {
    font-size: 35px;
    margin-bottom: 5px;
}

.letter-text p {
    color: #555;
    font-size: 0.9rem;
    line-height: 1.5;
    margin-bottom: 12px;
}
// Step-by-Step Sequential Animation Trigger
document.addEventListener("DOMContentLoaded", function () {
    setTimeout(() => showStep("step-1"), 500);   // Show Title
    setTimeout(() => showStep("step-2"), 2000);  // Show Date (3 November 2009)
    setTimeout(() => showStep("step-3"), 3500);  // Show Bear & Name
    setTimeout(() => showStep("step-4"), 5000);  // Show Click Here Button
});

function showStep(id) {
    const el = document.getElementById(id);
    if (el) {
        el.classList.remove("hidden");
        el.classList.add("show-step");
    }
}

// Open Wish Letter Modal
function openWishLetter() {
    document.getElementById("wishModal").style.display = "flex";
}

// Close Wish Letter Modal
function closeWishLetter() {
    document.getElementById("wishModal").style.display = "none";
}

// Floating White Hearts Background Animation 🤍
function createWhiteHeart() {
    const heart = document.createElement('div');
    heart.classList.add('white-heart');
    heart.innerText = '🤍';
    
    heart.style.left = Math.random() * 100 + 'vw';
    heart.style.animationDuration = (Math.random() * 2 + 3) + 's';
    
    document.body.appendChild(heart);
    
    setTimeout(() => {
        heart.remove();
    }, 5000);
}

setInterval(createWhiteHeart, 300);
