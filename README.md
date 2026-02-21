# Student-Support-Generative-AI-Chatbot
Student Support Generative AI Chatbot is a domain-focused system that assists university students with academic inquiries such as deadlines, grading, and policies. Built in Python and deployed on Google Colab, it integrates Gemini API, multi-turn memory, tool-based calculation routing, and interaction logging for evaluation and academic purposes.

## Project Purpose

This project is aimed at designing and deploying a **Student Support Generative AI Chatbot** to help university students with frequent academic requests, including deadlines, submissions, grading, office hours, and overall academic policies. The system provides an example of how Generative AI can be practically applied through prompt engineering, multi-turn conversation management, and agent-like behaviour via tool usage. To ensure relevance, reliability, and ethical responses, the chatbot is intentionally constrained to a specific academic support domain.

## System Architecture

The system architecture is lightweight and modular, making it appropriate for demonstration and evaluation purposes. The chatbot is accessed through a **command-line style interface** running within a Google Colab notebook. The backend is implemented in Python and is responsible for managing the system prompt, preserving multi-turn conversational context using a transcript-based memory, routing calculation-related queries to a calculator tool, and forwarding non-calculation queries to the Gemini Large Language Model API. Interaction data is recorded during runtime and stored in a structured format for later analysis and evaluation.

## Deployment Environment and Technologies

The system is deployed and executed within **Google Colab**, which provides a cloud-based environment and simplifies dependency management. The implementation relies on Python libraries such as `google-genai` for API access, `pandas` for data handling, and `matplotlib` for data visualisation. The Gemini API key is managed securely using **Colab Secrets** and is not hard-coded into the source code, ensuring secure configuration handling and adherence to API best practices.

## Running the Demo

To run the demo, users execute the notebook cells sequentially until the chatbot interface becomes available. Once loaded, users can interact with the chatbot by entering queries directly into the notebook. The system supports basic commands to reset the conversation memory, export interaction logs to a CSV file, and generate evaluation plots. This setup enables interactive testing of the chatbot while also producing evidence suitable for analysis and reporting.

## Known Limitations

Several limitations are acknowledged in the current implementation. The chatbot relies on **implicit few-shot prompting** through multi-turn conversation history rather than explicit few-shot examples embedded in the system prompt. The calculator tool requires explicit numerical expressions and does not fully interpret complex natural-language grade descriptions. Additionally, the system is subject to **Gemini API free-tier rate limits**, which may restrict the number of requests during testing. The interface is intended for demonstration purposes only and is not designed as a full production-ready web application.

## Summary

Overall, the project is well-structured and demonstrates the practical use of Generative AI for a student support chatbot. It integrates prompt engineering, agent-like tool usage, interaction logging, and evaluation within a simple and reproducible environment suitable for academic demonstration and assessment.
