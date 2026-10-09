```text
    █████████████████████████████████████████████████████
    ███    ███     ██     ██ ███ ██     ██     ██ ███ ███
    ███ ███ ██ ████████ ████ ███ ██ ██████ ██████  ██ ███
    ███    ███    █████ ████ █ █ ██    ███    ███ █ █ ███
    ███ ███ ██ ████████ ████  █  ██ ██████ ██████ ██  ███
    ███    ███     ████ ████ ███ ██     ██     ██ ███ ███
    █████████████████████████████████████████████████████

      T H E  ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━  ( * )

  ██████████████████████████████████████████████
  ███    ███ ███████   ████    ██ ███ ███    ███
  ███ ███ ██ ██████ ███ ██ ██████ ██ ███ ███████
  ███    ███ ██████ ███ ██ ██████   █████   ████
  ███ ███ ██ ██████ ███ ██ ██████ ██ ███████ ███
  ███    ███     ███   ████    ██ ███ ██    ████
  ██████████████████████████████████████████████
        ◥████
          ◥██
            ◥
```

**The student newsletter at APU, Kuala Lumpur.**
News, food, scores, arguments and dates from between one block and the next.

```text
  ■ CITY GUIDE   ■ CAMPUS NEWS   ■ SPORTS & ACTIVITIES   ■ DEBATES & OPINIONS   ■ EVENTS & TIMELINE
```

---

## What this is

The website for Between the Blocks, issue 1. It is one HTML file and two images.
There is no framework, no build step and nothing to install.

## The page, drawn out

```text
┌──────────────────────────────────────────────────────────────────┐
│ [logo]            Friday 9 October 2026 · Issue 1    [SUBSCRIBE] │
├──────────────────────────────────────────────────────────────────┤
│ CITY GUIDE  CAMPUS NEWS  SPORTS  DEBATES  EVENTS        (sticky) │
├──────────────────────────────────────────────────────────────────┤
│ ██████████████████████████████████████████  ┌─────────────────┐  │
│ ██  WHAT'S GOING ON                     ██  │ DEBATES story   │  │
│ ██  BETWEEN THE BLOCKS?                 ██  ├─────────────────┤  │
│ ██  [READ THE FIRST ISSUE]              ██  │ CAMPUS NEWS     │  │
│ ██████████████████████████████████████████  └─────────────────┘  │
├──────────────────────────────────────────────────────────────────┤
│ ■ CAMPUS NEWS                                                    │
│ ┌ Where to get help at APU ───┐  ┌ Societies welcome intake ───┐ │
│ └─────────────────────────────┘  └─────────────────────────────┘ │
├─────────────────────────────────┬────────────────────────────────┤
│ ■ CITY GUIDE                    │ ■ DEBATES & OPINIONS           │
├─────────────────────────────────┼────────────────────────────────┤
│ ■ SPORTS & ACTIVITIES (table)   │ ■ EVENTS & TIMELINE (dates)    │
├─────────────────────────────────┴────────────────────────────────┤
│ ██  WRITE FOR ONE OF OUR FIVE DEPARTMENTS                     ██ │
├──────────────────────────────────────────────────────────────────┤
│ Get every issue by email            [ student email ][SUBSCRIBE] │
└──────────────────────────────────────────────────────────────────┘
```

Clicking a story swaps the homepage for the full article. Both live in the same file.

## In issue 1

| Department | Story |
| :-- | :-- |
| Debates & Opinions | Community or Just a Group Chat? |
| Campus News | Where to get help at APU |
| Campus News | Societies welcome the September intake |

City Guide and Sports & Activities still show sample entries, labelled as such on the page.

## What's in the box

```text
between-the-blocks/
├── index.html ········ homepage, three articles, styles and script
├── assets/
│   ├── logo.jpg ······ the club logo
│   └── wellbeing.jpg · Centre for Psychology and Well-Being, Block E
└── README.md ········· you are here
```

## Run it

Open `index.html` in a browser. Or serve the folder:

```bash
npx serve .
```

## Put it online

```text
  your laptop ──── git push ────▶ GitHub ──── auto deploy ────▶ Vercel
```

1. Push this folder to a GitHub repository.
2. On vercel.com choose **Add New > Project** and import the repository.
3. Leave the framework preset as **Other** and the build command empty.
4. Deploy. Every later push to `main` goes live on its own.

## Add a story

1. Copy one `<article class="story" id="story-...">` block near the bottom of `index.html`.
2. Give it a new id that starts with `story-`, for example `story-futsal-final`.
3. Set its department with one class: `d-city`, `d-news`, `d-sport`, `d-debate` or `d-events`.
4. Link to it from the homepage with `href="#story-futsal-final"`.

## Colours

Each department owns one colour. They are variables at the top of the `<style>` block.

| Use | Variable | Hex |
| :-- | :-- | :-- |
| Masthead and hero | `--navy` | `#0f1053` |
| City Guide | `--city` | `#e0460b` |
| Campus News | `--news` | `#d91a2a` |
| Sports & Activities | `--sport` | `#087f4b` |
| Debates & Opinions | `--debate` | `#d416a0` |
| Events & Timeline | `--events` | `#2447f5` |

## Not finished yet

- The subscribe form checks the email address but does not save it.
- Section links such as "All guides" have no archive pages behind them.

```text
  ██████████████████████████████████████████████████████████████
  ██  Written and edited by students of APU, Kuala Lumpur.    ██
  ██████████████████████████████████████████████████████████████
        ◥████
          ◥██
```
