# Ensemble - Dynamic Group Director

Ensemble adds an "AI Director" to SillyTavern group chats. Instead of a rigid round-robin or manual selection, the Director analyzes the conversation flow and mathematically determines which character should speak next.

## Features
- **Dynamic Initiative**: Characters speak based on relevance (mentions, keywords) and recency.
- **Director Mode**: Enable/Disable the AI Director on the fly.
- **Steering**: Use `/direct "Instruction"` to force a specific topic for the next speaker.
- **Auto-Turn Limiter**: Prevents infinite loops between AI characters.

## Installation
1. Unzip the `ensemble` folder into `public/scripts/extensions/`.
2. Reload SillyTavern.
3. Open the Extensions menu and find "Ensemble".
4. Enable "Director Mode".

## Settings
- **Initiative Threshold**: How confident a character needs to be to interrupt. Higher = less frequent interruptions.
- **Talkativeness Bias**: Global multiplier for how often characters speak.
- **Max Auto-Turns**: How many AI-to-AI turns are allowed before waiting for the user.

## Usage
Just start a group chat and enable Director Mode. The characters will naturally converse with each other.

To steer the conversation:
`/direct "Argue about who is the strongest"`
The Director will pick the most relevant character and inject that instruction into their prompt.
