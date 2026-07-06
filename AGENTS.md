# AGENTS.md - AI Product Factory Operating System

This document defines the comprehensive operating rules and guidelines for all AI agents working within the AI Product Factory repository. It serves as the central "operating system" designed to ensure consistency, efficiency, and adherence to best practices across all AI development workflows.

## 1. Repository Purpose

The AI Product Factory repository serves as a centralized hub for developing, managing, and deploying AI-powered products. Its structure and rules are designed to facilitate a systematic, scalable, and collaborative approach to AI development, from ideation and prompt engineering to microagent implementation and deployment.

## 2. Core Principles

*   **Pragmatism over Perfection**: Strive for effective solutions that meet requirements, rather than getting stuck on achieving unattainable perfection.
*   **Clarity and Simplicity**: Favor clear, concise, and easily understandable code, documentation, and communication.
*   **Consistency**: Adhere to established standards and workflows to ensure uniformity across the project.
*   **Collaboration**: Foster an environment where AI agents can work effectively together and with human overseers.
*   **Continuous Improvement**: Regularly review and update processes, documentation, and code based on learnings and feedback.

## 3. General Workflow

The standard workflow for AI agents within this repository is as follows:

*   **Understand Requirements**: Thoroughly grasp the task or feature request, including its goals and constraints.
*   **Read Playbooks**: Consult relevant playbooks in the `playbooks/` directory to understand established procedures and best practices for the task at hand.
*   **Plan**: Outline the steps required to complete the task, identify potential challenges, and formulate a strategy. This may involve documenting decisions in a temporary file or using `think` tool.
*   **Implement**: Write code, create configurations, or generate documentation according to the plan and relevant standards.
*   **Validate**: Test the implementation to ensure it meets requirements, functions correctly, and adheres to coding standards. This includes running tests, performing manual checks, and reviewing outputs.
*   **Commit**: Create small, focused commits with clear and descriptive messages summarizing the changes.
*   **Push**: Push committed changes to the designated remote branch according to the Git Rules.

## 4. Git Rules

These rules govern all Git operations performed by AI agents:

*   **Never modify git global configuration.**
*   **Never initialize git.** Operate within the pre-existing repository.
*   **Never create a branch unless requested.** All work should be performed on the currently checked-out branch.
*   **Never create a Pull Request unless requested.**
*   **Always work on the current checked out branch.**
*   **Pull latest changes before starting work.** Ensure the local repository is up-to-date with `origin/main` (or the designated primary branch) before commencing any task.
*   **Make small focused commits.** Each commit should represent a single, logical change.

## 5. Documentation Rules

*   **Purposeful**: Documentation should serve a clear purpose, aiding understanding and usability.
*   **Concise and Practical**: Provide essential information without unnecessary jargon or verbosity. Focus on *what* and *why*, supplemented by necessary *how*.
*   **Accurate and Up-to-Date**: Reflect the current state of the codebase and project.
*   **Accessible**: Use clear language and a logical structure. Adhere to standards defined in `docs/`.
*   **Complete**: Ensure all relevant aspects of a feature, component, or process are documented.

## 6. Coding Standards

*   **Readability**: Code must be clean, well-formatted, and easy to understand. Follow linters and formatters.
*   **Maintainability**: Write code that is easy to modify, debug, and extend. Avoid unnecessary complexity.
*   **Efficiency**: Implement solutions that are performant and resource-conscious, without sacrificing readability.
*   **Modularity**: Design code in modular components with clear responsibilities and interfaces.
*   **Adherence to Standards**: Strictly follow the coding standards and guidelines documented in `docs/09-coding-standard.md`.

## 7. Decision Making

*   **Requirement Clarification**: If requirements are ambiguous, unclear, or incomplete, always ask for clarification *before* proceeding with implementation.
*   **Architectural Decisions**: Document and explain significant architectural decisions and their rationale before implementation, typically in a dedicated design document or via the `think` tool.
*   **Prioritization**: Focus on tasks that align with the overall project goals and priorities. If faced with conflicting priorities, seek guidance.

## 8. Communication Style

*   **Professional and Respectful**: Maintain a professional and respectful tone in all communications.
*   **Clear and Concise**: Articulate thoughts, plans, and results clearly and directly. Avoid ambiguity.
*   **Action-Oriented**: When reporting status or results, focus on actions taken, outcomes, and next steps.
*   **Transparency**: Be transparent about progress, challenges, and decisions made. Use tools like `think` and detailed commit messages to log reasoning.

## 9. Repository Structure

The repository is organized to facilitate a systematic and scalable approach to AI development:

*   **`docs/`**: Contains project documentation, including standards, workflows, and guidelines.
    *   **`docs/assets/`**: Stores assets (images, diagrams) used in documentation.
*   **`playbooks/`**: Stores detailed procedural guides and strategies for AI development tasks.
    *   **`playbooks/core/`**: Foundational playbooks.
    *   **`playbooks/project-types/`**: Playbooks specific to different AI project categories.
*   **`prompts/`**: Houses curated prompts for LLMs and AI models.
    *   **`prompts/system/`**: System-level prompts guiding agent behavior.
    *   **`prompts/tasks/`**: Prompts for specific task execution.
    *   **`prompts/review/`**: Prompts for code review and feedback generation.
*   **`templates/`**: Provides reusable templates for code, configurations, and documents.
    *   **`templates/prd/`**: Product Requirements Document templates.
    *   **`templates/architecture/`**: Architecture design templates.
    *   **`templates/database/`**: Database schema and design templates.
    *   **`templates/api/`**: API definition and documentation templates.
    *   **`templates/frontend/`**: Frontend code and component templates.
    *   **`templates/backend/`**: Backend service and module templates.
    *   **`templates/fullstack/`**: Full-stack project templates.
*   **`microagents/`**: Contains the source code for individual AI agents.
*   **`scripts/`**: Utility scripts for automation, development, and deployment.
*   **`examples/`**: Demonstrates practical applications and usage patterns.
    *   **`examples/sample-project/`**: A sample project showcasing factory capabilities.

## 10. Definition of Done

A task, feature, or change is considered "Done" when all the following criteria are met:

*   **Requirements Met**: All specified requirements and user stories are fully implemented.
*   **Code Complete**: The implementation is complete, adheres to coding standards, and is well-documented.
*   **Validated**: The changes have passed all relevant tests (unit, integration, etc.) and manual validation checks.
*   **Reviewed (if applicable)**: Code has been reviewed according to the established review process.
*   **Committed**: Changes are committed with a clear, descriptive message.
*   **Pushed**: Changes are successfully pushed to the target branch.
*   **Documentation Updated**: Any necessary documentation (code comments, READMEs, AGENTS.MD, etc.) has been created or updated.
*   **No Known Issues**: There are no outstanding bugs, performance regressions, or critical issues related to the changes.
*   **Follows Playbooks**: The implementation process adhered to relevant playbooks.
