# Piano

**Status:** Live at https://smack-up.decoybecoy.com/piano/ (once pushed)
**Skill it practises:** Cause and effect, then exploring and targeting (look at a key and it plays), plus a simple choice (which sound)
**Characters:** None for now

## The idea in one sentence

Look at a piano and play sounds - have the option to set noise type.

## How it plays

A row of big, chunky keys across the screen, each a different colour. Looking at a key presses it down and plays its note, and a little burst of musical notes floats up from it. Moving his eyes along the keys plays a tune up or down the scale. Looking away lets the key spring back up.

Keys play almost straight away (about a third of a second of looking), so it feels like playing. Keeping his eyes on a key plays the note once, then again after a short pause. 8 keys (one scale) to start, with 5 bigger keys as a grown-up option.

### Sound row

A row of sound options across the top, each with a picture. Looking at one for about a second picks it (longer than the keys, so passing over them on the way to the keys doesn't change the sound). Leave a clear gap between the row and the keys.

- cow (moos in tune)
- sheep (baas in tune)
- musical note (standard tones, made by the game)
- fart (fart noises in tune), only shown when rude noises are on

The moo, baa and notes are made by the game itself (like the splats in Smack Up), so they're always exactly in tune. The fart is a real recording (free to use, see [audio/piano/README.md](../audio/piano/README.md)), sped up or slowed down for each note, because the made-up one sounded distorted.

### Tune buttons

Big buttons down the right that play a tune in whichever sound is picked, with the keys lighting up as it plays. Looking at one for about a second plays it.

The tunes come from the family folder Smack Up already uses (Google Drive or a folder on the computer), in a `tunes` folder inside it. Smack Up's photos now go in a `smack-up` folder alongside it. The link is set once per computer and shared by both games:

- One `.abc` file per tune. The file name is the button's name, like `Seven Nation Army.abc`.
- A picture with the same name (like `Seven Nation Army.jpg`) goes on the button. Optional.
- Up to three tunes at once. Family tunes come first, and free built-in tunes fill any empty buttons: In the Hall of the Mountain King, Twinkle Twinkle, Ode to Joy.
- Tune files can also end in `.txt`, or be a Google Doc in the folder.
- How to write one: [piano/README.md](../piano/README.md).
- If a tune goes higher or lower than the keys on screen, the game moves it to fit. A mistake in a file skips that note rather than stopping the tune.

The game itself doesn't contain any copyrighted tunes. Only the family's own folder does.

**Tune files** use ABC notation, a plain-text way of writing music that includes timing. Example:

```
T:Twinkle Twinkle
M:4/4
L:1/4
Q:1/4=100
K:C
C C G G | A A G2 | F F E E | D D C2 |
```

`L:1/4` means a plain letter is one beat, `G2` is two beats, `C/` is half a beat, `z` is a pause and `Q:` is the speed. Lots of tunes are already written in ABC online.

## The reward

The notes themselves, coloured notes floating up from each key, and the tune buttons.

## Grown-up settings

How many keys (8 or 5), how long to look before a key plays, rude noises on or off (fart sound), the Google Drive folder or a folder on the computer for tunes, sound, the gaze dot.

## Ideas and changes

- Play-along: keys glow one at a time to lead him through a tune he plays himself.
- Crookie as an audience, bopping along.
- MIDI files as well as ABC for tunes.
