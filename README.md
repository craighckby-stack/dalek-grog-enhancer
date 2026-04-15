# Dalek Grog Enhancer: Sovereign v89.1 Evolution Engine

## Overview
Dalek Grog Enhancer (Sovereign Engine) is a high-frequency, context-aware code evolution system designed to automate repository refactoring through high-entropy mutations. It leverages a specialized "Auditor" persona to analyze project-wide documentation and inject architectural patterns across distributed codebases.

## Core Architecture

### 1. Sovereign Evolution Engine (`/enhancer`)
An advanced React-based orchestration layer that manages:
- **Contextual Indexing**: Prioritizes `README.md` and system prompts to prime LLMs with project-specific logic.
- **Mutation Cycles**: Automated cycles (defaulting to 4000ms) that iterate through file trees to perform refactors.
- **High-Entropy Protocol**: Utilizes Temperature 0.8 and specialized system prompts to ensure non-trivial, architectural improvements.
- **Telemetry**: Real-time monitoring of mutations, progress metrics, and error rates.

### 2. Siphon Engine Backend (`/engine`)
A TypeScript/Express proxy layer that secures and streamlines communication between the frontend and various high-performance AI providers:
- **Cerebras Proxy**: Fast inference using Llama 3.3 70B and 3.1 8B.
- **Grok Proxy**: Integration with x.ai's Grok-beta models.
- **Gemini Proxy**: Support for Google's Generative Language API.
- **GitHub Proxy**: Secure handling of repository read/write operations via personal access tokens.

## Technical Specifications
- **Frontend**: React (Hooks, useReducer, Custom Context), Vite
- **Backend**: Node.js, Express, TSX, TypeScript
- **Supported Languages**: JS, JSX, TS, TSX, Python, Rust, Go, C++, Java, Ruby, PHP, and more.
- **Evolution Model**: Sovereign Context-Aware Evolution (SCAE)

## Getting Started

### Prerequisites
- Node.js (v18+ recommended)
- GitHub Personal Access Token
- API Keys for one or more: Cerebras, x.ai (Grok), or Google (Gemini)

### Installation
1. **Environment Setup**:
   bash
   cp .env.example .env
   # Fill in GITHUB_TOKEN, CEREBRAS_API_KEY, and GROK_API_KEY
   

2. **Run the Engine**:
   bash
   cd engine
   npm install
   npm run dev
   

3. **Access UI**:
   Navigate to `http://localhost:3000` to launch the Sovereign interface.

## Operational Logic
1. **Priming**: The engine reads the target repository's README to understand intent.
2. **Sourcing**: It crawls the repo, ignoring standard noise (node_modules, dist).
3. **Inference**: Sends code snippets + context to the selected LLM via the Proxy layer.
4. **Mutation**: Commits the enhanced code back to the repository if evolution criteria are met.