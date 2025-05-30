# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This repository contains a Python technical specification representation of the U.S. Constitution. The main file `us_constitution.md` presents constitutional articles and sections as Python classes, dataclasses, and functions, along with Mermaid diagrams illustrating key constitutional processes.

## Project Structure

- `us_constitution.md` - The main document containing the Constitution represented as Python code with embedded Mermaid diagrams

## Development Notes

This is a creative documentation project that represents legal/governmental structures as code. When working with this repository:

1. Maintain Python syntax and idioms for consistency
2. Preserve the formal structure of constitutional articles and sections
3. Use appropriate Python constructs (dataclasses, classes, functions, enums) to represent governmental concepts
4. Keep code comments minimal - let the structure and naming convey meaning
5. Maintain the Mermaid diagrams for visual representation of processes

## Code Style

- Use Python 3.7+ syntax with type hints throughout
- Dataclasses for data structures (e.g., `Representative`, `Senator`)
- Functions for processes and eligibility checks
- Classes for institutional bodies (e.g., `HouseOfRepresentatives`)
- Enums for fixed categories (e.g., `Branch`, `BillType`)
- Maintain consistency with Python naming conventions (snake_case for functions/variables, PascalCase for classes)

## Visual Elements

The document includes Mermaid diagrams for:
- Separation of Powers overview
- Legislative Process flowchart
- Impeachment Process
- Amendment Process
- Supremacy Clause hierarchy