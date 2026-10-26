# Music Playlist Manager

A web app that manages a music playlist using a **doubly linked list**.

**Live demo:** _paste your GitHub Pages link here_

## DSA concept: Doubly linked list

Each song is a node holding the song data plus two pointers, `prev` and `next`. The list keeps `head`, `tail` and a `cur` pointer for the song that is playing. Because every node knows its neighbours in both directions, the player can move forward and backward and can insert or remove a song without shifting anything.

| Operation | Use in the app | Time |
|-----------|----------------|------|
| `addEnd` | Add a song at the tail | O(1) |
| `addAfterCurrent` | "Play next": insert after the current node | O(1) |
| `removeCurrent` | Delete the playing song and relink its neighbours | O(1) |
| `next` / `prev` | Move the current pointer | O(1) |
| `reverse` | Swap `prev` and `next` in every node | O(n) |

## Features
- Add songs to the end or right after the current song
- Next and previous controls
- Remove the current song
- Reverse the whole playlist
- Head, tail and playing labels, with an operation log

## Run it
Open `index.html` in a browser. No install or build step.

## Tech
HTML, CSS, and vanilla JavaScript in a single file.
