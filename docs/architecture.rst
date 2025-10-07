=======================================
Architecture Documentation
=======================================

This section contains comprehensive architectural documentation for the RD-Agent framework.

Overview
========

The architecture documentation is organized into three main documents:

1. **High-Level Architecture** - System overview and component interactions
2. **Low-Level Design** - Detailed implementation and class structures  
3. **Component Comparison** - Comparison with similar frameworks

Documents
=========

High-Level Architecture
-----------------------

.. toctree::
   :maxdepth: 2

An overview of the system architecture, including:

- System architecture diagram with all major components
- Key components and their responsibilities
- Data flow and execution model
- Supported scenarios
- Design principles
- Architecture benefits

`View High-Level Architecture <https://github.com/microsoft/RD-Agent/blob/main/docs/architecture/high_level_architecture.md>`_

Low-Level Design
----------------

Detailed component design and implementation details:

- Class structure and hierarchy diagrams
- Design patterns used (Strategy, Template Method, Observer)
- Core component details (Scenario, Experiment, Developer, etc.)
- Evolving framework components
- Workflow execution sequences
- Data structures
- Extension points
- Performance considerations

`View Low-Level Design <https://github.com/microsoft/RD-Agent/blob/main/docs/architecture/low_level_design.md>`_

Component Comparison
--------------------

Comparison with similar frameworks and systems:

- Framework comparison matrix
- Detailed component comparisons
- Unique advantages of RD-Agent
- Areas for improvement
- Use case mapping

`View Component Comparison <https://github.com/microsoft/RD-Agent/blob/main/docs/architecture/component_comparison.md>`_

Quick Start Guide
=================

If you're new to RD-Agent architecture:

1. Start with **High-Level Architecture** to understand the big picture
2. Review **Component Comparison** to see how RD-Agent compares to alternatives
3. Deep dive into **Low-Level Design** when you need implementation details

Architecture Diagrams
=====================

The documentation includes several types of diagrams:

- **System Architecture**: Overall component layout and interactions
- **Class Diagrams**: Detailed class structures using Mermaid
- **Sequence Diagrams**: Workflow and interaction flows
- **Comparison Diagrams**: Side-by-side comparisons with other frameworks

.. note::
   All diagrams are in Mermaid format and will render automatically in GitHub and most documentation viewers.

Key Architectural Concepts
===========================

Core Abstractions
-----------------

- **Scenario**: Domain-specific context and configuration
- **Hypothesis**: Proposed idea with reasoning
- **Experiment**: Structured implementation plan
- **Task**: Atomic unit of work
- **Workspace**: Code storage and execution environment
- **Feedback**: Evaluation results and learning signal
- **Trace**: Historical record for learning

Main Workflows
--------------

1. **R&D Loop**: Hypothesis → Experiment → Code → Execute → Feedback → Learn
2. **Evolving Strategy**: Error-driven code improvement (CoSTEER)
3. **Knowledge Flow**: RAG-based knowledge retrieval and update

Design Patterns
---------------

- **Strategy Pattern**: Pluggable components (HypothesisGen, Developer, Evaluator)
- **Template Method**: Abstract workflows with concrete implementations
- **Observer Pattern**: Trace recording and monitoring
- **Factory Pattern**: Scenario and component creation

Extending the Architecture
===========================

See the Extension Points section in the Low-Level Design documentation for details on:

- Adding new scenarios
- Implementing new evolution strategies
- Integrating new LLM backends
- Creating custom evaluators

Related Documentation
=====================

- :doc:`project_framework_introduction` - Original framework overview
- :doc:`development` - Setting up development environment
- :doc:`scens/catalog` - Specific scenario implementations
- :doc:`api_reference` - Detailed API documentation

Additional Resources
====================

For the most up-to-date architectural diagrams and detailed documentation:

- `Architecture Documentation on GitHub <https://github.com/microsoft/RD-Agent/tree/main/docs/architecture>`_

Contributing
============

When contributing to the architecture:

1. Update relevant diagrams when changing component structure
2. Add comparison entries when introducing features similar to other frameworks
3. Document new extension points
4. Keep diagrams in Mermaid format for consistency
5. Update documentation index when adding new content

Feedback
========

For questions or suggestions about the architecture:

- Open an issue on `GitHub <https://github.com/microsoft/RD-Agent/issues>`_
- Discuss in our `Discord channel <https://discord.gg/ybQ97B6Jjy>`_
- Contribute documentation improvements via pull request
