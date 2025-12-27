# Music Literacy Gym (Mandolin, Mandola, Guitar, Bass)

A browser-based music literacy “gym” that generates **two-measure (4/4 + 4/4)** sight-reading lines using:
- quarter notes
- quarter rests
- eighth-note pairs

Play the line; the current note highlights **pink**, completed notes highlight **green**. When you finish the full line, the app waits **1 second**, plays a **ding**, waits **1 second**, then loads a new exercise automatically.

## Run locally
Open `index.html` in Chrome.

> Mic permissions often require HTTPS or localhost. If mic is blocked when opening as a file:
>
> `python3 -m http.server 8000`
>
> Then open `http://localhost:8000`

## Pitch notes
- Mandolin / Mandola: sound as written
- Guitar / Bass: sound one octave lower than written (handled internally for matching)

## Tech
- VexFlow (notation rendering via CDN)
- WebAudio + getUserMedia (real-time pitch detection)
