# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
  The game was a simple page with a side bar for difficulty allowing the user to choose from 3 diffiulties, Easy, MEdium, and Hard. The main game section shows Developer debug information which shows the number to guess, attemps, score, and history. The game also allows you to submit a guess and 
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
    1. range for hard and medium are backwards, Medium should be from range 1-50 and hard should be from range 1-100.
    2. when you guess higher than expected it tells you to guess lower, when you guess lower it tells you to guess higher, Backwards.
    3. The new game button seems to be functional in that it cchanges the developer debug information, but,it does not print and ovverrite the mesage from the previous game and the message just stays there

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
  I used ClaudeCode for this project. 
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  One example of an AI suggeston that was correct is when I gave a query on the hard and medium difficulties being backwards, it pinpointed where that error was in the code and suggested a fix that was correct.
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
  In this project I did not have a instance where the AI suggestions was incorrect or misleading, atleast not to my knowledge. 

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
  I decided that by manually testing the application.
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
  I ran manual tests on all 3 errors and for example the swapped hints error I tested it after it fixed the code and it gave the correct hint.
- Did AI help you design or understand any tests? How?
  Yes it helped me design all the tests that verified that a guess of 60 against a secret of 50 returns true

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
  reruns in streamlit refers to any interaction will lead to a refresh, so a button click, a submission, any interaciotn will refresh the while app.
  Because of this fact, if you want data to persist after each rerun, you must use session state to allow for data persistence, much like UseState in React.js.
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
  One habit would be prompting strategy and breaking down bugs and solving them one at a time and one commit at a time instead of solving them in bulk.
- What is one thing you would do differently next time you work with AI on a coding task?
  I would try to incorporate agents more as they are more and experiment with them more.
- In one or two sentences, describe how this project changed the way you think about AI generated code.
  The project reinforced the importance of using AI as a companion in coding projects and the huge shift in coding practice due to AI generated code.