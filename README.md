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

---

## Learnings from Module 2 (Course 1)
- Learned that we can **create our own datasets** using the LangSmith SDK.  
- Explored how to structure **inputs and outputs** for question-answer datasets.  
- Observed how datasets can be used later to retrieve answers or build retrieval-augmented workflows.

---

## Changes Implemented for Module 2 (Course 1)
- Implemented a **question-answer dataset** related to **how to register for ICPC**.  
- Used the LangSmith `Client` to **create examples** in the dataset.  
- Prepared multiple input questions and corresponding output answers to simulate real queries.

---

## Learnings from Module 2 (Course 2)
- Learned how to **create evaluators** to check similarities between outputs.  
- Explored how **LLMs can be used** to implement these evaluators.  
- Observed how evaluators can help automate the evaluation of responses or code logic.

---

## Changes Implemented for Module 2 (Course 2)
- Implemented a **code logic similarity evaluator** to compare code snippets across different programming languages.  
- Created **sample inputs and expected outputs** to test the evaluator.  
- Evaluated the **similarity between expected and given outputs** using the evaluator.

---

## Learnings from Module 2 (Course 3)
- Learned how to **run experiments on datasets** using LLMs via the LangSmith SDK.  
- Explored the use of **custom evaluators** to assess the outputs of LLMs.  
- Observed how **metadata can be passed** to experiments to track model details or other information.  

---

## Changes Implemented for Module 2 (Course 3)
- Implemented a **conciseness evaluator** (`is_concise_enough`) to check if the LLM output is shorter than 1.5x the reference output length.  
- Created a **target function** (`target_function`) that generates responses for questions using our retrieval-augmented workflow (`langsmith_rag`).  
- Ran **experiments on the dataset** `"ICPC Dataset"` with the evaluator to automatically assess LLM outputs.  
- Added the ability to **pass custom metadata** (like `model_name`) to the experiments for better tracking and analysis.

---
