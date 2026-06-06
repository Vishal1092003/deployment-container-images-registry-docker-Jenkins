# How GitHub Webhooks Are Used

GitHub webhooks are commonly used to **automate actions whenever something happens in a repository**.

## Example 1: CI/CD Pipeline (Most Common)

When a developer pushes code:

```mermaid
flowchart TD
    A[👨‍💻 Developer Pushes Code]
    B[📂 GitHub Repository]
    C[🔔 GitHub Webhook]
    D[⚙️ Jenkins]
    E[🧪 Build & Test Code]
    F[🚀 Deploy Application]

    A --> B
    B -->|Push Event| C
    C -->|HTTP POST Request| D
    D --> E
    E -->|Success| F

    classDef dev fill:#3498db,stroke:#21618c,color:#fff,stroke-width:2px;
    classDef github fill:#24292e,stroke:#000,color:#fff,stroke-width:2px;
    classDef webhook fill:#f39c12,stroke:#a65d00,color:#fff,stroke-width:2px;
    classDef jenkins fill:#27ae60,stroke:#145a32,color:#fff,stroke-width:2px;
    classDef process fill:#8e44ad,stroke:#512e5f,color:#fff,stroke-width:2px;

    class A dev;
    class B github;
    class C webhook;
    class D jenkins;
    class E,F process;
```

## Flow

1. Developer pushes code to GitHub.
2. GitHub detects the **push** event.
3. GitHub sends a webhook request to Jenkins.
4. Jenkins automatically:
   - Pulls the latest code.
   - Builds the application.
   - Runs tests.
   - Deploys the application if everything succeeds.

## Benefits

- Automatic build and deployment.
- Faster feedback for developers.
- Reduced manual effort.
- Consistent CI/CD workflow.

## Summary

GitHub Webhooks enable event-driven automation:

```mermaid
flowchart LR
    A[Code Push] --> B[GitHub]
    B --> C[Webhook]
    C --> D[Jenkins]
    D --> E[Build & Test]
    E --> F[Deploy]
```
