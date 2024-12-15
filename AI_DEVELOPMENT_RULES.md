## 1. Memlog System

**Project Initialization:**
- Always create or verify the existence of a `memlog` folder at the start of any project.
- The `memlog` folder must contain the following files:
  - `tasks.log`
  - `changelog.md`
  - `file_dependencies.md`
  - `stability_checklist.md`
  - `potential_issues.md`

**Usage and Maintenance:**
- Before providing any responses or taking actions, verify and update the files within the `memlog` folder.
- Use these logs to:
  - Track user progress.
  - Monitor system state.
  - Maintain persistent data between conversations.

**Task Management:**
- **Do Not** remove or alter existing task lists.
- Only append new tasks or update task states from `TODO` to `DONE`.
- **Never** rewrite the entire task list or changelog.
- Only add new entries to maintain a clear history of actions.

## 2. Task Breakdown and Execution

### Step-by-Step Breakdown:
- Deconstruct all user instructions into clear, numbered steps.
- Each step should include:
  - The specific action to be taken.
  - The reasoning behind the action.

### Proactive Issue Identification:
- Anticipate and flag potential issues before they occur.

### Sequential Verification:
- Verify the completion and correctness of each step before proceeding to the next.

### Error Handling:
- If errors are encountered:
  - Document the error in detail.
  - Return to the previous steps as necessary.
  - Retry the steps after addressing the issue.

## 3. Test-Driven Development (TDD)

### Pre-Implementation Phase
1. Review `functional_specifications.md`.
2. Analyze existing codebase.
3. Design test cases before implementation.

### Test Development Guidelines

#### Feature Testing Approach:
1. Write test cases first.
2. Implement unit tests.
3. Add integration tests.
4. Cover edge cases.
5. Test error scenarios.

#### Test Structure:
1. Mirror production code organization.
2. Follow AAA (Arrange, Act, Assert).
3. Ensure test independence.
4. Use descriptive test names.

#### Coverage Requirements:
1. Comprehensive business logic testing.
2. Success/failure path verification.
3. Boundary condition testing.
4. External dependency mocking.

## 4. Credential Management

**Clear Communication:**
- When requesting credentials, explain the purpose and necessity of each one.

**User Guidance:**
- Assist users in obtaining any missing credentials required for the project.

**Validation:**
- Always test the validity of credentials before utilizing them in the system.

**Security Practices:**
- **Never** store credentials in plaintext within the code or files.
- Use environment variables or secure credential storage methods.

**Credential Refresh Procedures:**
- Implement proper procedures to handle expiring credentials, including timely refreshes.

**User Education:**
- Provide guidance on best practices for secure credential storage and management.

## 5. Code Structure and Organization

### Modularity:
- Keep files small and modular.
- **No file must exceed 400 lines of code**.
- If a file becomes too large, refactor by breaking down classes or functions into smaller modules.

### Modularization Principles:

1. Group by Domain/Feature
   - Separate core business logic from infrastructure code.
   - Keep related functionality together.
2. Single Responsibility
   - Each module handles one specific concern.
   - Clear and focused purpose for each file.
3. Low Coupling
   - Minimize dependencies between modules.
   - Use interfaces/contracts for module communication.
4. High Cohesion
   - Keep strongly related code together.
   - Avoid mixing different levels of abstraction.
5. Clear Boundaries
   - Define explicit module interfaces.
   - Document module responsibilities and dependencies.

### Component Management:
- Split large components into smaller, manageable parts to enhance readability and maintainability.

### Separation of Concerns:
- Move constants, configurations, and lengthy strings to separate files or configuration modules.

### Naming Conventions:
- Use descriptive and meaningful names for files, functions, and variables to improve code clarity.

### Documentation:
- Document all file dependencies.
- Maintain a clean and organized project structure with clear directories and file hierarchies.

## 6. Error Handling and Reporting

**Detailed Reporting:**
- Implement comprehensive error reporting mechanisms that provide actionable information.

**Logging:**
- Log errors with relevant context and timestamps to aid in debugging and historical analysis.

**User Communication:**
- Provide users with clear, step-by-step instructions for error recovery.

**Error Tracking:**
- Maintain a history of errors to identify recurring patterns or systemic issues.

**Escalation Procedures:**
- Implement protocols to escalate unresolved issues to higher support levels or developers.

**Robust Mechanisms:**
- Ensure that all systems and components have strong error handling and recovery processes in place.

## 7. Documentation

**Code Documentation:**
- Write clear and concise comments for all public functions, methods, and complex code segments.

**README Files:**
- Include `README.md` files in each package or service directory, explaining the purpose, usage, and any special considerations.

**Architecture Documentation:**
- Maintain updated architectural diagrams (e.g., Mermaid diagrams) and descriptions in the main `README.md`.
- Maintain updated documentation and descriptions in main `.md` files of important services and areas.

**Configuration Documentation:**
- Document all configuration options, their defaults, and examples in the code and example configuration files.

**Functional Specifications Documentation:**
1. When code changes affect project structure or functionality:
   - Update `functional_specifications.md` to reflect:
     - New features or requirements.
     - Modified business rules.
     - Changed specifications.
     - Deprecated functionality.

## 8. Change Management

### When suggesting changes:
1. Start with test cases that validate requirements
2. Explain the rationale behind architectural decisions
3. Highlight potential impacts on existing code and tests
4. Consider maintainability and future extensibility
5. Provide migration steps if significant refactoring is needed
6. Include test updates or additions needed

### After implementing changes:
1. Review and update affected documentation
2. Confirm documentation accuracy
3. Verify all tests pass
4. Notify of any documentation updates made
5. Suggest additional test coverage if needed
