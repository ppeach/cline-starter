  # CLINE Starter

  Welcome to the CLINE Starter repository! This template is designed to help you kickstart your projects with minimal effort while fostering a collaborative and efficient development process with coding agents.

  ## Features

  - **AI_DEVELOPMENT_RULES.md**: Establishes rules and guidelines for the coding agent, ensuring consistency, quality, and adherence to your project goals.
  - **CUSTOM_INSTRUCTION.md**: Contains instructions to be copied and pasted into CLINE’s Custom Instruction settings, tailoring the model’s behavior for your specific project.
  - **PROJECT_SUMMARY.md**: Provides a structured summary of the project, serving as a blueprint for development.
  - **README.md**: This file, outlining the purpose and usage of the CLINE Starter repository.

  ## Setting Up a New Project

  1. **Copy Starter Files**: Clone or download this repository and copy the contents into your new Git repository.
  2. **Customize PROJECT_SUMMARY.md**: Fill out the `PROJECT_SUMMARY.md` file with your project details based on the provided example.
  3. **Configure Custom Instruction**: Copy the contents of `CUSTOM_INSTRUCTION.md` into CLINE’s Custom Instruction settings.
  4. **Initialize LLM Collaboration**: Start your development session with your Large Language Model (LLM).

     **First Prompt to LLM**:

```plaintext
You are a helpful AI coding assistant focused on documenting software projects. Your task is to help the user fill out their PROJECT_SUMMARY.md file. This file exists in their root folder and contains a basic template.

When assisting with the PROJECT_SUMMARY.md:

1. If you see an existing template, preserve its structure while helping fill it out
2. Ask relevant questions about any missing information needed for key sections
3. Help maintain clear, concise documentation that follows Markdown best practices

Please format code blocks, commands, and technical terms using appropriate Markdown syntax. Keep explanations clear and developer-friendly.

If the user needs to add new sections beyond the template, help them integrate those seamlessly while maintaining document flow and readability.

Before finalizing changes, verify that:
- All placeholder text is replaced with actual content
- Links are valid
- Headers follow a logical hierarchy
- Code blocks are properly formatted
- Installation steps are complete and clear

```

**Second Prompt to LLM**:

     ```plaintext
     Please review the `AI_DEVELOPMENT_RULES.md` and `CUSTOM_INSTRUCTION.md` to fully understand the guidelines and constraints of our collaboration. Once you're familiar with these rules, analyze the `PROJECT_SUMMARY.md` file and create a detailed, step-by-step plan to develop the project. Provide the reasoning behind each step and prepare the project infrastructure accordingly.
     ```

  ## Why Use CLINE Starter?

  CLINE Starter simplifies the initial setup, enabling you to focus on your ideas and collaborate effectively. By using a structured approach, you can maximize productivity and ensure high-quality outcomes.

  ## Contributing

  Contributions are welcome! Please fork the repository and submit a pull request with your improvements.

  ## License

  This project is licensed under the MIT License.
