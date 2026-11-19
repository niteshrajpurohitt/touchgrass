# touchgrass

Type a friend's name. Watch them go outside.

**[touchgrass.niteshrajpurohit.in](https://touchgrass.niteshrajpurohit.in)**

![touch grass, Elon.](demo.gif)

A tiny hand-drawn animation you can send to anyone who has been online too long. Type their name and press Enter. A person puts down their phone, the furniture flies away, they walk outside, the grass grows, and they sit down to smell a flower. Then the words write themselves: *touch grass, Elon.*

## What you can do

- **Type a name** straight onto the picture and press Enter (or tap the key on a phone).
- **Pick the opening scene**: scrolling in bed, or working at a desk.
- **Pick the character**: two to choose from.
- **Pick the wording**: touch grass, go outside, or log off.
- **Pick the colours**: five themes, including a night one.
- **Turn on the sound** with the speaker button: key clicks as you type, a whoosh as the room flies off, and soft music outdoors.
- **Save it** as a video (with sound), GIF or JPG, in 9:16 or 16:9.
- **Share it** as a file, or as a link that plays the animation for your friend with their name in it.

## How it's built

- One `index.html` file. Plain JavaScript and a canvas, with no framework and no build step.
- Everything is drawn in code. There are no image assets in the animation: every line is a path with a slight wobble that redraws eight times a second, which gives the hand-drawn "boiling" look.
- The person is a small skeleton posed with forward and inverse kinematics, so walking, sitting and reaching for the flower are all computed.
- The sound is made in code too, with the Web Audio API. There are no audio files.
- Video is encoded in the browser with WebCodecs and [mp4-muxer](https://github.com/Vanilagy/mp4-muxer), and GIFs with [gifenc](https://github.com/mattdesl/gifenc). Nothing is uploaded anywhere.
- The font is [Shantell Sans](https://fonts.google.com/specimen/Shantell+Sans).

## Run it locally

Download the repo and open `index.html` in a browser. That's all.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole site |
| `og.png` | The preview picture shown when the link is shared |
| `demo.gif` | The animation shown at the top of this page |
| `icon.png` | The home-screen icon |
| `vercel.json` | Security headers for hosting on Vercel |

## Privacy

No accounts, no cookies, no tracking of what you type. The name lives only in the link you share. The site uses Vercel Web Analytics to count visits.
