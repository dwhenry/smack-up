# Piano

Big coloured keys you play by looking at them. Choose a sound across the top (moo, baa, notes or, with rude noises on, a fart), and look at a tune button on the right to hear a whole tune played in that sound, with the keys lighting up as it goes.

All the sounds are made by the game itself, so there are no sound files to download.

## Adding your own tunes

The game comes with three free tunes: In the Hall of the Mountain King, Twinkle Twinkle and Ode to Joy. You can add up to three of your own, and they take the first tune buttons.

Tunes live in the same family Google Drive folder as the Smack Up photos, in a folder inside it called `tunes`:

```
Family folder/        (shared as "Anyone with the link can view")
  smack-up/           photos for Smack Up
  tunes/              tunes for Piano
    Seven Nation Army.abc
    Seven Nation Army.jpg   (optional picture for the button)
```

1. Make a folder called `tunes` inside the family folder.
2. Put a tune file in it for each tune. The file name is the button's name, so `Seven Nation Army.abc` makes a button called “Seven Nation Army”.
3. Optional: add a picture with the same name and it goes on the button.
4. If Smack Up is already set up in this browser, that's it: Piano uses the same folder link. If not, open Piano's grown-up menu, paste the family folder link under **Tunes** and press **Load tunes**. It's then set for Smack Up too.

The link is saved in that browser. On another computer, paste the same link once and the tunes are there. Changes to the folder show up within a minute.

You can also choose a folder on the computer instead (the same one as Smack Up, with a `tunes` folder inside). Tune files can end in `.abc` or `.txt`, or be a Google Doc in the folder.

Tunes from your folder are only on your computer or your Drive, never on the public website. That's how songs still under copyright stay private to your family.

## Writing a tune file

Tunes use **ABC notation**, a plain-text way of writing music. Here's Twinkle Twinkle:

```
T:Twinkle Twinkle
M:4/4
L:1/4
Q:1/4=110
K:C
C C G G | A A G2 | F F E E | D D C2 |
```

The lines at the top:

| Line | Means |
|---|---|
| `T:` | The tune's name (the button uses the file name instead) |
| `M:4/4` | Beats in a bar |
| `L:1/4` | How long a plain note is: `1/4` is one beat, `1/8` is half a beat |
| `Q:1/4=110` | Speed: 110 beats a minute |
| `K:C` | The key. `K:G` adds the F sharps for you, `K:Em` is E minor |

The notes:

| Write | Means |
|---|---|
| `C D E F G A B` | The notes from middle C upwards |
| `c d e` | An octave higher |
| `C, B,` | An octave lower |
| `G2` `G3` `G/` `G3/2` | Twice as long, three times, half as long, one and a half |
| `^F` `_B` `=F` | Sharp, flat, back to natural |
| `z` `z2` | A pause |
| `\|` | A bar line (just for reading, apart from resetting sharps and flats) |
| `\|: … :\|` | Play this bit twice |

Lots of tunes are already written in ABC online. Search for the tune's name plus “abc”. If the game can't read a note it skips it, and the menu tells you if a file had no notes it could read.

The game moves a tune up or down so it fits the keys on screen, and any sharps and flats light up the nearest key.
