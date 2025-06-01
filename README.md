<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Normal Mode Training Cards + Game Mode</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #121212, #1e1e1e);
      color: white;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 30px;
      gap: 20px;
    }

    .card {
      background: linear-gradient(to bottom, #d45c99, #670097);
      border-radius: 20px;
      padding: 25px;
      width: 280px;
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.5);
      flex-shrink: 0;
    }

    .card h2 {
      font-size: 1.4em;
      margin-bottom: 10px;
    }

    .card h2 span {
      margin-right: 8px;
    }

    .card strong {
      display: block;
      margin-top: 15px;
      margin-bottom: 8px;
      font-size: 1em;
    }

    .card ul {
      margin: 0;
      padding-left: 20px;
    }

    .card p {
      font-style: italic;
      margin-top: 20px;
      border-top: 1px solid rgba(255, 255, 255, 0.3);
      padding-top: 10px;
      font-size: 0.95em;
    }

    /* Video container */
    .video-container {
      width: 560px;
      max-width: 100%;
      margin-bottom: 40px;
      flex-basis: 100%;
      display: flex;
      justify-content: center;
    }

    iframe {
      border-radius: 15px;
      box-shadow: 0 6px 20px rgba(0, 0, 0, 0.7);
      width: 100%;
      height: 315px;
    }

    /* Game mode styles */
    .game-mode {
      background: linear-gradient(to bottom, #2c3e50, #4ca1af);
      border-radius: 20px;
      padding: 30px;
      width: 600px;
      max-width: 100%;
      color: #fff;
      box-shadow: 0 8px 30px rgba(0,0,0,0.7);
      flex-basis: 100%;
    }

    .game-mode h2 {
      margin-top: 0;
      margin-bottom: 20px;
      font-size: 1.8em;
      text-align: center;
    }

    .question {
      font-size: 1.2em;
      margin-bottom: 20px;
    }

    .answers button {
      background: #670097;
      border: none;
      padding: 12px 20px;
      margin: 8px 12px 8px 0;
      border-radius: 12px;
      color: white;
      cursor: pointer;
      font-size: 1em;
      transition: background 0.3s;
    }
    .answers button:hover {
      background: #d45c99;
    }

    .explanation {
      margin-top: 20px;
      padding: 15px;
      background: rgba(0,0,0,0.5);
      border-radius: 10px;
      font-style: italic;
      display: none;
    }

    .next-btn {
      margin-top: 25px;
      background: #fff;
      color: #670097;
      border: none;
      padding: 12px 30px;
      border-radius: 20px;
      font-weight: bold;
      cursor: pointer;
      display: none;
      transition: background 0.3s;
    }
    .next-btn:hover {
      background: #d45c99;
      color: white;
    }

    /* Responsive */
    @media (max-width: 650px) {
      .game-mode {
        width: 100%;
      }
      .card {
        width: 100%;
      }
    }
  </style>
</head>
<body>

  <!-- Training Cards -->
  <div class="card">
    <h2><span>🛡️</span>Be Unstoppable to Guard</h2>
    <strong>When to Use:</strong>
    <ul>
      <li>Use strength vs small defenders</li>
      <li>Use speed vs bigger defenders</li>
      <li>1-on-1 situations</li>
    </ul>
    <strong>Training Drills:</strong>
    <ul>
      <li>1v1 King of the Court (wing/top/isolation)</li>
      <li>Shoulder Bump Finishes</li>
      <li>Speed Stop Pull-Ups (2 hard dribbles → stop → shoot)</li>
    </ul>
    <p>Nobody can match all my tools.</p>
  </div>

  <div class="card">
    <h2><span>🧊</span>Mental Toughness & Confidence</h2>
    <strong>When to Use:</strong>
    <ul>
      <li>You’re missing shots</li>
      <li>It’s crunch time</li>
      <li>Defenders try to frustrate you</li>
    </ul>
    <strong>Training Drills:</strong>
    <ul>
      <li>Free Throw Focus (10 makes in a row under pressure)</li>
      <li>Game-Winner Simulation (5-4-3 countdown situations)</li>
      <li>Self-Talk Reps (say focus phrase before attack/shoot)</li>
    </ul>
    <p>I'm built for this — win with heart and head.</p>
  </div>

  <div class="card">
    <h2><span>🔥</span>Explosive First Step</h2>
    <strong>When to Use:</strong>
    <ul>
      <li>Defender is flat-footed or leaning</li>
      <li>After a jab step or hesitation</li>
      <li>Right after a screen if the big is slow</li>
    </ul>
    <strong>Training Drills:</strong>
    <ul>
      <li>Jab Step + Explode (triple threat → jab → hard drive)</li>
      <li>Corner Sprint Finishes (start from corner → full drive + layup)</li>
      <li>1 Dribble Blow-Bys (attack off a jab or catch)</li>
    </ul>
    <p>The moment they freeze or lean, I’m gone.</p>
  </div>

  <div class="card">
    <h2><span>🎯</span>Three-Level Scoring</h2>
    <strong>When to Use:</strong>
    <ul>
      <li>Finish at the rim if help is late</li>
      <li>Pull-up mid-range when drive is cut off</li>
      <li>Shoot 3s if defender sags or you create space</li>
    </ul>
    <strong>Training Drills:</strong>
    <ul>
      <li>Mikan Variations (regular, reverse, extended)</li>
      <li>1-2 Pull-Ups (wing, elbow, top of the key)</li>
      <li>Catch + Shoot + Relocation Threes</li>
    </ul>
    <p>Wherever they’re weak, I’ll score from there.</p>
  </div>

  <div class="card">
    <h2><span>🧠</span>Ball Handling & Decision-Making</h2>
    <strong>When to Use:</strong>
    <ul>
      <li>When pressured tightly</li>
      <li>Running pick-and-rolls</li>
      <li>Driving and help rotates</li>
    </ul>
    <strong>Training Drills:</strong>
    <ul>
      <li>Figure 8 + Combo Moves (tight space ball control)</li>
      <li>Live 2-Dribble Reads (defender plays live help)</li>
      <li>1v1 Decisions (defender controls help or force baseline)</li>
    </ul>
    <p>Control the game — read, react, punish.</p>
  </div>

  <!-- Video Embed -->
  <div class="video-container">
    <iframe
      src="https://www.youtube.com/embed/EzP6j3igZl0?si=fRexcPH1_rT4oHY9"
      title="Anthony Edwards Offensive Moves"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen></iframe>
  </div>

  <!-- Game Mode Section -->
  <div class="game-mode">
    <h2>Game Mode: Simulate In-Game Situations</h2>
    <div class="question"></div>
    <div class="answers"></div>
    <button class="next-btn">Next Question</button>
    <div class="explanation"></div>
  </div>

  <script>
    // Questions for the game mode
    const questions = [
      {
        question: "Your defender is flat-footed after a jab step. What's your best move?",
        answers: [
          "Explosive first step to drive past",
          "Pull up for a three-pointer immediately",
          "Pass to a teammate",
          "Post up and back them down"
        ],
        correct: 0,
        explanation: "When the defender is flat-footed after a jab step, an explosive first step exploits their balance and allows you to blow by them quickly."
      },
      {
        question: "Help defense slides in to stop your drive. What's the best shot to take?",
        answers: [
          "Finish strong at the rim",
          "Kick out to the corner for a three",
          "Pull up mid-range jumper",
          "Turn back and reset the play"
        ],
        correct: 1,
        explanation: "If help defense slides in, the corner three is usually wide open and a high-percentage shot."
      },
      {
        question: "You face a bigger, slower defender after a screen. What should you do?",
        answers: [
          "Use strength to back them down",
          "Attack quickly using your speed",
          "Shoot a contested mid-range jumper",
          "Pass and cut to the basket"
        ],
        correct: 1,
        explanation: "Against a slower defender, using your speed immediately after the screen can create a mismatch and an easy scoring opportunity."
      },
      {
        question: "Your shot is off, and defenders are closing in. How do you stay confident?",
        answers: [
          "Take a timeout to regroup",
          "Use mental toughness drills and self-talk",
          "Try riskier shots",
          "Pass every time to avoid shooting"
        ],
        correct: 1,
        explanation: "Mental toughness and positive self-talk help you maintain confidence even when shots aren’t falling."
      },
      {
        question: "The paint is crowded. What's the best offensive move?",
        answers: [
          "Force your way through the defense",
          "Skip the ball and swing it back to reset spacing",
          "Take a quick contested shot",
          "Call for a timeout"
        ],
        correct: 1,
        explanation: "When the paint is packed, swinging the ball out resets spacing and opens new lanes for attack."
      }
    ];

    const questionEl = document.querySelector(".game-mode .question");
    const answersEl = document.querySelector(".game-mode .answers");
    const explanationEl = document.querySelector(".game-mode .explanation");
    const nextBtn = document.querySelector(".game-mode .next-btn");

    let currentQuestionIndex = 0;
    let answered = false;

    function showQuestion() {
      answered = false;
      explanationEl.style.display = "none";
      nextBtn.style.display = "none";

      const q = questions[currentQuestionIndex];
      questionEl.textContent = q.question;
      answersEl.innerHTML = "";

      q.answers.forEach((answer, i) => {
        const btn = document.createElement("button");
        btn.textContent = answer;
        btn.onclick = () => selectAnswer(i);
        answersEl.appendChild(btn);
      });
    }

    function selectAnswer(selectedIndex) {
      if (answered) return;
      answered = true;

      const q = questions[currentQuestionIndex];

      // Disable buttons
      [...answersEl.children].forEach(btn => btn.disabled = true);

      // Mark correct and wrong answers
      [...answersEl.children].forEach((btn, i) => {
        if (i === q.correct) {
          btn.style.backgroundColor = "#28a745"; // green
        } else if (i === selectedIndex) {
          btn.style.backgroundColor = "#dc3545"; // red
        }
      });

      explanationEl.textContent = q.explanation;
      explanationEl.style.display = "block";
      nextBtn.style.display = "inline-block";
    }

    nextBtn.onclick = () => {
      currentQuestionIndex++;
      if (currentQuestionIndex >= questions.length) {
        questionEl.textContent = "Great job! You've completed the game mode.";
        answersEl.innerHTML = "";
        explanationEl.style.display = "none";
        nextBtn.style.display = "none";
      } else {
        showQuestion();
      }
    };

    // Start the first question
    showQuestion();
  </script>

</body>
</html>
