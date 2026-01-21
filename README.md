# Claude Code Marketplace

A collection of plugins and skills for Claude Code.

## Plugins

This repository contains the following plugins:

| Plugin | Description |
|--------|-------------|
| **review-tool** | Code review skills for various tech stacks |
| **agent-call** | Skills to delegate tasks to other AI agents |
| **agent-session** | Session analysis and agent rule suggestions |
| **research** | Web search and documentation retrieval skills |

## Installation

Follow the instructions below to install the plugins in Claude Code.

```bash
# Register the marketplace
/plugin marketplace add dotneet/claude-code-marketplace

# Install individual plugins
/plugin install review-tool@dotneet-marketplace
/plugin install agent-call@dotneet-marketplace
/plugin install agent-session@dotneet-marketplace
/plugin install research@dotneet-marketplace
```

## Skills

### review-tool

#### typescript-react-reviewer

Expert code reviewer for TypeScript + React 19 applications.

**Use when:**
- Reviewing React code and PR reviews
- Identifying anti-patterns and code smells
- Evaluating state management patterns
- TypeScript type safety checks

**Key features:**
- React 19 new hooks patterns (useActionState, useOptimistic, use)
- useEffect abuse detection
- State mutation detection

#### code-modularization-evaluator

Evaluate and improve code modularization using the Balanced Coupling Model.

**Use when:**
- Reviewing code architecture
- Refactoring modules
- Designing new systems

**Key features:**
- Coupling strength analysis (Intrusive/Functional/Model/Contract)
- Connascence type identification
- Actionable refactoring recommendations

### agent-call

#### call-claude

Delegate tasks to Claude Code CLI.

#### call-codex

Delegate tasks to Codex CLI.

#### call-cursor-agent

Delegate tasks to Cursor Agent.

### agent-session

#### suggest-agent-rules

Analyze session history and repository to suggest agent rules. Useful for onboarding or when review feedback increases.

### research

#### perplexity-search

Perform web searches, research, and reasoning using the Perplexity API. Requires `PERPLEXITY_API_KEY` environment variable.

**Capabilities:**
- Real-time web information retrieval
- Deep research analysis
- Advanced reasoning tasks

#### context7

Retrieve the latest library documentation using Context7. Prevents hallucinations from outdated training data.

**Use when:**
- Checking how to use a library's API
- Needing version-specific documentation
- Requesting code examples

## Usage

Once installed, these skills are automatically available in Claude Code. They will be suggested when relevant tasks are detected, or you can invoke them directly.

