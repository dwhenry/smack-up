# Catch Me

**Status:** Live at https://smack-up.decoybecoy.com/catch-me/ with anime-style garden, cupboard and hedge maze backgrounds
**Skill it practises:** cause and effect / targeting /
**Characters:** Tank, a cheeky hamster in a ball (our own character, not Rhino from Bolt).

## The idea in one sentence

hamster runs around the screen, when you look at him he bnounces off like a pinball around teh screen.

## How it plays

So the screen vary between games, but all of them with the same maze shape so the player can predict where they go next. so 4 levels with 3 bridges betwwen each level.

one is a garden with flowers (prefer a nice generated image for the background), one is a cupboard with angled book to changes levels and the last is a actual maze. don;t draw them yourself, find a free graphics engine to generate better quality images for these background.

## Layout

Four paths run across the screen, one above the other, with three ladders (or bridges or ramps) in each gap. They're staggered so he zig-zags, and the layout is the same in every theme so the player can learn where he'll go next.

```
======================================   path 1 (27% down the screen)
H              H                    H    ladders at 4%, 36%, 96% across
======================================   path 2 (49%)
       H                 H        H      ladders at 16%, 58%, 84%
======================================   path 3 (71%)
H                H                  H    ladders at 4%, 40%, 96%
======================================   path 4 (93%)
```

**Landscape only.** The layout only works on a wide screen. On a phone held upright the game shows a friendly “turn your phone sideways” screen instead, and carries on when it's turned. Phones aren't the main use, so this just needs to not break.

The hamster runs along the top of a path and can climb or hop to the next path at a ladder. When he's caught he breaks free, pinballs off the edges of the screen for a few seconds, then drops back onto the nearest path and carries on.

## Backgrounds

Each theme is one picture, made with a free AI image generator, that shows the paths and ladders in exactly these places. The game measures where the paths are in each finished picture, so the hamster runs along what you see. The hamster himself is drawn and animated by the game (a generator can't make him move).

**Layout guide:** [catch-me/layout-guide.png](../catch-me/layout-guide.png) is a plain black-and-white drawing of the layout at 16:9. Give it to the generator as a structure reference so the scenery is built around it.

**How (Adobe Firefly, free account with monthly credits):** sign in at firefly.adobe.com → **Generate** in the left panel → **Generate image** → set the aspect ratio to **Widescreen (16:9)** → open **Composition** → under **Reference**, choose **Upload image** and pick `layout-guide.png` → move the **Strength** slider high → paste a prompt below → **Generate** → download the best one. Save it as `catch-me/garden.jpg`, `catch-me/cupboard.jpg` or `catch-me/maze.jpg`. Adobe renames these menus from time to time; if they've moved, look for the reference or composition option.

Start every prompt with this, then add the theme. If Firefly has a style option, choose **Art** as the content type and try the anime or illustration styles:

> High-quality anime background art for a children's game, hand-painted look, rich detail, soft warm lighting, vibrant but gentle colours, side view, no characters, no animals, no text, no people. Keep the reference layout exactly: four long flat horizontal walkways across the full width, clearly visible, with short ladders between them in the same places, and open space at the top. Keep the walkways and ladders bold and easy to see against the scenery.

- **Garden:** a sunny summer garden in late afternoon light. The four walkways are long wooden planks along raised flower beds, with soil and roots below each one. The ladders are little wooden garden ladders and bean poles. Flowers, leaves and the odd snail between the walkways; blue sky with fluffy clouds at the top.
- **Cupboard:** inside a cosy wooden cupboard. The four walkways are long wooden shelves. Between the shelves, books lean at an angle as ramps where the ladders are. Jars, tins and toys along the back wall; warm lamp light at the top.
- **Maze:** a hedge maze in a grand garden, seen from the side. The four walkways run along the tops of tall green hedges. The ladders are little stone staircases cut into the hedges. Flowers and archways in the hedges; sky at the top.

If a result doesn't follow the layout closely, try again or turn the structure strength up. Leaning books are fine: the game handles ramps as well as straight ladders.

**Style match:** Tank is drawn by the game in a clean cartoon style with dark outlines. Painted anime scenery behind a cel-style character is a normal anime look, so it should sit well; once the first background is in, I'll check how he looks against it and adjust his colours or outline if he gets lost.

## The reward

He has lots of sayings as he runs around.. and stands up and flexes, but once hit he bounces and moans one his catch phrase.

## Things Crookie (or anyone) says

| Line           | When         |
| -------------- | ------------ |
| can't catch me | when running |
| look at me go  | when running |
| you got lucky  | when hit     |
| not again      | when hit     |

Suggestions (keep the ones you like):

| Line | When |
| ---- | ---- |
| Too fast for you! · Over here! · Wheee! · Bet you can't find me! · Hamster power! | when running |
| Check out these muscles! · Feel the burn! · Am I amazing or what? · Ten out of ten hamster! | when he stops to flex (an easy moment to catch him) |
| Whoaaaa! · Ow, my ball! · Best two out of three! | when hit |
| I'm all dizzy… · I'm OK! · That didn't hurt… much. | after bouncing |
| Hello? Anyone there? · I'll just do some push-ups then. | when nobody's looking for a while |

## Grown-up settings

Speed of the hamster (low med high)
Distance to hamster (how close they have to be to trigger a hit)
Length of hit (how long the hit should be help before it trigger a hit action)

Suggested extras: theme (garden, cupboard, maze or random), how wild and how long the pinball bounce is, slow down when looked at (on or off), sound, the hamster talks, show where he's looking. Plus the usual grown-up menu, full-screen PLAY and a catch counter with a celebration every 10.

## Ideas and changes

-

## Open questions

- **Decided:** his name is **Tank**.
- **Decided:** he's our own hamster, not Rhino from Bolt: a chunky ginger-and-cream hamster in a see-through ball, wearing a red sweatband (he's into fitness, hence the flexing).
- **Skill stage:** catching something that moves is targeting a moving target, a step up from Look and Go. Slowing down when looked at, the flex pauses and a generous catch distance keep it gentle.
