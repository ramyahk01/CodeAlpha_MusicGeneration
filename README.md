# 🎵 AI Music Generation using LSTM

A deep learning project that generates new music after learning patterns from Bach chorales. Built with **TensorFlow/Keras** and **music21** as part of the CodeAlpha internship program.

## ✨ Features

- Extracts notes and chords from Bach chorales using music21
- Preprocesses sequences with NLTK-style tokenization approach
- Trains a 2-layer LSTM neural network on 50-note sequences
- Generates 200 new notes based on learned patterns
- Converts generated notes back to MIDI format
- Downloadable output file playable in any media player

## 🛠️ Tech Stack

| Component | Technology |
|-----------|------------|
| Language | Python 3.13 |
| Deep Learning | TensorFlow 2.x + Keras |
| Music Processing | music21 |
| Data Handling | NumPy |
| Platform | Google Colab (T4 GPU) |

## 🧠 How It Works

1. Load Bach chorales from music21's built-in corpus
2. Extract all notes and chords as string tokens
3. Build a vocabulary of unique notes/chords
4. Create training sequences (50 notes → next note)
5. Normalize and one-hot encode the data
6. Train LSTM model (2 layers, 256 units each)
7. Generate new sequences by predicting note-by-note
8. Convert generated sequence to MIDI using music21
9. Save and download the output file

## 🚀 How to Run

1. Open Google Colab: https://colab.research.google.com
2. Upload `Music_Generation_LSTM.ipynb` (File → Upload notebook)
3. Enable GPU: Runtime → Change runtime type → T4 GPU → Save
4. Install music21 (first cell):
   ```bash
   !pip install music21
5. Run all cells in order (Runtime → Run all)
6. Wait for training to finish (~15-25 min on GPU)
7. Listen to the generated generated_music.mid file

## 📁 Project Structure
CodeAlpha_MusicGeneration/
├── Music_Generation_LSTM.ipynb    # Main Colab notebook
├── generated_music.mid            # Sample generated output
└── README.md                      # Project documentation

## 🎼 Output
The model generates a 200-note sequence in MIDI format. The output is a short piece of classical-style music inspired by Bach's compositional patterns.

## 👤 Author
Ramya H K — B.Tech AI & ML Student

## 📜 License
This project is part of the CodeAlpha internship program.
