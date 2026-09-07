 Virtual Instructor — AI-Powered Educational Assistant

An intelligent educational assistant that helps students and educators generate personalized learning content, interact with an AI tutor, track learning progress, and access multilingual support through a unified interface.

Overview

Virtual Instructor is an AI-powered educational assistant designed to act as a virtual teaching companion for students and educators. The application brings multiple learning utilities together in one platform, including syllabus generation, assignment and quiz creation, flashcard generation, translation, progress tracking, and conversational interaction with an AI instructor.

The project is built with LangChain, OpenRouter, and Gradio, with additional knowledge-base and memory components designed to support a modular, LMS-ready architecture.

Key Features

📚 Learning Content Generation

Syllabus Generator — Create structured and personalized study syllabi.

Assignment & Quiz Creator — Generate MCQs and theory-based questions.

Flashcard Generator — Produce concise flashcards for revision and active recall.

🤖 AI Instructor

Interactive chat with an AI-powered instructor.

Uses LangChain and OpenRouter-powered language models for intelligent responses.

Provides a centralized interface for personalized learning assistance.

🌍 Multilingual Support

Translation support for:

Urdu

Hindi

French

Spanish

Arabic

Chinese

📈 Progress Tracking

Track learning progress through the application.

Supports a more personalized learning experience based on user activity.

🧩 Modular & LMS-Ready

Modular project structure for easier maintenance and extension.

Designed with the potential to integrate into Learning Management Systems (LMS).

🖥️ User-Friendly Interface

Built with Gradio.

Organized through an intuitive tab-based interface.

Technology Stack

Component

Technology

Frontend / UI

Gradio

LLM Integration

LangChain + OpenRouter

Language Models

GPT-3.5-turbo / Mistral

Knowledge Base

AIML, Prolog, Neo4j

Memory

Semantic, Episodic, PAM, Social

Multilingual Support

LangChain multilingual modules

Programming Language

Python

Project Architecture

The project follows a modular architecture that separates the user interface, AI/LLM integration, educational content generation, multilingual functionality, progress tracking, and knowledge/memory components.

This structure makes the application easier to maintain and provides a foundation for future educational features and LMS integration.

Project Structure

Virtual-Instructor/
├── .env.example
├── requirements.txt
├── README.md
├── run.py
├── src/
│   ├── generating_syllabus.py
│   ├── flashcard_generator.py
│   ├── openrouter_llm.py
│   ├── teaching_agent.py
│   ├── multilingual_support.py
│   ├── progress_tracker.py
│   └── ...
├── data/
│   ├── conversation.aiml
│   └── ...
└── pretrained_model/
    ├── learningFileList.aiml
    └── aiml_pretrained_model.dump

Getting Started

Prerequisites

Make sure the following are installed:

Python 3.9+

Git

An OpenRouter API key

1. Clone the Repository

git clone https://github.com/your-username/virtual-instructor.git
cd virtual-instructor

2. Create a Virtual Environment

Windows:

python -m venv .venv
.venv\Scripts\activate

macOS / Linux:

python -m venv .venv
source .venv/bin/activate

3. Install Dependencies

pip install -r requirements.txt

4. Configure Environment Variables

Create a .env file in the project root and add your OpenRouter API key:

OPENROUTER_API_KEY=your_openrouter_api_key_here

Security: Never commit your .env file or expose your API key in a public repository. Use .env.example to document required environment variables.

5. Run the Application

python src/run.py

Once the application starts, open the local Gradio interface in your browser:

http://127.0.0.1:7860

How It Works

The user selects an educational task through the Gradio interface.

The application processes the request using its corresponding modular component.

LangChain and OpenRouter provide the AI/LLM capabilities where required.

Educational content is generated or retrieved according to the selected feature.

Results are presented through the Gradio interface for further use.

Use Cases

Virtual Instructor can support:

Personalized study planning

Course and syllabus preparation

Assignment generation

Quiz and examination preparation

Flashcard-based revision

Multilingual learning

AI-assisted tutoring

Student progress monitoring

Future LMS-based educational workflows

Future Enhancements

Potential future improvements include:

Integration with additional LLM providers

Advanced student performance analytics

Personalized recommendation systems

Expanded language support

LMS and classroom-platform integrations

User authentication and role-based access

Persistent student profiles and learning histories

Enhanced assessment and feedback capabilities

Security & Best Practices

Store API credentials in environment variables.

Add .env to .gitignore.

Do not hard-code private API keys in source files.

Use .env.example for sharing configuration requirements.

Review third-party dependencies regularly.

License

No license is currently specified for this project.

 

Author / Project

Virtual Instructor

An AI-powered educational platform designed to make learning content generation, tutoring, assessment, and progress tracking more accessible through a unified interface.

Virtual Instructor — Learn smarter. Teach better.
