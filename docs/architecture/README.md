# RD-Agent Architecture Documentation

This directory contains comprehensive architectural documentation for the RD-Agent framework.

## Documents

### 1. [High-Level Architecture](high_level_architecture.md)
An overview of the system architecture, including:
- System architecture diagram with all major components
- Key components and their responsibilities
- Data flow and execution model
- Supported scenarios
- Design principles
- Architecture benefits

**Best for:** Understanding the overall system design and component interactions.

### 2. [Low-Level Design](low_level_design.md)
Detailed component design and implementation details:
- Class structure and hierarchy diagrams
- Design patterns used (Strategy, Template Method, Observer)
- Core component details (Scenario, Experiment, Developer, etc.)
- Evolving framework components
- Workflow execution sequences
- Data structures
- Extension points
- Performance considerations

**Best for:** Developers wanting to understand implementation details or extend the framework.

### 3. [Component Comparison](component_comparison.md)
Comparison with similar frameworks and systems:
- Framework comparison matrix
- Detailed component comparisons
  - Hypothesis generation
  - Code generation (CoSTEER vs others)
  - Experiment execution
  - Feedback loops
  - Knowledge management
  - Multi-agent coordination
- Unique advantages of RD-Agent
- Areas for improvement
- Use case mapping

**Best for:** Understanding RD-Agent's positioning in the AI agent ecosystem and choosing the right tool.

## Quick Start

If you're new to RD-Agent architecture:

1. **Start with** [High-Level Architecture](high_level_architecture.md) to understand the big picture
2. **Then review** [Component Comparison](component_comparison.md) to see how RD-Agent compares to alternatives
3. **Deep dive into** [Low-Level Design](low_level_design.md) when you need implementation details

## Architecture Diagrams

The documentation includes several types of diagrams:

- **System Architecture**: Overall component layout and interactions
- **Class Diagrams**: Detailed class structures using Mermaid
- **Sequence Diagrams**: Workflow and interaction flows
- **Comparison Diagrams**: Side-by-side comparisons with other frameworks

All diagrams are in Mermaid format and will render automatically in GitHub and most documentation viewers.

## Key Architectural Concepts

### Core Abstractions
- **Scenario**: Domain-specific context and configuration
- **Hypothesis**: Proposed idea with reasoning
- **Experiment**: Structured implementation plan
- **Task**: Atomic unit of work
- **Workspace**: Code storage and execution environment
- **Feedback**: Evaluation results and learning signal
- **Trace**: Historical record for learning

### Main Workflows
1. **R&D Loop**: Hypothesis → Experiment → Code → Execute → Feedback → Learn
2. **Evolving Strategy**: Error-driven code improvement (CoSTEER)
3. **Knowledge Flow**: RAG-based knowledge retrieval and update

### Design Patterns
- **Strategy Pattern**: Pluggable components (HypothesisGen, Developer, Evaluator)
- **Template Method**: Abstract workflows with concrete implementations
- **Observer Pattern**: Trace recording and monitoring
- **Factory Pattern**: Scenario and component creation

## Extending the Architecture

See [Low-Level Design - Extension Points](low_level_design.md#extension-points) for details on:
- Adding new scenarios
- Implementing new evolution strategies
- Integrating new LLM backends
- Creating custom evaluators

## Related Documentation

- [Project Framework Introduction](../project_framework_introduction.rst) - Original framework overview
- [Development Guide](../development.rst) - Setting up development environment
- [Scenario Documentation](../scens/catalog.rst) - Specific scenario implementations
- [API Reference](../api_reference.rst) - Detailed API documentation

## Contributing

When contributing to the architecture:
1. Update relevant diagrams when changing component structure
2. Add comparison entries when introducing features similar to other frameworks
3. Document new extension points
4. Keep diagrams in Mermaid format for consistency
5. Update this index when adding new documentation

## Feedback

For questions or suggestions about the architecture:
- Open an issue on GitHub
- Discuss in Discord channel
- Contribute documentation improvements via pull request
