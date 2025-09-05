# 🎭 The Empathy Engine

An advanced AI voice synthesis system that transforms plain text into emotionally expressive speech, designed to sound naturally human with nuanced breathing, pauses, and emotional intensity.

---

## Features

- **Emotion Analysis:** Combines Hugging Face Transformers and VADER sentiment for rich emotion detection mapped onto Valence, Arousal, and Dominance dimensions.
- **Expressive Breathing Sounds:** Inserts realistic breathing audio at controlled intervals for natural voice effects.
- **Dynamic Pauses:** Adds clearly audible longer pauses after sentence endings to mimic human speech rhythm.
- **Controlled Speaking Rate:** Slows down speech by 10% overall, improving clarity and naturalness.
- **Audio Post-Processing:** Applies normalization and dynamic range compression for pleasant, consistent volume.
- **Interactive Web Interface:** Built with Gradio for easy testing, input entry, and immediate audio playback.

---

## Quick Start

### Prerequisites

- Python 3.7+
- Required packages: `gradio`, `torch`, `transformers`, `vaderSentiment`, `gTTS`, `pydub`



### Setup

- Place a short breathing audio file named `Breathing_.wav` in your working directory or update the path in the code.
- Run the Jupyter notebook `empathy_engine.ipynb` which contains the complete, end-to-end implementation.

### Running the Project

1. Start the Jupyter notebook and run all cells sequentially.
2. The Gradio web interface will launch automatically.
3. Input your text and generate emotionally expressive speech with real-time feedback.

---

## Usage Example

Input:  
`I'm so excited about this amazing project!`

Output:  
An MP3 audio file with speech modulated to sound enthusiastic, with dynamic breathing sounds, longer pauses, and louder emphasis on emotional peaks.

---

## Design Highlights

- **Emotion Detection:** Uses `j-hartmann/emotion-english-distilroberta-base` transformer to classify emotions and VADER sentiment for intensity.
- **Voice Modulation:** Adjusts speech rate, inserts pauses and breaths, and boosts volume dynamically based on emotion.
- **Audio Processing:** Uses `pydub` for concatenation, normalization, compression, and speed adjustment.
- **Web UI:** Streamlined interface supporting instant text input, visualization, and audio playback.

---

## Development Notes

- The breathing sound volume and frequency are carefully adjusted to be audible but not overwhelming.
- The overall speech speed is slowed by 10% to enhance naturalness.
- Emotional loudness spikes are applied selectively to stressed phrases.
- Chunking preserves word integrity to avoid unnatural word cutting during TTS.

---


# 🚀 Extra Miles Beyond the Original Project

## What We Added to Make This Project Special:

- **Chunk-wise Speech Synthesis:** Ensured no words are cut by splitting input text into meaningful chunks before synthesis, improving clarity and naturalness.

- **Realistic Breathing Sounds:** Injected audible breathing audio at carefully spaced intervals to mimic human voice patterns and enhance empathy.

- **Dynamic and Longer Pauses:** Added natural, longer pauses after punctuation for better conversational pacing.

- **Stress-Based Loudness Boost:** Amplified volume significantly during emotional or stressed phrases for expressive impact.

- **Slowed Down Speech:** Reduced overall speaking speed by 10% to create a calmer, more thoughtful voice.

- **Audio Post-Processing:** Applied normalization and dynamic compression for consistent volume and pleasant listening experience.

- **Implemented Web UI:** Created an instant, easy-to-use interface to test and listen to emotional TTS outputs live.

---

These enhancements bring the voice closer to genuine human speech, making the AI feel more empathetic and relatable—beyond the basic original requirements.

## Future Enhancements that can be done

- Integrate higher-quality neural TTS APIs supporting emotional control.
- Add SSML tags for fine-grained prosody control.
- Support user-selectable voice personas and multilingual speech.
- Enhance emotional context awareness across multi-turn conversations.



## Acknowledgments

Developed using Hugging Face Transformers, VADER Sentiment, Google Text-to-Speech (gTTS), pydub, and Gradio.

The empathy concept inspired by next-generation human-like conversational AI research.

---


