# Discord Bot - Amom (Demonic Oracle)

## Overview

This project is a Discord bot named "Amom" that acts as a demonic oracle character. The bot integrates with OpenAI's GPT API to provide mystical, enigmatic responses to user questions in character as a demon of knowledge. The bot is designed to respond to slash commands and maintain a consistent persona throughout all interactions.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Bot Framework
- **Discord.py Library**: Uses the discord.py library with the commands extension for structured command handling
- **Command System**: Implements slash commands with `/profecia` as the primary interaction method
- **Intent Configuration**: Currently configured with default intents (privileged intents like message_content are commented out to avoid permission requirements)

### AI Integration
- **OpenAI API**: Integrates with OpenAI's ChatGPT API for generating character-appropriate responses
- **Persona System**: Uses a system prompt (`PROMPT_PERSONA`) to maintain consistent character behavior as "Amom, a demon of knowledge"
- **Context Preservation**: Each interaction includes the base persona prompt to ensure character consistency

### Security and Configuration
- **Environment Variables**: Sensitive data (Discord token, OpenAI API key) is loaded from environment variables
- **Token Management**: Bot token and API keys are kept separate from the codebase for security

### Character Design
- **Persona**: "Amom" (Marquês Amon) - a demonic oracle connected to past, present, and future
- **Response Style**: Mystical, enigmatic, and oracle-like responses delivered in an infernal pub setting
- **Character Consistency**: Strict instructions to never break character regardless of user input

### Channel Management
- **Target Channel**: Originally designed to work in a specific channel called "Oráculo" 
- **Flexible Deployment**: Channel restrictions are currently disabled for easier testing and deployment

## External Dependencies

### Required APIs
- **Discord API**: For bot functionality, server connection, and user interaction
- **OpenAI API**: For GPT-based response generation and character roleplay

### Python Libraries
- **discord.py**: Discord bot framework and API wrapper
- **openai**: Official OpenAI Python client library
- **os**: For environment variable management

### Environment Configuration
- **DISCORD_TOKEN**: Bot authentication token from Discord Developer Portal
- **OPENAI_API_KEY**: API key for OpenAI services
- **Runtime Environment**: Designed to run on platforms supporting Python environment variables

### Potential Integrations
- **Discord Server**: Requires invitation to target Discord server with appropriate permissions
- **Hosting Platform**: Designed for deployment on cloud platforms like Replit, Heroku, or similar services