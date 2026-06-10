---
layout: home

hero:
  name: "Syne"
  text: "The Context Compiler."
  tagline: "Distill legacy Java monoliths into precise execution flows. Cut token costs, eliminate context bloat, and keep enterprise code secure."
  actions:
    - theme: brand
      text: Get Started
      link: /guide/
    - theme: alt
      text: View on GitHub
      link: https://github.com/rajasekharb/syne-compiler

features:
  - title: Execution Slicing (.slice)
    details: Extracts isolated execution paths from deep inheritance trees. Feed LLMs only the exact logic required for reliable refactoring.
  - title: Zero-Leakage Privacy
    details: Process monolithic codebases entirely locally. Keep proprietary, audited banking software secure and completely out of cloud APIs.
  - title: GraphRAG Ready (.strata)
    details: Compiles an Intermediate Representation (IR) knowledge graph. Map architectural blast radiuses before generating a single line of code.
---

## How It Works

Syne parses your legacy Java application locally and compiles the context into LLM-optimized artifacts.

```bash
# 1. Target the entry point of the monolith
$ syne compile src/main/java/com/bank/core/PaymentProcessor.java

# 2. Syne analyzes the AST and generates context artifacts
Compiling execution paths... [Done]
Extracting dependencies... [Done]
Building knowledge graph... [Done]

# Outputs generated:
# ➔ target/payment_flow.slice   (Optimized code prompt)
# ➔ target/architecture.strata  (GraphRAG IR)
```

## Why build a compiler for context?
LLMs struggle with deep, sprawling enterprise codebases. Dumping 50,000 lines of Java into a context window leads to hallucinations, massive token bills, and security risks.
Syne solves this by acting as a local pre-processor. By relying on deterministic static analysis and AST traversal, it distills the codebase so the LLM only "reads" what actually executes.
