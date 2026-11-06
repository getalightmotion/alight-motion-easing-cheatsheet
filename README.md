# Alight Motion Easing Cheat Sheet

An unofficial reference for choosing easing curves in mobile motion design and video edits, with a small interactive page that compares each curve with linear motion.

**[Try the live page](https://getalightmotion.github.io/alight-motion-easing-cheatsheet/):** pick a curve and press **Play**.

## Which curve to use

Choose from what the layer is doing, not from the shape of the graph.

| The layer is… | Curve | Starting length at 30 fps |
|---|---|---|
| Moving at a constant rate (loader, ticker) | Linear | Any |
| Leaving the frame or fading away | Ease-in | 8–12 frames |
| Entering and settling on screen | Ease-out | 12–18 frames |
| Travelling between two visible positions | Ease-in-out | 20–40 frames |
| Popping in and settling back | Overshoot | 12–16 frames |

These lengths are starting points based on common motion design practice. Adjust them for your edit.

## Reading a curve

- The horizontal axis is time between two keyframes.
- The vertical axis is how far through the change the layer is.
- A **steep** section means fast movement. A **flat** section means slow movement.

## Fix these before changing the curve

1. **Values:** do the two keyframes hold different values?
2. **Spacing:** is the move the right length? Closer keyframes make it faster.
3. **Curve:** only now adjust the speed inside that time.

## Files

| File | What it is |
|---|---|
| `index.html` | Interactive comparison page, with no dependencies or build step |
| `easing-curves.json` | The curves as data, with suggested uses and lengths |

The control points are CSS-style `cubic-bezier` values, included so you can reuse them on the web or in other tools. Alight Motion's Curve Editor is visual, so use the graph as a shape guide there.

## More guides

For step-by-step help, see the [keyframes and easing guide](https://getalightmotion.com/keyframes-easing/) on [GetAlightMotion](https://getalightmotion.com/).

## License and disclaimer

[MIT](LICENSE). This is an independent project and is not affiliated with, endorsed by, or sponsored by Alight Creative or Bending Spoons. "Alight Motion" is a trademark of its owner.
