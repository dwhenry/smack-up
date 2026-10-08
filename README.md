# Smack Up

An eye-gaze practice game. Photos float down on parachutes. Look at one and keep looking: a yellow ring fills up, the photo slows down and wobbles, and then something gets thrown at it. It might be a cream pie, a cake, a tomato, an egg, slime, a water balloon, a rubber chicken, a fish, or (if rude noises are on) the photo makes a farting noise and zooms off like a let-go balloon. Every 10 splats there's confetti.

The whole game is one file, `index.html`. It doesn't need a server or anything installed on the device.

## Play it online

The game lives at **https://smack-up.decoybecoy.com**. Anyone can use it: open the page, go to Settings (⚙ twice, or Esc), paste the link to your own shared Google Drive folder and click "Load photos". The folder link is saved in that browser only. It never goes to the website, and other people using the game can't see it.

## Setting it up on the Tobii Dynavox I-12+

1. **Make the eye gaze move the mouse pointer.** The game works out where he's looking from the mouse pointer, so the eye tracker needs to be in its mouse or computer-control mode. Depending on which software your I-12+ has, that's Windows Control, Gaze Interaction or Computer Control (or "Computer Control" inside Communicator / TD Snap). If the pointer follows his eyes on the Windows desktop, you're set. Dwell-clicking can stay on: a stray click won't do anything in the game.
2. **Use Chrome or the new Microsoft Edge.** Old Internet Explorer and the old Edge won't run it. Windows 10 with an up-to-date Edge is fine.
3. **Open https://smack-up.decoybecoy.com** in Chrome or Edge on the I-12+. If the device is often offline, copy `index.html` onto it and open that instead.
4. **Connect the shared photo folder** (see below), or click "Choose photo folder" to use a folder on the device instead.
5. **Press "Full screen & play".** In Chrome and Edge, a quick tap of Esc in full screen opens the settings, and you have to *hold* Esc down to leave full screen. That makes it hard for him to come out of the game by accident.

## The shared photo folder (Google Drive)

The game loads photos straight from a Google Drive folder over the internet, so nothing needs installing on the I-12+. It's free, and anyone you invite can add or delete photos from the Google Drive app on their phone. The game checks the folder about once a minute, so new photos turn up while he's playing.

**1. Make the folder (2 minutes)**

1. In Google Drive, make a new folder, for example "Splat photos".
2. Click **Share**. Under "General access", choose **Anyone with the link** and leave it as **Viewer**. The game needs this to see the photos.
3. In the same box, add family by email address as **Editors**. Each of them needs a Google account. They'll get the folder in their own Drive app.
4. Click **Copy link**.

Anyone who has that link can look at the photos, so share the link only with people you'd trust with the photos.

**2. Get a free Google API key (5 minutes, once only)**

The key lets the game ask Google for the list of photos. It doesn't need a credit card.

1. Go to [console.cloud.google.com](https://console.cloud.google.com) and sign in with the same Google account.
2. Create a project, for example "Smack Up".
3. Go to **APIs & Services → Library**, search for **Google Drive API** and click **Enable**.
4. Go to **APIs & Services → Credentials → Create credentials → API key**.
5. Click the new key, and under **API restrictions** choose **Restrict key → Google Drive API**. Save, then copy the key (it starts `AIza`).

The key can only read files that are already shared with "Anyone with the link". It can't see anything else in your Drive.

If the key is for the website, lock it to the site: under **Application restrictions** choose **Websites** and add `https://smack-up.decoybecoy.com/*`. Then put the key in the `DRIVE` line of `index.html` (below) and push the change. Visitors will then only need their folder link. A key locked to the website won't work from a copy of the file on a computer, so that copy needs its own unrestricted key in Settings.

**3. Put them into the game**

Either open Settings on the device and paste the folder link and the key into the "Google Drive" boxes, or (handier if you'll copy the game onto other computers) open `index.html` in a text editor and fill in this line near the top of the script:

```js
const DRIVE = { folder: 'https://drive.google.com/drive/folders/…', apiKey: 'AIza…' };
```

Put photos straight into the folder rather than into folders inside it. Photos named something like `Grandma.jpg` or `Uncle Pete.png` get that name written under them. Camera names like `IMG_1234.jpg` are left blank. iPhone HEIC photos work too, because Google converts them.

## Grown-up controls

- **Settings:** click the ⚙ in the top-right corner twice, or press Esc. The game pauses while settings are open.
- **How long to look** (default 1 second) and **How close counts** (default 50px): start easy, with a longer look time and a bigger "close" area, then make them harder as he gets the hang of it.
- **Falling speed, photo size and how many photos fall at once.**
- **Which splats to use**, sound on or off, and rude noises on or off.
- **Show where he's looking:** a soft yellow dot. Some children find it helps and some find themselves chasing it, so try it both ways.
- He can start the game himself by looking at the big PLAY button until it fills up.

## Good to know

- With Google Drive the device needs internet. With a local folder it works offline, but HEIC photos won't show (JPG, PNG, GIF and WebP do).
- The game itself never uploads anything.
- If no folder is picked yet, or the folder is empty, the game uses sample animal faces so there's always something to splat.
