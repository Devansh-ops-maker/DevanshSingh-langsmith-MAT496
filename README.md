# LangSmith  Project

**Author:** Devansh Singh (2410110755)

---


## Learnings from Module 1 (Course 1)
- Implemented and explored the **traceable detector**.  
- Learned how traceable helps monitor and debug the steps taken by the application.  
- Observed how it generates logs for each step, making the workflow more transparent and easier to analyze.

---

## Changes Implemented for Module 1(Course 1)
- Added **new prompts** for improved responses.  
- Applied the **traceable detector** to all functions.  
- Added **metadata for functions** to enhance traceability and logging.

---

## Learnings from Module 1 (Course 2)
We learned about the different types of runs in LangSmith: **LLM**, **tool**, and **retrieve**.  

- **LLM run:** Executes a language model to generate responses.  
- **Tool run:** Calls a predefined function or tool to perform a task.  
- **Retrieve run:** Fetches relevant documents or data for answering questions.  

**Changes done in Module 1 (Course 2):**  
- Added three functions that retrieve `.cpp` and `.txt` files to demonstrate the retrieve run (hardcoded for demo).  
- Added a tool checker function to return the name of the admin if asked.  
- Added prompts for the LLM run.
  
---
## Learnings from Module 1 (Course 3)
- Explored **RunTree**, **wrapOpenAI**, and **Trace Context Manager** as alternative methods for logging traces.  
- Learned how **RunTree** can track workflows in more advanced scenarios.  
- Understood how **wrapOpenAI** can integrate trace logging directly with OpenAI API calls.  
- Observed how **Trace Context Manager** allows contextual trace logging within workflows.

---

## Changes Implemented for Module 1 (Course 3)
- Created a **calculator workflow** to demonstrate trace logging using **Trace Context Manager**.  
- Queried detailed information about **Shiv Nadar University** to showcase **wrapOpenAI** functionality.  
- Developed **MathDemo** examples to illustrate **Advanced RunTree** capabilities.  
- Overall, implemented examples to show alternatives to **traceable**, highlighting different logging strategies and their benefits.

---

## Learnings from Module 1 (Course 4)
- Learned that a **sequence of traces is called a track**, which allows keeping track of conversations.  
- All traces belonging to a conversation share the **same key** but are differentiated by their **values**.  
- Implemented a **conversation between a BMS student and a CSE student** to demonstrate the practical use of track in monitoring sequential interactions.

---

## Changes Implemented for Module 1 (Course 4)
- Added a **conversation workflow** to log multiple question-answer interactions as a single track.  
- Demonstrated how each step (retrieval, LLM call, response generation) is traced under the same conversation key.  
- Showcased the **trace sequence** to monitor and debug the full conversation between the students.
