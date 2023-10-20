# COCA Project

## Overview
COCA (Captivating Original Conversations through Art) is an interactive art installation that allows museum visitors to have natural conversations with digitally rendered portraits. Inspired by the living portraits in Harry Potter, this project uses facial tracking and natural language processing to create an immersive magical realism experience.

Visitors can interact with the portraits in two ways:
1. **Facial Mimicry** - Cameras track visitors' facial expressions and movements in real-time, mapping their expressions onto the digital portraits to bring them to life.
2. **Conversational AI** - Visitors can activate a microphone to ask the portraits questions. Speech recognition transcribes the query, which is then processed by a natural language model to generate a relevant conversational response.

## Technical Implementation
The project uses the following technologies:
- **Next.js** - React framework for building user interfaces and rendering portrait mimicry.
- **Face API** - For tracking facial landmarks and mapping expressions.
- **GPT-3 API** - Natural language processing for analyzing queries and generating responses.
- **Speech to Text** - Transcribing user's spoken questions.
- **Text to Speech** - Converting generated responses into lifelike voice.

## System Architecture
![System Architecture](system-architecture-image-url)

The frontend uses React components and canvas elements to display the portraits. Face API integrates with the camera to handle facial tracking. Speech recognition and GPT-3 APIs are called via REST endpoints.

## Interaction Flow
1. User approaches interactive portrait station.
2. Frontend activates device camera and begins facial tracking.
3. User expressions are mirrored on the digital portrait in real-time.
4. User pushes the mic button and asks the portrait a question.
5. Audio is streamed to the Speech to Text API.
6. Transcript is sent to the GPT-3 API for processing.
7. GPT-3 generates a conversational response.
8. Response text is passed to the Text to Speech API.
9. Portrait plays vocalized response to the user.
10. Showcase

