# Lab 01: Explicit Agent Loop

## Question

What is the smallest understandable tool-using agent loop that makes state,
decisions, tool calls, validation, and stopping conditions explicit?

## Learning Objectives

- Understand the components of a tool-using agent loop
- Represent tool inputs and outputs with typed schemas
- Separate model decisions from deterministic execution
- Identify failure boundaries
- Test the loop without depending on a live model

## Initial Scope

- One deterministic mock model
- One typed tool
- Explicit tool dispatch
- Input validation
- Explicit loop state
- Clear stopping conditions
- Unit tests for successful and invalid tool calls

## Non-Goals

- Durable persistence
- Multiple agents
- Kubernetes deployment
- Model routing
- Sandboxed command execution
- A general-purpose agent framework

## Acceptance Criteria

- Every state transition is visible in the implementation
- Invalid tool arguments are rejected safely
- Tool execution is deterministic and independently testable
- The complete lab runs from a clean checkout
- The README explains the design without relying on framework terminology