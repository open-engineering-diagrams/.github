Open Engineering Diagrams

Diagrams for understanding, explaining, investigating, and engineering systems.

Open Engineering Diagrams is the visual language and diagramming capability of the Open Engineering ecosystem.

We create open, reusable, machine-readable diagrams that help engineers move between elements, relationships, systems, architecture, behaviour, evidence, and decisions.

If engineering is about understanding how things fit together, diagrams are one of the most powerful ways to make that understanding visible.

⸻

What is Open Engineering Diagrams?

Open Engineering Diagrams provides the conventions, models, components, generators, and tooling needed to create engineering diagrams as first-class Open Engineering Elements.

A diagram is not merely an image.

It can be:

* generated from structured engineering data
* connected to Open Engineering Elements
* linked to Systems of Record
* validated against conventions
* version controlled
* rendered into multiple visual formats
* used as evidence in an investigation
* embedded into documentation
* used as an input to AI assistants
* continuously regenerated as systems change

This makes diagrams part of the engineering system rather than an artefact produced at the end of a project.

⸻

The Open Engineering Diagram

An Open Engineering Diagram describes:

                    ┌─────────────────────┐
                    │       Diagram       │
                    │                     │
                    │   Elements          │
                    │   Relationships     │
                    │   Semantics         │
                    │   Layout            │
                    │   Evidence          │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
        Open Engineering   Systems of Record   Evidence
           Elements

The important distinction is between what a diagram means and how it is rendered.

The same engineering model should be capable of producing:

* architecture diagrams
* system context diagrams
* dependency graphs
* deployment diagrams
* sequence diagrams
* state diagrams
* topology diagrams
* journey maps
* investigation maps
* relationship graphs
* product maps
* capability maps
* engineering landscapes

⸻

Principles

1. Diagrams are data

A diagram should be representable as structured information.

diagram:
  id: oee.diagram.example
  type: architecture
  elements:
    - service-a
    - service-b
    - database
  relationships:
    - from: service-a
      to: service-b
    - from: service-b
      to: database

The visual representation is a rendering of that model.

⸻

2. Semantics before layout

The meaning of a diagram should not depend on where an object happens to be drawn.

We therefore separate:

Semantic model

from

Visual representation

This allows the same model to be rendered differently for different audiences and purposes.

⸻

3. Open Engineering Elements are the building blocks

Diagrams can reference any Open Engineering Element.

Element
   │
   ├── Component
   ├── Service
   ├── Product
   ├── Repository
   ├── Person
   ├── Capability
   ├── System
   ├── Environment
   ├── Event
   ├── Investigation
   └── Evidence

A diagram becomes a view over the engineering universe.

⸻

4. Diagrams should be reproducible

Where possible, diagrams should be generated from source data rather than manually maintained pixels.

Source
  │
  ▼
Engineering Model
  │
  ▼
Diagram Definition
  │
  ├──────────────┐
  ▼              ▼
SVG            PNG
  │              │
  └──────┬───────┘
         ▼
      Documentation

This makes diagrams suitable for version control and continuous engineering workflows.

⸻

5. Diagrams should be composable

Small diagrams should be capable of being combined into larger engineering views.

Element Diagram
       │
       ▼
System Diagram
       │
       ▼
Architecture Diagram
       │
       ▼
Engineering Landscape

This enables progressive exploration rather than forcing every diagram to contain everything.

⸻

Diagram Dimensions

Open Engineering Diagrams can describe several complementary dimensions of a system.

Structure

What exists?

Components, services, products, repositories, infrastructure and other elements.

Relationships

How are things connected?

Dependencies, ownership, communication, composition and association.

Behaviour

What happens?

Events, workflows, sequences, state transitions and interactions.

Topology

Where are things?

Networks, infrastructure, environments, locations and deployment relationships.

Time

How does the system change?

Versions, evolution, migrations, timelines and journeys.

Evidence

Why do we believe this?

Observations, measurements, investigation results and supporting evidence.

⸻

Diagram Types

The organisation can provide reusable definitions and tooling for diagram families such as:

Family	Purpose
Architecture	Understand system structure
Context	Understand system boundaries
Component	Explore internal composition
Dependency	Understand dependencies
Deployment	Understand runtime placement
Network	Understand connectivity
Sequence	Understand interactions over time
State	Understand behavioural transitions
Workflow	Understand processes
Journey	Understand experiences and paths
Product	Understand product structure
Capability	Understand organisational capabilities
Investigation	Explore hypotheses and evidence
Landscape	Understand large engineering environments

The catalogue should grow organically as new reusable diagram patterns emerge.

⸻

Diagram Pipeline

Open Engineering Diagrams fits into the wider Open Engineering architecture:

                Systems of Record
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
       GitHub       Backstage     Kubernetes
          │            │            │
          └────────────┼────────────┘
                       ▼
              Open Engineering
                   Elements
                       │
                       ▼
              Diagram Definition
                       │
                       ▼
             Open Engineering
                  Diagrams
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
         SVG          PNG          Interactive
          │            │            │
          └────────────┼────────────┘
                       ▼
              Humans + AI

This makes diagrams a natural projection of the Open Engineering model.

⸻

Diagrams + AI

Diagrams are particularly valuable to AI assistants because they provide a structured visual representation of complex relationships.

An AI assistant can:

* generate diagrams
* explain diagrams
* detect inconsistencies
* compare diagrams
* identify missing relationships
* navigate from a diagram to underlying elements
* use diagrams as investigation context
* update diagrams after engineering changes
* create diagrams from natural-language descriptions

This creates a useful feedback loop:

Observe
   ↓
Understand
   ↓
Model
   ↓
Diagram
   ↓
Investigate
   ↓
Discover
   ↓
Update Model
   ↓
Regenerate Diagram

⸻

Open Engineering Map

Open Engineering Diagrams is closely related to Open Engineering Map.

Where Open Engineering Map provides the ability to discover and navigate engineering elements, diagrams provide focused visual projections of those elements.

Open Engineering Ecosystem
            │
            ▼
    Open Engineering Map
            │
            ▼
     Element relationships
            │
            ▼
   Open Engineering Diagram
            │
            ▼
     Human understanding

A map shows the landscape.

A diagram explains a particular view of that landscape.

⸻

Evidence-aware diagrams

Engineering diagrams can also become part of an investigation.

For example:

Observation
    │
    ▼
Investigation
    │
    ├── Hypothesis
    │
    ├── Evidence
    │
    └── Findings
            │
            ▼
         Diagram

This allows a diagram to communicate not only what the system looks like, but also why we believe it looks that way.

This is particularly useful for the Code Smell Detective, Architecture Detective, Dependency Detective, and other Detective OS specialisations.

⸻

Repositories

The organisation can host reusable building blocks such as:

* diagram conventions
* diagram schemas
* diagram definitions
* diagram components
* diagram generators
* diagram renderers
* diagram examples
* diagram datasets
* diagram validation tools
* diagram integrations

Repositories should favour reusable capabilities over isolated finished images.

⸻

Open by Design

Open Engineering Diagrams is intended to be:

* Open — open source and open standards where possible
* Composable — built from reusable elements
* Machine-readable — diagrams have structured representations
* Versionable — diagram definitions belong in source control
* Reproducible — the same source should produce the same result
* Interoperable — compatible with existing engineering tools
* Evidence-aware — relationships can have provenance
* AI-ready — diagrams can be generated and consumed by AI systems

⸻

Part of Open Engineering

Open Engineering Diagrams is one part of the wider Open Engineering ecosystem.

                 Open Engineering
                        │
       ┌────────────────┼────────────────┐
       │                │                │
   Elements          Systems          Evidence
       │                │                │
       └────────────────┼────────────────┘
                        │
                        ▼
                Open Engineering
                     Diagrams
                        │
             ┌──────────┼──────────┐
             ▼          ▼          ▼
          Maps       Stories    Motion
                                  Pictures

Together these capabilities allow engineering knowledge to move between data, models, diagrams, stories, investigations, and experiences.

⸻

Contributing

We welcome contributions that improve the ability to represent engineering knowledge visually.

Useful contributions include:

* new diagram conventions
* new diagram schemas
* reusable diagram components
* renderers
* generators
* validation rules
* integrations
* examples
* documentation
* experiments with AI-generated diagrams

If you have an engineering representation that could become a reusable diagram pattern, we’d love to explore it.

⸻

Vision

Our goal is simple:

Make engineering systems easier to see, understand, investigate, and explain.

Open Engineering Diagrams turns engineering relationships into reusable visual knowledge.

Model it.
Diagram it.
Understand it.
Engineer it.

⸻

Open Engineering Diagrams
The visual language of Open Engineering.
