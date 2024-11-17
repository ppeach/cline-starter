  ### 1. Memlog System

**Project Initialization**:
* Always create or verify the existence of a `memlog` folder at the start of any project.
* The `memlog` folder must contain the following files:
* `tasks.log`
* `changelog.md`
* `file_dependencies.md`
* `stability_checklist.md`
* `potential_issues.md`

**Usage and Maintenance**:
* Before providing any responses or taking actions, verify and update the files within the `memlog` folder.
Use these logs to:
* Track user progress.
* Monitor system state.
* Maintain persistent data between conversations.
**Task Management**:
* **Do Not** remove or alter existing task lists.
* Only append new tasks or update task states from `TODO` to `DONE`.
* **Never** rewrite the entire task list or changelog.
* Only add new entries to maintain a clear history of actions.

### 2. Task Breakdown and Execution

**StepbyStep Breakdown**:

* Deconstruct all user instructions into clear, numbered steps.
Each step should include:
* The specific action to be taken.
* The reasoning behind the action.

**Proactive Issue Identification**:

* Anticipate and flag potential issues before they occur.

**Sequential Verification**:

* Verify the completion and correctness of each step before proceeding to the next.

**Error Handling**:

If errors are encountered:
* Document the error in detail.
* Return to the previous steps as necessary.
* Retry the steps after addressing the issue.

### 3. Credential Management

**Clear Communication**:
* When requesting credentials, explain the purpose and necessity of each one.

**User Guidance**:

 * Assist users in obtaining any missing credentials required for the project.


**Validation**:

* Always test the validity of credentials before utilizing them in the system.

**Security Practices**:

* **Never** store credentials in plaintext within the code or files.

* Use environment variables or secure credential storage methods.

**Credential Refresh Procedures**:

* Implement proper procedures to handle expiring credentials, including timely refreshes.

**User Education**:

* Provide guidance on best practices for secure credential storage and management.

### 4. Code Structure and Organization

**Modularity**:
* Keep files small and modular.

*   **No file must exceed 400 lines of code**.

* If a file becomes too large, refactor by breaking down classes or functions into smaller modules.

**Component Management**:

* Split large components into smaller, manageable parts to enhance readability and maintainability.

**Separation of Concerns**:

* Move constants, configurations, and lengthy strings to separate files or configuration modules.

**Naming Conventions**:

* Use descriptive and meaningful names for files, functions, and variables to improve code clarity.

**Documentation**:

* Document all file dependencies.
* Maintain a clean and organized project structure with clear directories and file hierarchies.

### 5. Error Handling and Reporting

**Detailed Reporting**:

  * Implement comprehensive error reporting mechanisms that provide actionable information.

**Logging**:

  * Log errors with relevant context and timestamps to aid in debugging and historical analysis.

**User Communication**:

  * Provide users with clear, stepbystep instructions for error recovery.

**Error Tracking**:

  * Maintain a history of errors to identify recurring patterns or systemic issues.

**Escalation Procedures**:

  * Implement protocols to escalate unresolved issues to higher support levels or developers.

**Robust Mechanisms**:

  * Ensure that all systems and components have strong error handling and recovery processes in place.

### 6. Documentation

**Code Documentation**:

  * Write clear and concise comments for all public functions, methods, and complex code segments.

**README Files**:

  * Include `README.md` files in each package or service directory, explaining the purpose, usage, and any special considerations.

**Architecture Documentation**:

  * Maintain updated architectural diagrams (e.g., Mermaid diagrams) and descriptions in the main `README.md`.
  * Maintain updated documentation and descriptions in main `.md` files of important services and areas.

**Configuration Documentation**:
  * Document all configuration options, their defaults, and examples in the code and example configuration files.
