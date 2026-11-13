**3.1 Concepts**

Educational Gamification combined with a Web-Based Execution Decision Support System (DSS) is a learning module or paradigm that combines gamified behavioural mechanics, for example sequential learning, real-time feedback loops, scoring marks and diagnostic hints directly into web-based execution platform. Rather than depending on passive reading materials, this technology evaluates player’s knowledge by the dashboard.

The core technology functions on a continuous Input-Evaluate-Feedback-Reward (IEFR) lifecycle:
i.	Input: Player inspect the wrong code given or visual threat scenarios.

ii.	Evaluate: Client-side deterministic engine parses the player’s answer against expected pattern tokens.

iii.	Feedback: The system instantly triggers visual indicators (color-coded highlighting, line error markers or diagnostic hint prompts)

iv.	Reward & Progression: Validated answer will be an increment for player’s scores to unlock the next level in the game.

```mermaid
flowchart TD
    Start([Start]) --> Login{Log in?}
    Login -- Yes --> EnterUser[/Enter username, password/]
    Login -- No --> SignUp[Sign up]
    SignUp --> EnterDetails[/Enter details/]
    EnterUser --> Dashboard[Game Dashboard]
    EnterDetails --> Dashboard

    Dashboard --> Room1{Room 1?}
    Room1 -- Yes --> Game1[Fill-in-the-blank coding game]
    Room1 -- No --> Room2{Room 2?}

    Room2 -- Yes --> Game2[Debugging game]
    Room2 -- No --> Room3{Room 3?}

    Room3 -- Yes --> Game3[Cyber-threat scenarios game]
    Room3 -- No --> Dashboard

    Game1 --> Input[/User input the answer and click validate/]
    Game2 --> Input
    Game3 --> Input

    Input --> Correct{Is the answer correct?}
    Correct -- Yes --> Green[Green successful indicator pop out]
    Correct -- No --> Red[Red indicator failed pop out]
    Red --> Hint[Hint pop out]
    Hint --> Input

    Green --> Continue{Continue playing?}
    Continue -- Yes --> NextLevel[Next level]
    NextLevel --> Dashboard
    Continue -- No --> Logout[Log out]
    Logout --> End([End])
```


