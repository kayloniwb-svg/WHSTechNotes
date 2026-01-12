# August 27, 2025

Today, I created my first GitHub account and repository. I'm excited to start using GitHub for my projects!


# September 2, 2025
 New laws limiting cell phone use while driving, such as hands-free mandates and full handheld bans, are an essential public safety measure proven to reduce traffic accidents and fatalities.  According to the National Highway Traffic Safety Administration (NHTSA), studies in states that enacted handheld cell phone bans have shown a reduction in motor vehicle-related emergency department visits. Furthermore, data collected by organizations like the Governors Highway Safety Association (GHSA) consistently show that handheld bans, which are easier to enforce than texting-only bans, lead to a measurable decrease in drivers using their phones.  These findings directly support the claim that stricter cell phone laws increase safety by forcing drivers to keep their hands on the wheel and their attention focused solely on the road. Distracted driving, often caused by cell phone use, significantly impairs a driver's reaction time and cognitive function, making them a hazard to themselves and others. By legally prohibiting this dangerous behavior, states effectively mandate safer driving habits, leading to a demonstrable improvement in overall road safety statistics and preventing preventable tragedies.


# September 8, 2025

 Computer science is a valuable asset in the profession of sports analytics, empowering teams to gain a competitive edge. By leveraging data analysis, machine learning, and advanced algorithms, computer science helps teams make data-driven decisions that enhance player performance, optimize game strategies, and inform player recruitment.
 For example, professional sports teams now rely on data scientists and computer scientists to analyze large datasets of player and game statistics. A concrete instance is how advanced statistical models, developed through computer science, revolutionized Major League Baseball by allowing teams to identify and recruit undervalued players. Computer-generated analytics evaluate player performance beyond traditional stats like batting average. This helps to identify undervalued players and make better decisions, mirroring how professional teams find hidden talent.
 Computer science inteGRATion allows for sophisticated predictive modeling and data visualization, going beyond simple statistical analysis. This gives teams the ability to anticipate outcomes and visualize complex data in an understandable way for coaches and players. Computer science provides actionable insights based on robust data, allowing sports organizations to move beyond intuition and tradition, which leads to more strategic, informed, and ultimately, more successful decisions.

# September 15, 2025


An AI-powered nutritional assistant, “NutriSense,” would analyze user-inputted food photos and provide immediate, personalized dietary feedback based on health goals. The system would meet requirements by using computer vision to identify foods and apply machine learning algorithms to assess nutritional content against the user's specific health profile, such as managing diabetes or weight. NutriSense would be useful by offering real-time, actionable health information that helps individuals make better food choices, thereby promoting healthier lifestyles and potentially reducing the incidence of diet-related health issues.


# September 22, 2025

I feel like saying no to this because poeple can abuse the privilege of this and can get credit for it.On the other hand,This can be a benefit to people who cant handle working in person,this can help with young workers.Another thing is that thid can be useless for most people,like roblox os a child age game,or higher,this can get macroed with onine abusers,hackers and mess up the co workers work space,this can cause issues.



# September 30, 2025

The phrase "6, 7" is an internet meme originating from the song "Doot Doot (6 7)" by rapper Skrilla. It is often repeated with a specific hand motion. The phrase, sometimes paired with edits of basketball players like LaMelo Ball, is intentionally nonsensical. Its humor comes from being a shared inside joke that adults typically don't understand. Students repeat it playfully and randomly in conversations or hallways, sometimes as an ironic, unserious punchline. The mood is goofy, and its meaninglessness is entirely the point.


# October 6, 2025

As the leader of our school, my technology and AI policy would balance innovation with focus. We would implement a "phones away for the day" policy, requiring students to store their personal cell phones in lockers or designated pouches to eliminate distractions during class time [1]. School-provided Chromebooks would be the primary tools for classwork, used responsibly for educational purposes only, with robust filtering systems in place to block non-academic sites and online games, except for a curated list of approved, teacher-vetted learning and math games that enhance curriculum engagement [1]. AI tools like ChatGPT would be integrated as aids for learning and drafting, not for final assessments, teaching students how to use them ethically as research partners rather than cheating mechanisms [1]. This approach fosters an environment of deep learning, digital citizenship, and collaboration, preparing students for a technology-driven world while ensuring they master foundational skills [1]. The clear boundaries promote better academic performance, reduce anxiety associated with constant connectivity, and encourage face-to-face interaction and critical thinking [1]. Ultimately, this policy is designed to make technology a powerful servant to education, not its master, creating a more focused and engaging school environment for everyone [1].

# October 14, 2025

<!doctype html>
<html lang="en">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Math Challenge Game</title>
  <script src="/_sdk/element_sdk.js"></script>
  <style>
    body {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      height: 100%;
      font-family: 'Arial', sans-serif;
    }
    
    html {
      height: 100%;
    }
    
    * {
      box-sizing: border-box;
    }
  </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
  <script src="https://cdn.tailwindcss.com" type="text/javascript"></script>
 </head>
 <body>
  <div id="app"></div>
  <script>
    const defaultConfig = {
      background_color: '#4f46e5',
      card_color: '#ffffff',
      text_color: '#1f2937',
      primary_button_color: '#10b981',
      secondary_button_color: '#6366f1',
      font_family: 'Arial',
      font_size: 16,
      game_title: 'Math Challenge',
      score_label: 'Score',
      streak_label: 'Streak',
      submit_button: 'Submit Answer',
      new_problem_button: 'New Problem'
    };

    let score = 0;
    let streak = 0;
    let currentProblem = null;
    let userAnswer = '';
    let showFeedback = false;
    let feedbackMessage = '';
    let isCorrect = false;

    function generateProblem() {
      const operations = ['+', '-', '×', '÷'];
      const operation = operations[Math.floor(Math.random() * operations.length)];
      let num1, num2, answer;

      switch(operation) {
        case '+':
          num1 = Math.floor(Math.random() * 50) + 1;
          num2 = Math.floor(Math.random() * 50) + 1;
          answer = num1 + num2;
          break;
        case '-':
          num1 = Math.floor(Math.random() * 50) + 20;
          num2 = Math.floor(Math.random() * num1);
          answer = num1 - num2;
          break;
        case '×':
          num1 = Math.floor(Math.random() * 12) + 1;
          num2 = Math.floor(Math.random() * 12) + 1;
          answer = num1 * num2;
          break;
        case '÷':
          num2 = Math.floor(Math.random() * 10) + 2;
          answer = Math.floor(Math.random() * 12) + 1;
          num1 = num2 * answer;
          break;
      }

      return { num1, num2, operation, answer };
    }

    function checkAnswer() {
      const userNum = parseInt(userAnswer);
      if (isNaN(userNum)) {
        feedbackMessage = 'Please enter a valid number!';
        isCorrect = false;
        showFeedback = true;
        render();
        return;
      }

      if (userNum === currentProblem.answer) {
        score += 10;
        streak += 1;
        feedbackMessage = '🎉 Correct! Great job!';
        isCorrect = true;
      } else {
        streak = 0;
        feedbackMessage = `❌ Not quite. The answer was ${currentProblem.answer}`;
        isCorrect = false;
      }
      
      showFeedback = true;
      render();
    }

    function newProblem() {
      currentProblem = generateProblem();
      userAnswer = '';
      showFeedback = false;
      feedbackMessage = '';
      render();
      document.getElementById('answer-input').focus();
    }

    function handleInput(e) {
      userAnswer = e.target.value;
    }

    function handleSubmit(e) {
      e.preventDefault();
      if (!showFeedback && userAnswer.trim()) {
        checkAnswer();
      }
    }

    function render() {
      const config = window.elementSdk?.config || defaultConfig;
      const customFont = config.font_family || defaultConfig.font_family;
      const baseSize = config.font_size || defaultConfig.font_size;
      const baseFontStack = 'Arial, sans-serif';

      const app = document.getElementById('app');
      app.style.cssText = `
        min-height: 100%;
        background: ${config.background_color || defaultConfig.background_color};
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 24px;
        font-family: ${customFont}, ${baseFontStack};
      `;

      app.innerHTML = `
        <div style="
          background: ${config.card_color || defaultConfig.card_color};
          border-radius: 16px;
          padding: 40px;
          box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
          max-width: 500px;
          width: 100%;
        ">
          <h1 style="
            margin: 0 0 32px 0;
            color: ${config.text_color || defaultConfig.text_color};
            font-size: ${baseSize * 2}px;
            text-align: center;
            font-family: ${customFont}, ${baseFontStack};
          ">${config.game_title || defaultConfig.game_title}</h1>

          <div style="
            display: flex;
            justify-content: space-around;
            margin-bottom: 32px;
            gap: 16px;
          ">
            <div style="
              text-align: center;
              padding: 16px;
              background: ${config.background_color || defaultConfig.background_color}15;
              border-radius: 12px;
              flex: 1;
            ">
              <div style="
                font-size: ${baseSize * 0.85}px;
                color: ${config.text_color || defaultConfig.text_color}99;
                margin-bottom: 4px;
                font-family: ${customFont}, ${baseFontStack};
              ">${config.score_label || defaultConfig.score_label}</div>
              <div style="
                font-size: ${baseSize * 1.75}px;
                font-weight: bold;
                color: ${config.text_color || defaultConfig.text_color};
                font-family: ${customFont}, ${baseFontStack};
              ">${score}</div>
            </div>
            <div style="
              text-align: center;
              padding: 16px;
              background: ${config.background_color || defaultConfig.background_color}15;
              border-radius: 12px;
              flex: 1;
            ">
              <div style="
                font-size: ${baseSize * 0.85}px;
                color: ${config.text_color || defaultConfig.text_color}99;
                margin-bottom: 4px;
                font-family: ${customFont}, ${baseFontStack};
              ">${config.streak_label || defaultConfig.streak_label}</div>
              <div style="
                font-size: ${baseSize * 1.75}px;
                font-weight: bold;
                color: ${config.text_color || defaultConfig.text_color};
                font-family: ${customFont}, ${baseFontStack};
              ">${streak} 🔥</div>
            </div>
          </div>

          <div style="
            background: ${config.background_color || defaultConfig.background_color}10;
            padding: 32px;
            border-radius: 12px;
            margin-bottom: 24px;
            text-align: center;
          ">
            <div style="
              font-size: ${baseSize * 2.5}px;
              font-weight: bold;
              color: ${config.text_color || defaultConfig.text_color};
              margin-bottom: 24px;
              font-family: ${customFont}, ${baseFontStack};
            ">
              ${currentProblem.num1} ${currentProblem.operation} ${currentProblem.num2} = ?
            </div>

            <form id="answer-form" style="margin-bottom: 16px;">
              <label for="answer-input" style="
                display: block;
                font-size: ${baseSize * 0.85}px;
                color: ${config.text_color || defaultConfig.text_color};
                margin-bottom: 8px;
                font-family: ${customFont}, ${baseFontStack};
              ">Your Answer:</label>
              <input 
                type="number" 
                id="answer-input"
                value="${userAnswer}"
                ${showFeedback ? 'disabled' : ''}
                style="
                  width: 100%;
                  padding: 16px;
                  font-size: ${baseSize * 1.25}px;
                  border: 2px solid ${config.background_color || defaultConfig.background_color}30;
                  border-radius: 8px;
                  text-align: center;
                  font-family: ${customFont}, ${baseFontStack};
                  color: ${config.text_color || defaultConfig.text_color};
                  ${showFeedback ? 'opacity: 0.6;' : ''}
                "
              />
            </form>

            ${showFeedback ? `
              <div style="
                padding: 16px;
                border-radius: 8px;
                background: ${isCorrect ? '#10b98120' : '#ef444420'};
                color: ${config.text_color || defaultConfig.text_color};
                font-size: ${baseSize}px;
                margin-bottom: 16px;
                font-family: ${customFont}, ${baseFontStack};
              ">
                ${feedbackMessage}
              </div>
            ` : ''}

            ${!showFeedback ? `
              <button id="submit-btn" style="
                width: 100%;
                padding: 16px 32px;
                font-size: ${baseSize}px;
                font-weight: bold;
                color: white;
                background: ${config.primary_button_color || defaultConfig.primary_button_color};
                border: none;
                border-radius: 8px;
                cursor: pointer;
                transition: all 0.2s;
                font-family: ${customFont}, ${baseFontStack};
              ">${config.submit_button || defaultConfig.submit_button}</button>
            ` : `
              <button id="next-btn" style="
                width: 100%;
                padding: 16px 32px;
                font-size: ${baseSize}px;
                font-weight: bold;
                color: white;
                background: ${config.secondary_button_color || defaultConfig.secondary_button_color};
                border: none;
                border-radius: 8px;
                cursor: pointer;
                transition: all 0.2s;
                font-family: ${customFont}, ${baseFontStack};
              ">${config.new_problem_button || defaultConfig.new_problem_button}</button>
            `}
          </div>
        </div>
      `;

      const form = document.getElementById('answer-form');
      if (form) {
        form.addEventListener('submit', handleSubmit);
      }

      const input = document.getElementById('answer-input');
      if (input) {
        input.addEventListener('input', handleInput);
      }

      const submitBtn = document.getElementById('submit-btn');
      if (submitBtn) {
        submitBtn.addEventListener('click', checkAnswer);
        submitBtn.addEventListener('mouseenter', function() {
          this.style.transform = 'translateY(-2px)';
          this.style.boxShadow = '0 4px 12px rgba(16, 185, 129, 0.4)';
        });
        submitBtn.addEventListener('mouseleave', function() {
          this.style.transform = 'translateY(0)';
          this.style.boxShadow = 'none';
        });
      }

      const nextBtn = document.getElementById('next-btn');
      if (nextBtn) {
        nextBtn.addEventListener('click', newProblem);
        nextBtn.addEventListener('mouseenter', function() {
          this.style.transform = 'translateY(-2px)';
          this.style.boxShadow = '0 4px 12px rgba(99, 102, 241, 0.4)';
        });
        nextBtn.addEventListener('mouseleave', function() {
          this.style.transform = 'translateY(0)';
          this.style.boxShadow = 'none';
        });
      }
    }

    async function onConfigChange(config) {
      render();
    }

    if (window.elementSdk) {
      window.elementSdk.init({
        defaultConfig,
        onConfigChange,
        mapToCapabilities: (config) => ({
          recolorables: [
            {
              get: () => config.background_color || defaultConfig.background_color,
              set: (value) => {
                config.background_color = value;
                window.elementSdk.setConfig({ background_color: value });
              }
            },
            {
              get: () => config.card_color || defaultConfig.card_color,
              set: (value) => {
                config.card_color = value;
                window.elementSdk.setConfig({ card_color: value });
              }
            },
            {
              get: () => config.text_color || defaultConfig.text_color,
              set: (value) => {
                config.text_color = value;
                window.elementSdk.setConfig({ text_color: value });
              }
            },
            {
              get: () => config.primary_button_color || defaultConfig.primary_button_color,
              set: (value) => {
                config.primary_button_color = value;
                window.elementSdk.setConfig({ primary_button_color: value });
              }
            },
            {
              get: () => config.secondary_button_color || defaultConfig.secondary_button_color,
              set: (value) => {
                config.secondary_button_color = value;
                window.elementSdk.setConfig({ secondary_button_color: value });
              }
            }
          ],
          borderables: [],
          fontEditable: {
            get: () => config.font_family || defaultConfig.font_family,
            set: (value) => {
              config.font_family = value;
              window.elementSdk.setConfig({ font_family: value });
            }
          },
          fontSizeable: {
            get: () => config.font_size || defaultConfig.font_size,
            set: (value) => {
              config.font_size = value;
              window.elementSdk.setConfig({ font_size: value });
            }
          }
        }),
        mapToEditPanelValues: (config) => new Map([
          ['game_title', config.game_title || defaultConfig.game_title],
          ['score_label', config.score_label || defaultConfig.score_label],
          ['streak_label', config.streak_label || defaultConfig.streak_label],
          ['submit_button', config.submit_button || defaultConfig.submit_button],
          ['new_problem_button', config.new_problem_button || defaultConfig.new_problem_button]
        ])
      });
    }

    currentProblem = generateProblem();
    render();
  </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'996b5c0dd36868e0',t:'MTc2MTgzMTk5NC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>





# october 20, 2025

| Name     | Class | Seat |
| :------- | :---- | :--- |
| Franklin |  second     |91A      |
| Hardeep  |      third | 61F     |
| Marla    |     first  |   35B   |



# October 27, 2025

Technology plays a pivotal role in every stage of a natural disaster, from early detection to long-term recovery. Before a hurricane, for example, satellite technology and Doppler radar are crucial for forecasting the storm's path and intensity, allowing the National Hurricane Center to issue timely warnings [1]. During the event, smartphone apps and emergency alert systems deliver these life-saving warnings directly to individuals, providing real-time instructions on evacuation routes and shelter locations, while battery-operated or hand-crank radios offer a reliable communication lifeline if the power grid fails [1]. After the storm, social media platforms and services like the American Red Cross's "Safe and Well" list help loved ones reconnect, and drones are used by first responders to assess damage in hard-to-reach areas and locate survivors more efficiently [1]. These tools collectively save lives by providing actionable information and facilitating a coordinated response.

# November 3, 2025


When the SNAP program faces funding disruptions, as occurred over this past weekend due to a government shutdown, millions of low-income families and vulnerable individuals struggle to afford food, making it a critical issue. The primary problem is the immediate loss of a key safety net, which forces people to go hungry, buy cheaper, less nutritious food, or turn to already-strained food banks, leading to increased food insecurity and potential health and educational impacts. Technology could help by powering apps or websites that instantly connect people to local food banks, free meal programs, and grocers with available stock, potentially using real-time inventory and navigation features. Furthermore, community alert systems could use text messages to notify users about emergency food distribution sites, bypassing the need for a constant internet connection. However, significant challenges exist, as many low-income individuals lack reliable internet access or smartphones, and privacy concerns regarding location data or personal information could hinder adoption. If I were the designer, I would create a simple, text-message-based system accessible via any mobile phone, ensuring maximum reach and minimal technical barriers during a crisis.


# November 10, 2025

Thanksgiving break is something many people look forward to for various reasons like spending time with family, enjoying holiday food and traditions, and getting a rest from school or work.but i dont really celebrate.





# December 1, 2025

A real job that uses drones is a Drone Software Engineer, who creates the programs and algorithms that control drone operations. In this role, coding in languages like Python and C++ is essential for developing flight control software, programming autonomous navigation and obstacle avoidance systems, and integrating sensors like GPS and cameras. Software engineers enable drones to process data in real-time, making intelligent decisions without constant human input for tasks such as environmental monitoring, surveillance, or delivery services.
Regarding compensation, the average annual salary for a Drone Software Engineer in the United States is approximately \$147,524, with top earners making over \$200,000 annually, according to a November 2025 ZipRecruiter report. Educational requirements for this career typically include a bachelor's degree in computer science, aerospace engineering, or a related technical field. Additionally, an FAA Part 107 Remote Pilot Certificate is often required for testing and operating drones in a commercial capacity.



# December 8, 2025

 **A self-driving car might fail to recognize a stopped school bus because its perception system—cameras and LiDAR—struggles with the school bus stop arm, a relatively small, dynamic object [1]. The AI's training data might be insufficient to cover all lighting conditions or angles, or the stop arm's motion against complex urban backgrounds could confuse the car's object classification models [1]. The primary challenge lies in the AI accurately interpreting the meaning of the flashing red lights and the extended arm as a legal requirement to stop, not just another object to navigate around [1]. As a Waymo programmer, one safety improvement would be to implement a dedicated, high-priority software rule that specifically identifies the unique visual signature of school buses and their stop indicators [1]. This rule would be hardcoded to immediately trigger an emergency stop if a school bus signal is detected within a certain proximity, overriding standard navigation logic and preventing the vehicle from proceeding until the signal is explicitly confirmed as clear [1].
**

# December 15, 2025

Winter break will be a great break i hope because i need sleep....and we getting gifts so that will be fun.




# January 6, 2026
This break was quit fun it was chill we did some things and did news things.We also ate somethings it was my brothers birthday on the 22nd so we took him to olive garden and it was delicious.We also chilled and played outside,went to my cousins house.


# January 12, 2026

Autcraft was created by Stuart Duncan in 2013 as a direct response to the problem of widespread bullying and exclusion his autistic son and other neurodivergent children faced in unmoderated public online gaming spaces. It was designed as a safe, moderated, and welcoming private Minecraft server where autistic individuals and their families could play without fear of harassment or judgment. Protection from Harm: Unmoderated online spaces often expose vulnerable users to cyberbullying, hate speech, trolling, and other forms of harassment, which can have significant emotional and psychological impacts.Protection from Harm: Unmoderated online spaces often expose vulnerable users to cyberbullying, hate speech, trolling, and other forms of harassment, which can have significant emotional and psychological impacts.
