<!DOCTYPE html>
<html lang="gu">
<head>
<meta charset="UTF-8">
<title>ગ્રામ અવાજ</title>

<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: linear-gradient(180deg, #87ceeb, #b3e5fc, #e1f5fe);
    overflow-x: hidden;
}

/* Floating light animation */
.lights {
    position: fixed;
    inset: 0;
    pointer-events: none;
    z-index: 0;
}
.light {
    position: absolute;
    width: 12px;
    height: 12px;
    background: rgba(255,255,255,0.8);
    border-radius: 50%;
    animation: float 12s linear infinite;
}
.light:nth-child(1){left:10%; animation-duration:14s;}
.light:nth-child(2){left:30%; animation-duration:10s;}
.light:nth-child(3){left:50%; animation-duration:16s;}
.light:nth-child(4){left:70%; animation-duration:11s;}
.light:nth-child(5){left:90%; animation-duration:13s;}

@keyframes float {
    0% { top: 100%; opacity: 0; }
    20% { opacity: 0.8; }
    50% { opacity: 0.4; }
    100% { top: -10%; opacity: 0; }
}

/* Right Sidebar Navigation */
nav {
    position: fixed;
    right: 0;
    top: 0;
    height: 100%;
    width: 180px;
    background: #0288d1;
    display: flex;
    flex-direction: column;
    padding-top: 20px;
    z-index: 2;
}

nav button {
    background: white;
    color: #0288d1;
    border: none;
    margin: 10px;
    padding: 10px;
    border-radius: 10px;
    font-weight: bold;
    cursor: pointer;
}

/* Main content */
main {
    margin-right: 200px;
    padding: 20px;
    position: relative;
    z-index: 1;
}

section { display: none; }
section.active { display: block; }

.container {
    background: rgba(255,255,255,0.95);
    max-width: 520px;
    margin: auto;
    padding: 20px;
    border-radius: 16px;
    box-shadow: 0 10px 25px rgba(0,0,0,0.25);
}

h2 {
    text-align: center;
    color: #01579b;
}

label {
    font-weight: bold;
    display: block;
    margin-top: 10px;
}

input, textarea, select {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
    border-radius: 8px;
    border: 2px solid #ddd;
}

button.main {
    width: 100%;
    padding: 12px;
    margin-top: 10px;
    background: linear-gradient(to right, #03a9f4, #0288d1);
    color: white;
    border: none;
    border-radius: 10px;
}

.voice {
    background: #2e7d32;
}

.problem {
    border: 2px solid #e3f2fd;
    padding: 12px;
    margin-top: 10px;
    border-radius: 10px;
    background: #f1f9ff;
}

.vote-btn {
    padding: 6px 10px;
    border-radius: 6px;
    border: none;
    margin-right: 8px;
    cursor: pointer;
}

.like { background: #2e7d32; color: white; }
.dislike { background: #c62828; color: white; }

.helpline p {
    background: #e3f2fd;
    padding: 10px;
    border-radius: 8px;
    margin: 8px 0;
}

canvas {
    margin-top: 20px;
    background: white;
    border-radius: 10px;
}
</style>
</head>

<body>

<!-- Light animation -->
<div class="lights">
    <div class="light"></div>
    <div class="light"></div>
    <div class="light"></div>
    <div class="light"></div>
    <div class="light"></div>
</div>

<nav>
    <button onclick="showSection('submit')">🕊️ ફરિયાદ</button>
    <button onclick="showSection('view')">📢 ફરિયાદો</button>
    <button onclick="showSection('graph')">📊 પરિણામ</button>
    <button onclick="showSection('help')">📞 Helpline</button>
</nav>

<main>

<!-- Submit Complaint -->
<section id="submit" class="active">
<div class="container">
<h2>નવી ફરિયાદ</h2>

<label>ફરિયાદનો પ્રકાર</label>
<select id="problemType">
    <option>પાણી</option>
    <option>વિજળી</option>
    <option>રસ્તા</option>
    <option>આરોગ્ય</option>
    <option>અન્ય</option>
</select>

<label>ફરિયાદ લખો અથવા બોલો</label>
<textarea id="text" rows="4"></textarea>

<button class="main voice" onclick="startGujaratiVoice()">🎤 બોલીને ફરિયાદ કરો</button>
<button class="main" onclick="addProblem()">📨 મોકલો</button>
</div>
</section>

<!-- View Complaints -->
<section id="view">
<div class="container">
<h2>ગામની ફરિયાદો</h2>
<div id="problemList"></div>
</div>
</section>

<!-- Graph -->
<section id="graph">
<div class="container">
<h2>સહમતિ પરિણામ</h2>
<canvas id="chart" width="400" height="300"></canvas>
</div>
</section>

<!-- Helpline -->
<section id="help">
<div class="container helpline">
<h2>જરૂરી સંપર્ક નંબર</h2>
<p>🔧 પ્લમ્બર – રમેશભાઈ પટેલ : 9876543210</p>
<p>⚡ ઇલેક્ટ્રિશિયન – મહેશભાઈ રાઠોડ : 9890123456</p>
<p>🧹 સફાઈ કર્મચારી – કિરણબેન ચૌધરી : 9784561230</p>
<p>🚰 પાણી કર્મચારી – વિનોદભાઈ સોલંકી : 9654321087</p>
</div>
</section>

</main>

<script>
let problems = [];

function showSection(id) {
    document.querySelectorAll("section").forEach(s => s.classList.remove("active"));
    document.getElementById(id).classList.add("active");
    if (id === "graph") drawGraph();
}

function addProblem() {
    const text = document.getElementById("text").value;
    if (!text) { alert("ફરિયાદ લખો"); return; }
    problems.push({ text, like: 0, dislike: 0 });
    document.getElementById("text").value = "";
    renderProblems();
}

function renderProblems() {
    const list = document.getElementById("problemList");
    list.innerHTML = "";
    problems.forEach((p, i) => {
        list.innerHTML += `
        <div class="problem">
            <p>${p.text}</p>
            <button class="vote-btn like" onclick="vote(${i},'like')">👍 ${p.like}</button>
            <button class="vote-btn dislike" onclick="vote(${i},'dislike')">👎 ${p.dislike}</button>
        </div>`;
    });
}

function vote(i, t) {
    problems[i][t]++;
    renderProblems();
}

function drawGraph() {
    const c = document.getElementById("chart");
    const ctx = c.getContext("2d");
    ctx.clearRect(0,0,c.width,c.height);
    problems.forEach((p,i)=>{
        ctx.fillStyle="#2e7d32";
        ctx.fillRect(60+i*90,250-p.like*20,25,p.like*20);
        ctx.fillStyle="#c62828";
        ctx.fillRect(90+i*90,250-p.dislike*20,25,p.dislike*20);
        ctx.fillStyle="#000";
        ctx.fillText(`P${i+1}`,70+i*90,270);
    });
}

function startGujaratiVoice() {
    if (!('webkitSpeechRecognition' in window)) {
        alert("Google Chrome વાપરો");
        return;
    }
    const r = new webkitSpeechRecognition();
    r.lang = "gu-IN";
    r.onresult = e => {
        document.getElementById("text").value += " " + e.results[0][0].transcript;
    };
    r.start();
}
</script>

</body>
</html>
