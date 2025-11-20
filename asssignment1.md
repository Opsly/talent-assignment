# FastAPI Repository Chat Agent - Interview Assignment

## Overview

Build a production-ready chat agent that can answer questions about the FastAPI codebase using a knowledge graph and OpenAI's LLM. This assignment tests your ability to design scalable systems, work with graph databases, integrate LLMs, and write maintainable code.


## Objective

Create an intelligent chat agent that can:
- Index the FastAPI repository into a knowledge graph
- Answer technical questions about FastAPI's architecture, code patterns, and functionality
- Provide code examples and explanations based on the actual repository
- Handle multi-turn conversations with context retention

## Requirements

### 1. Repository Setup
- Clone the FastAPI repository: `https://github.com/tiangolo/fastapi`
- Parse and index Python files, documentation, and key metadata
- Focus on the core `fastapi/` directory

### 2. Knowledge Graph Implementation
- Design and implement a knowledge graph schema that captures:
  - Classes, functions, and methods
  - Dependencies and relationships between modules
  - Docstrings and code documentation
  - File structure and organization
- Use Neo4j, NetworkX, or any graph database of your choice
- Implement efficient querying mechanisms

### 3. Chat Agent Architecture
- Build a FastAPI application with the following endpoints:
  - `POST /api/chat` - Send a message and receive a response
  - `POST /api/index` - Trigger repository indexing
  - `GET /api/health` - Health check endpoint
- Implement conversation memory/context management
- Use OpenAI's API (GPT-4 or GPT-3.5-turbo) for response generation







### Configuration Requirements
- Use environment variables for sensitive data (OpenAI API key, database credentials)
- Implement proper configuration management (use Pydantic Settings)
- Support different environments (development, testing, production)

### Code Quality Standards
- Type hints throughout the codebase
- Comprehensive docstrings (Google or NumPy style)
- Error handling with custom exceptions
- Logging at appropriate levels
- Input validation using Pydantic
- Clean code principles (SOLID, DRY)

## Evaluation Criteria

### Architecture & Design (30%)
- Clear separation of concerns
- Proper dependency injection
- Scalable and maintainable structure
- Appropriate design patterns

### Code Quality (25%)
- Type safety and type hints
- Error handling and edge cases
- Code readability and documentation
- Testing coverage (aim for >70%)

### Functionality (25%)
- Accurate repository indexing
- Effective knowledge graph queries
- Quality of LLM responses
- Proper context management

### Production Readiness (20%)
- Configuration management
- Logging and monitoring
- Docker support (bonus)
- API documentation (OpenAPI/Swagger)
- Security considerations

## Deliverables

1. **Source Code**
   - Complete, working codebase
   - Follow the specified project structure
   - Include all dependencies in `requirements.txt`

2. **README.md**
   - Setup instructions
   - Architecture overview
   - API documentation
   - Design decisions and trade-offs
   - Known limitations

3. **Tests**
   - Unit tests for core services
   - Integration tests for API endpoints
   - Instructions for running tests

4. **Environment Configuration**
   - `.env.example` with required variables
   - Clear documentation of configuration options

## Bonus Points

- Implement caching for repeated queries
- Add rate limiting
- Create a simple frontend (React/Vue) to interact with the API
- Implement streaming responses
- Add observability (metrics, tracing)
- Docker Compose setup for all services
- CI/CD pipeline configuration
- Vector embeddings for enhanced semantic search
- Support for multiple repositories

## Sample Questions to Test

Your agent should be able to answer questions like:
- "How does FastAPI handle request validation?"
- "Show me an example of dependency injection in FastAPI"
- "What's the difference between Path and Query parameters?"
- "How does FastAPI generate OpenAPI schemas?"
- "Explain the lifecycle of a FastAPI request"

## Submission Guidelines

1. Create a private GitHub repository
2. Include all source code and documentation
3. Ensure the application runs with clear setup instructions
4. Provide a short video (5-10 min) or written walkthrough demonstrating:
   - Setup and installation
   - Indexing process
   - Example queries and responses
   - Code architecture highlights


**Good luck! We're excited to see your solution.**
