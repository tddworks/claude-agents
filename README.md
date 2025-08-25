# Claude Code Specialized Agents

A collection of specialized AI agents for Claude Code that enhance software development workflows with focused expertise in specific domains.

## Overview

This repository contains intelligent agents designed to work with [Claude Code](https://claude.ai/code), Anthropic's CLI tool for AI-assisted software development. Each agent is a specialist that brings deep domain knowledge and best practices to help developers build better software faster.

## Available Agents

### 🏗️ TDD Chicago School Kotlin Agent
**File**: `tdd-chicago-school-kotlin.md`

A Test-Driven Development specialist following the Chicago School (classicist) approach for Kotlin development. This agent emphasizes:

- **Inside-Out Development**: Start with core domain objects and build outward
- **State-Based Verification**: Assert on object state rather than interactions  
- **Emergent Design**: Let design emerge naturally from tests
- **Minimal Mocking**: Use real objects whenever possible
- **Kotlin Idioms**: Leverage Kotlin's type system and language features

Perfect for developers who want to practice disciplined TDD with a focus on state verification and clean, testable code architecture.

### 🎨 ASCII UI Prototype Agent  
**File**: `ui-ascii-prototype.md`

A UI/UX design specialist focused on creating ASCII-based wireframes, mockups, and prototypes. This agent excels at:

- **ASCII Wireframing**: Create clear layout structures using text characters
- **Component Visualization**: Represent UI elements with consistent ASCII patterns
- **Responsive Design Concepts**: Show how layouts adapt across different screen sizes
- **Interactive Flow Mapping**: Visualize user journeys and state changes
- **Design Documentation**: Create maintainable, text-based design specs

Ideal for rapid prototyping, design documentation that lives alongside code, and communicating UI concepts in text-based environments.

## Why Specialized Agents?

Each agent represents years of accumulated best practices and domain expertise, distilled into actionable guidance. Instead of generic AI assistance, you get:

- **Domain-Specific Knowledge**: Deep understanding of specialized methodologies
- **Consistent Practices**: Agents follow established patterns and conventions
- **Accelerated Learning**: Learn best practices while building
- **Quality Assurance**: Built-in checks and guidance for common pitfalls

## How It Works

These agents integrate with Claude Code's agent system. Each `.md` file defines an agent with:

- **Specialized Knowledge**: Deep expertise in a specific domain
- **Automated Hooks**: Pre and post-execution scripts for environment setup
- **Consistent Patterns**: Established conventions and best practices
- **Quality Gates**: Built-in validation and verification steps

## Getting Started

### Prerequisites

- [Claude Code](https://claude.ai/code) - Anthropic's CLI tool for AI-assisted software development
- Basic familiarity with your chosen domain (TDD, UI/UX design, etc.)

### Installation & Setup

1. **Clone this repository**:
   ```bash
   git clone https://github.com/tddworks/claude-agents.git
   cd claude-agents
   ```

2. **Choose your agent**: Copy the agent file you want to use to your project directory or configure Claude Code to reference it.

3. **Integration**: Each agent file contains metadata that Claude Code uses to understand the agent's capabilities and configure the appropriate environment.

### Usage Examples

#### Using the TDD Chicago School Kotlin Agent

```bash
# In your Kotlin project directory
claude-code --agent tdd-chicago-school-kotlin.md "Help me implement a user registration feature using TDD"
```

The agent will:
- Set up the TDD environment with gradle clean
- Guide you through inside-out development
- Ensure state-based verification patterns
- Run tests and coverage verification
- Follow Kotlin idioms and best practices

#### Using the ASCII UI Prototype Agent

```bash
# In your project directory  
claude-code --agent ui-ascii-prototype.md "Create wireframes for a user dashboard"
```

The agent will:
- Create clear ASCII wireframes
- Show responsive design concepts
- Map interactive flows
- Document design decisions in text format
- Suggest improvements to layout and user experience

## Agent Structure

Each agent follows this structure:

```yaml
---
name: agent-name
type: category
color: "#hexcolor"
description: Brief description
capabilities:
  - capability1
  - capability2
priority: high|medium|low
hooks:
  pre: |
    # Setup commands
  post: |
    # Cleanup/verification commands
---

# Agent content with detailed instructions, examples, and best practices
```

## Contributing

We welcome contributions to expand the collection of specialized agents! Here's how you can help:

### Creating a New Agent

1. **Identify a Domain**: Choose a specific methodology, framework, or development practice that would benefit from specialized guidance.

2. **Research Best Practices**: Gather established patterns, conventions, and expert knowledge in that domain.

3. **Follow the Template**: Use the agent structure shown above and include:
   - Clear metadata with appropriate capabilities
   - Comprehensive methodology documentation
   - Practical examples and code samples
   - Common patterns and anti-patterns
   - Integration hooks for environment setup

4. **Test Your Agent**: Verify it works well with Claude Code and provides valuable, specialized guidance.

### Contribution Guidelines

- **Focus on Expertise**: Agents should represent deep, specialized knowledge rather than general advice
- **Include Examples**: Provide concrete code examples and usage patterns
- **Document Thoroughly**: Include both methodology and practical implementation guidance
- **Quality over Quantity**: Each agent should be comprehensive and well-tested
- **Follow Conventions**: Use consistent formatting and structure across agents

### Submission Process

1. Fork this repository
2. Create a new branch for your agent
3. Add your agent file with thorough documentation
4. Test the agent with Claude Code
5. Submit a pull request with a clear description

### Ideas for Future Agents

- **DDD (Domain-Driven Design) Specialist**: Bounded contexts, aggregates, domain events
- **Clean Architecture Guide**: Dependency inversion, use cases, adapters
- **Security Review Expert**: OWASP guidelines, vulnerability assessment
- **Performance Optimization**: Profiling, bottleneck analysis, optimization strategies
- **API Design Specialist**: REST, GraphQL, OpenAPI best practices
- **Database Design Expert**: Normalization, indexing, query optimization

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Anthropic](https://anthropic.com) for developing Claude Code
- The open source community for establishing the best practices these agents embody
- Contributors who help expand and improve the agent collection

---

**Start building better software with specialized AI guidance. Choose your agent and elevate your development workflow today!**