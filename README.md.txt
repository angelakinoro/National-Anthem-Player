# Arduino Melody

This repository contains an Arduino sketch to play the first stanza of the Kenyan National Anthem using a buzzer. The melody is defined using musical notes and their corresponding frequencies, and the tempo can be adjusted to play the song faster or slower.

## Features

- Plays a melody through a buzzer.
- Supports adjustable tempo.
- Uses defined musical notes and their frequencies in Arduino code.

## Requirements

- Arduino board (e.g., Arduino Uno, Nano, etc.)
- Buzzer
- Arduino IDE for uploading the code to the board

## How to Use

1. **Connect the Buzzer**: Connect the positive leg of the buzzer to pin `8` on your Arduino board and the negative leg to `GND`.

2. **Upload the Code**:
   - Open the `melody.ino` file in the Arduino IDE.
   - Select the correct Arduino board and port in the IDE.
   - Upload the code to your Arduino board.

3. **Adjust Tempo** (Optional):
   - You can change the tempo of the melody by adjusting the `tempo` variable in the code. The default is `80` beats per minute.
   - Higher values will make the song play faster, while lower values will make it slower.

4. **Enjoy the Melody**: Once uploaded, the melody will automatically play once and stop.

## Code Explanation

- The melody is stored in an array called `melody[]` where each note is followed by its duration.
- The `tone()` function is used to generate the correct frequency on the buzzer for the duration of the note.
- The `delay()` function is used to wait for the specified duration before playing the next note.
- Dotted notes are handled by multiplying their duration by `1.5`.

## Example Melody

The melody is defined using musical notes such as:

- `NOTE_A4` (440 Hz)
- `NOTE_B4` (494 Hz)
- `REST` (no sound, silence)

The array of notes defines the song's structure with varying note lengths, including quarter, eighth, and dotted notes.


