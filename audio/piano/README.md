# Piano sounds

The notes are made by the game itself. The moo, baa and fart are real recordings, sped up or slowed down by the game to play each note, and fitted to each note's length.

| File | What | Where it's from | Licence |
|---|---|---|---|
| `cow.mp3` | One long moo | [“Cow moos #6”, BigSoundBank](https://bigsoundbank.com/cow-moos-6-s2386.html) | CC0 (public domain) |
| `sheep.mp3` | One baa | [“Sheep #5”, BigSoundBank](https://bigsoundbank.com/sheep-5-s2347.html) | CC0 (public domain) |
| `fart.mp3` | One fart | [“Flatulence #1”, BigSoundBank](https://bigsoundbank.com/pet-1-s0111.html) | CC0 (public domain) |

CC0 means free to use for anything, with no credit needed. These were picked from the free recordings because each holds a fairly steady pitch, so the keys stay in tune with each other.

To swap one, replace the file and update its line in `SAMPLES` in [piano/index.html](../../piano/index.html). `ref` is the note that plays the recording at its own speed. The times say where in the recording the sound starts, which steady part repeats for long notes, and where it tails off.
