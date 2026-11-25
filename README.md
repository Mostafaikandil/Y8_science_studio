# Y8 Science Studio

A free, single-page science practice app for **Year 8 (ages 12–13)** students following the English Key Stage 3 curriculum. It covers cells and respiration and electricity and magnetism, with labelled diagrams, typed answers, worked explanations and progress tracking for a parent.

## Play

Open the live page in any modern browser:

`https://mostafaikandil.github.io/Y8_science_studio/`

On a phone or tablet, add it to the Home screen so it opens like an app (Chrome: ⋮ menu → *Add to Home screen*; Safari: Share → *Add to Home Screen*).

## Topics

Eight topic modules, each with three tiers.

| # | Topic | Includes |
|---|---|---|
| 1 | Using a microscope | Parts of a light microscope, technique, magnification calculations |
| 2 | Cells | Animal and plant cells, what each part does |
| 3 | Cell organisation | Cells, tissues, organs, organ systems, organisms |
| 4 | Respiration | Aerobic and anaerobic respiration, word equation, where it happens |
| 5 | Circuits and symbols | Circuit components, complete circuits |
| 6 | Current and potential difference | Series and parallel circuits, ammeters, voltmeters, calculations |
| 7 | Static electricity | Charge, forces between charges, sparks |
| 8 | Magnets and electromagnets | Poles, magnetic fields, building and strengthening electromagnets |

## How the tiers work

| Tier | What the student does |
|---|---|
| **Warm-up** | Multiple choice, with the diagram part highlighted |
| **Practice** | Types the answer. Labelling questions show a hint such as `c _ _ _  w _ _ _` |
| **Challenge** | Types the answer with no hint, plus "apply and explain" questions |

Scoring 80% or more unlocks the next tier.

## Features

- **Label the diagram:** nine built-in diagrams (microscope, animal cell, plant cell, levels of organisation, circuit symbols, series and parallel circuits, bar magnet, electromagnet). Every part is numbered and the one being asked about is highlighted.
- **Explanations:** after each answer the app shows what the part or idea is for.
- **Flexible answer checking:** accepts common alternative names, and flags small spelling slips on long scientific terms.
- **Calculations with changing numbers:** microscope magnification and series and parallel circuit problems.
- **Mixed review** (10 questions across topics) and **Quick check** (16 questions, 2 per topic) with a result for each topic.
- **Resume where you stopped:** progress is saved after every question, so a level can be paused with the Home button and continued later.
- **Working pad:** a drawing area for a stylus or finger.
- **Sound:** optional sound effects and quiet background music, each with its own on/off button.
- **Parent area** (PIN protected): accuracy by topic, best scores, recent mistakes, and a backup and restore code.
- Light and dark mode follow the device setting.

## Privacy

- No account, no tracking and no data sent to any server.
- The student's name, progress, scores and mistakes are stored **only in the browser on the device being used** (local storage).
- Clearing the browser's site data on that device deletes the progress. Use the backup code in the Parent area to keep a copy.
- Other people who open the link get their own separate, empty copy.
- The parent PIN is stored in the same browser storage. It stops casual access and is not a security feature.
- If several apps are hosted under the same `github.io` address they share the browser's storage area. This app uses its own storage key, so it does not mix with them.

## Technical notes

- One `index.html` file with plain HTML, CSS and JavaScript. No frameworks, no build step and no external libraries or images.
- Diagrams are inline SVG drawings created for this project.
- Sound is generated in the browser with the Web Audio API, so there are no audio files.
- To run it locally, open `index.html` in a browser, or serve the folder with `python3 -m http.server 8080` and visit `http://localhost:8080`.
- Questions come from a built-in question bank and small generator functions. Each question stores its own answer and explanation.

## Updating

Replace `index.html` in this repository and commit. GitHub Pages republishes within a couple of minutes. Saved progress is kept, as long as the storage key in the file is unchanged.

## Known limitations

- Some topics have a small question bank, so a round can be shorter than 10 questions and questions repeat sooner.
- Typed answers must match a listed term or alternative. An unlisted but correct wording may be marked wrong.
- Mistakes are listed for the parent but not yet grouped by type of error.

## Roadmap

- Larger question banks for every topic
- More topics as the course progresses
- Spaced review that brings weaker topics back more often
- Optional offline installable app

## Curriculum and disclaimer

Topics follow the Key Stage 3 science programme of study for England. All questions and diagrams are original and written for this project. This is a practice tool and not an official assessment. It is not affiliated with or endorsed by any publisher or school.
