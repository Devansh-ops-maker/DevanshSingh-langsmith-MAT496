# LangSmith Project
**Author:** Devansh Singh (2410110755)

---

## Module 1 (Course 1)
**Learnings from this Course:**  
- Implemented and explored the traceable detector.  
- Learned how traceable helps monitor and debug the steps taken by the application.  
- Observed how it generates logs for each step, making the workflow more transparent and easier to analyze.

**Changes Implemented:**  
- Added new prompts for improved responses.  
- Applied the traceable detector to all functions.  
- Added metadata for functions to enhance traceability and logging.

---

## Module 1 (Course 2)
**Learnings from this Course:**  
- Learned about the different types of runs in LangSmith: **LLM, tool, and retrieve**.  
  - **LLM run:** Executes a language model to generate responses.  
  - **Tool run:** Calls a predefined function or tool to perform a task.  
  - **Retrieve run:** Fetches relevant documents or data for answering questions.

**Changes Implemented:**  
- Added three functions that retrieve `.cpp` and `.txt` files to demonstrate the retrieve run (hardcoded for demo).  
- Added a tool checker function to return the name of the admin if asked.  
- Added prompts for the LLM run.

---

## Module 1 (Course 3)
**Learnings from this Course:**  
- Explored **RunTree**, **wrapOpenAI**, and **Trace Context Manager** as alternative methods for logging traces.  
- Learned how RunTree can track workflows in more advanced scenarios.  
- Understood how wrapOpenAI can integrate trace logging directly with OpenAI API calls.  
- Observed how Trace Context Manager allows contextual trace logging within workflows.

**Changes Implemented:**  
- Created a calculator workflow to demonstrate trace logging using Trace Context Manager.  
- Queried detailed information about Shiv Nadar University to showcase wrapOpenAI functionality.  
- Developed MathDemo examples to illustrate advanced RunTree capabilities.  
- Implemented examples to show alternatives to traceable, highlighting different logging strategies and their benefits.

---

## Module 1 (Course 4)
**Learnings from this Course:**  
- Learned that a sequence of traces is called a **track**, which allows keeping track of conversations.  
- All traces belonging to a conversation share the same key but are differentiated by their values.  
- Implemented a conversation between a BMS student and a CSE student to demonstrate the practical use of track in monitoring sequential interactions.

**Changes Implemented:**  
- Added a conversation workflow to log multiple question-answer interactions as a single track.  
- Demonstrated how each step (retrieval, LLM call, response generation) is traced under the same conversation key.  
- Showcased the trace sequence to monitor and debug the full conversation between the students.

---

## Module 2 (Course 1)
**Learnings from this Course:**  
- Learned that we can create our own datasets using the LangSmith SDK.  
- Explored how to structure inputs and outputs for question-answer datasets.  
- Observed how datasets can be used later to retrieve answers or build retrieval-augmented workflows.

**Changes Implemented:**  
- Implemented a question-answer dataset related to how to register for ICPC.  
- Used the LangSmith Client to create examples in the dataset.  
- Prepared multiple input questions and corresponding output answers to simulate real queries.

---

## Module 2 (Course 2)
**Learnings from this Course:**  
- Learned how to create evaluators to check similarities between outputs.  
- Explored how LLMs can be used to implement these evaluators.  
- Observed how evaluators can help automate the evaluation of responses or code logic.

**Changes Implemented:**  
- Implemented a code logic similarity evaluator to compare code snippets across different programming languages.  
- Created sample inputs and expected outputs to test the evaluator.  
- Evaluated the similarity between expected and given outputs using the evaluator.

---

## Module 2 (Course 3)
**Learnings from this Course:**  
- Learned how to run experiments on datasets using LLMs via the LangSmith SDK.  
- Explored the use of custom evaluators to assess the outputs of LLMs.  
- Observed how metadata can be passed to experiments to track model details or other information.

**Changes Implemented:**  
- Implemented a conciseness evaluator (`is_concise_enough`) to check if the LLM output is shorter than 1.5x the reference output length.  
- Created a target function (`target_function`) that generates responses for questions using our retrieval-augmented workflow (`langsmith_rag`).  
- Ran experiments on the dataset `"ds-dependable-pickup-7"` with the evaluator to automatically assess LLM outputs.  
- Added the ability to pass custom metadata (like `model_name`) to the experiments for better tracking and analysis.

---

## Module 3 (Course 1)
**Learnings from this Course:**  
- Learned how to create and manage multiple datasets in LangSmith for structured experimentation.  
- Created a dataset related to environment-based questions to perform evaluation and analysis experiments.  
- Understood how datasets can be leveraged to test model performance across different domains.

**Changes Implemented:**  
- Created an additional dataset related to CCC (Coding and Computing Concepts) questions to conduct experiments.  
- Used both datasets to compare model responses and analyze performance consistency across different subject areas.

---

## Module 3 (Course 2)
**Learnings from this Course:**  
- Learned how to create custom prompts on LangChain.  
- Learned how to pull prompts from LangChain repositories.  
- Learned how to hydrate prompts with variables.  
- Learned how to convert hydrated prompts to OpenAI-compatible format.  
- Learned how to pull down a specific commit/version of a prompt.  
- Learned how to upload prompts programmatically from code.  
- Learned how to push a prompt as a **RunnableSequence**, linking it to a model.

**Changes Implemented:**  
- Created our own prompt `chess-llm`.  
- Pulled it down from LangChain and got its OpenAI version.  
- Made changes to the prompt and pulled a specific commit.  
- Converted the updated prompt to OpenAI format.  
- Uploaded a coding assistant related prompt to LangChain.  
- Pushed the same prompt as a RunnableSequence connected to `gpt-4o-mini`.
---
## Module 3 (Course 3)

### Learnings from this Course
- Learned how to use **LangChain Playground** to test and refine prompts interactively.
- Understood that **commits made to prompts in LangSmith** automatically reflect in the code, eliminating the need for manual updates.
- Observed how this **version control for prompts** improves workflow efficiency and reduces errors during development.
---
### Changes Implemented
- Integrated our **custom coding assistant prompt** into the `coding_rag` workflow.
- Demonstrated the feature where **updated prompt commits automatically sync** with the application.
- Verified that the system dynamically adapts to new prompt versions without requiring code changes.
---
