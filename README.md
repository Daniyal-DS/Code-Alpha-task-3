# AI-Powered Music Generation System

This project uses deep learning techniques to generate original music. It leverages Recurrent Neural Networks (RNNs) with Long Short-Term Memory (LSTM) layers to learn patterns from MIDI files and compose new music sequences.

## Features
- Load and preprocess MIDI files.
- Train an LSTM-based model to learn musical patterns.
- Generate new music sequences.
- Save generated music as a MIDI file.

## Requirements
- Python 3.x
- TensorFlow
- music21

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Daniyal-DS/Code-Alpha-task-3
   cd ai-music-generation
   ```

2. Install the required libraries:
   ```bash
   pip install tensorflow music21
   ```

## Usage
1. Place your MIDI files in the `midi_files` directory (or update the path in the code).
2. Run the Jupyter Notebook or Python script:
   ```bash
   jupyter notebook music_generation.ipynb
   ```
3. The script will:
   - Load and preprocess the MIDI files.
   - Train the LSTM model.
   - Generate new music and save it as `output.mid`.

4. Download the generated MIDI file:
   ```python
   from google.colab import files
   files.download('output.mid')
   ```

## Code Overview
- **Install Libraries**: Installs TensorFlow and music21.
- **Import Libraries**: Imports necessary libraries for data processing and model building.
- **Load and Preprocess Data**: Loads MIDI files and extracts notes and chords.
- **Prepare Data**: Converts notes into sequences and reshapes them for the LSTM model.
- **Build Model**: Constructs the LSTM model with dropout layers.
- **Train Model**: Trains the model on the prepared data.
- **Generate Music**: Predicts new music sequences using the trained model.
- **Create MIDI File**: Saves the generated music as a MIDI file.
- **Download MIDI File**: Downloads the generated MIDI file.

## Example
To generate music from the Pakistan National Anthem:
1. Upload `pakistan_anthem.mid` to the `midi_files` directory.
2. Run the script.
3. Download and listen to the generated `output.mid`.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
