# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the secret number kept changing" or "the hints were backwards").
  1. the hints were wrong (in the opposite direction)
  2. can not create or start a new game 
  3. discrepency for attempts allowed 8 vs. 7
---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
  Copilot
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  "After i give context about the wrong hints (in the opposite direction), it correctly suggested to reverse LOWER & HIGHER in #file:app.py, and can give correct hints. "
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
  "Bug: unable to create or restart a new game.
  When prompted to debug this and suggest correction, AI seems to find the cause but the corrections does not full solve the issue. It even brought a new bug: streamlit.errors.StreamlitAPIException: st.session_state.guess_input_Normal cannot be modified after the widget with key guess_input_Normal is instantiated."

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
  1. I played several games, compared my guess with secret to check if the hints are in the right direction.
  2. I manually clicked the new game button to make sure it can create/restart a new game.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
- What change did you make that finally gave the game a stable secret number?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
