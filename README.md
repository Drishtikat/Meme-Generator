# Random Meme Generator 

## Overview

This project is a **Random Meme Generator** that fetches a random joke from an API and reads it aloud using Text-to-Speech (TTS). It allows users to experience a fun and interactive way to listen to jokes, with an option to hear a new joke or exit the program.

The program utilizes the `requests` library to fetch jokes from an online API and the `pyttsx3` library to convert the joke text into speech. The user can interact with the program by pressing Enter to hear the punchline and decide whether to continue or exit after each joke.

## Features

- Fetches random jokes from the **Official Joke API**.
- Reads the joke aloud using the **pyttsx3 Text-to-Speech** engine.
- Allows users to interact with the program by choosing whether to hear another joke or exit.
- Supports customizable voice and speech rate.

## Prerequisites

To run this project, you need the following Python libraries:

- `requests` (for fetching jokes from the API)
- `pyttsx3` (for converting text to speech)

You can install these dependencies using `pip`:

```bash
pip install requests pyttsx3
```

## How It Works

1. **Text-to-Speech Engine**: 
   - The `pyttsx3` engine is initialized to convert text into speech.
   - The voice rate and type can be customized. By default, it uses a female voice with a moderate speech rate.

2. **Fetching Jokes**:
   - The program sends a GET request to the **Official Joke API** to retrieve a random joke.
   - The joke consists of two parts: a **setup** and a **punchline**.
   
3. **User Interaction**:
   - The joke setup is read aloud, and the user is prompted to press Enter to hear the punchline.
   - The punchline is then spoken out loud.
   - After each joke, the user can choose to hear another joke or exit the program.

4. **Exiting the Program**:
   - If the user opts not to hear another joke, the program will say goodbye and exit.


### Example Output

```plaintext
😂 Random Joke 😂

Why don't skeletons fight each other?

Press Enter for the punchline...
They don't have the guts!

Want another joke? (yes/no): no
Goodbye! Have a great day!
```

The program will continuously fetch jokes and read them aloud until the user opts to exit.
