# Your Little Solfège Friend

This Python script allows users to generate and play rhythms using simple beep sounds in an interactive Jupyter Notebook environment. Users can specify the tempo and a series of notes identified by their type (whole, half, quarter, etc.), and the program will play the rhythm using beep sounds corresponding to the duration of each note.
The notes' duration is based on the tempo and the note type, and the beep sounds are generated using the `simpleaudio` library. However, the notes' pitch is not considered in this script, so the beep sounds are all the same frequency. You can change the frequency of the beep sound by changing the `frequency` variable in the `generate_beep` function. The default frequency is 440 Hz, which corresponds to the A4 note.

*Note: I changed the keywords for the notes with what I was more comfortable with, which is explained in `play_rhythm` function. Feel free to change it with whatever floats your boat.*

## Features

- **Tempo Control**: Adjust the tempo (BPM) using a slider to speed up or slow down the rhythm playback.
- **Rhythm Input**: Input a series of notes using short aliases (w for whole, h for half, q for quarter, e for eighth, s for sixteenth) and optionally add a 'd' at the end for *dotted notes* which increase the duration by 50%.
- **Interactive Playback**: Play the rhythm based on the input series of notes and tempo with a simple click of a button.

## How to Use

1. **Setup**: Ensure you have a Jupyter Notebook environment with IPython, numpy, simpleaudio, and ipywidgets installed.
2. **Launch**: Open the notebook and run the provided Python script.
3. **Adjust Tempo**: Use the tempo slider to set the desired beats per minute (BPM) for your rhythm.
4. **Input Rhythm**: In the rhythm text box, input your series of notes separated by spaces. Use the aliases for note types
*example:* (e.g., `q q h` for two quarter notes followed by a half note).
5. **Play Rhythm**: Click the "Play Rhythm" button to hear the rhythm played back as beep sounds.

## Dependencies

- numpy
- ipywidgets
- simpleaudio

Make sure these libraries are installed in your Python environment to run the script successfully.

## Example

After running the script in a Jupyter Notebook cell, you might set the tempo to 120 BPM and input `q q h` in the rhythm text box. Upon clicking "Play Rhythm," you'll hear two quarter notes followed by a half note played at the specified tempo.

## Note

This script is intended for my own educational use since my stupid mind loses the track of a metronome after a few seconds. Feel free to use it for your own educational purposes! 