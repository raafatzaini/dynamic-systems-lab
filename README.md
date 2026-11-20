# Dynamic Systems Lab

**See why things grow, level off, collapse, or swing, and the structure that makes them do it.**

Dynamic Systems Lab is a free, interactive web lab about *patterns of change*. Pick a situation from your own field, watch it unfold as an illustrated story, and then look underneath: the feedback loops, stocks and flows, and delays that produce the pattern.

It is built for students and for faculty in any discipline, including those who have never studied system dynamics. It runs in 15 languages, on phones and computers.

> 🚧 **Work in progress.** This is an early version and feedback is very welcome. Use the **Help us improve** button at the bottom of the lab, or [open an issue](../../issues).

**▶ Try it:** https://raafatzaini.github.io/dynamic-systems-lab/

![Dynamic Systems Lab](og-image.png)

---

## What you can do

Each situation runs through five steps:

| Step | What you see |
| --- | --- |
| **Story** | An illustrated animation of the situation, with captions that say which feedback loop is in charge. Optional narration. |
| **Qualitative** | An animated causal loop diagram. Dots travel around each loop, faster on the loop in charge. The graph shows the shape of the change, with no numbers. |
| **Quantitative** | The same situation as stocks and flows: a tank-and-pipe picture, a graph with numbers, readouts and equations. |
| **Experiment** | Sketch a prediction, run it and compare, then change the settings and take on a challenge. |
| **Check** | A few quick questions with instant feedback. |

## Patterns of change

| Pattern | Structure underneath | Example |
| --- | --- | --- |
| Exponential growth | A reinforcing loop (R), with a weaker balancing loop (B) | Money in savings |
| Goal seeking | A balancing loop (B) | Water refilling a cistern |
| S-shaped growth | R in charge first, then B as the limit nears | Bacteria in a wound |
| Overshoot and collapse | R and B, with a slow-to-shrink capacity | A sheep herd and its pasture |
| Oscillation | B with a delay between two stocks | Room temperature around a setting |

## Areas

Everyday · Energy · Environment · Manufacturing · Biotechnology · Human body · Computing · Public interest technology · National security · Geography · Business · Economics · Psychology · Education · *Your own system* (custom labels)

## Languages

English, العربية, 中文, Español, Français, Deutsch, 日本語, 한국어, Italiano, Português, हिन्दी, Bahasa Indonesia, Türkçe, Русский, فارسی. Arabic and Persian display right to left.

The translations are drafts and still need review by native speakers. Corrections are welcome.

## Narration

Turn on the 🔈 button to hear the story captions. English uses recorded clips in a natural voice. Other languages use the device's own text-to-speech voice where one is available. The story waits for each sentence to finish.

## How it's built

- **No build step and no dependencies.** The whole lab is one HTML file with inline JavaScript and canvas drawing. Recorded English narration lives in `audio/`.
- **Simulations:** small stock-and-flow models stepped in the browser, one per pattern. All areas share the five models; only the labels, units and pictures change.
- **Accessibility:** keyboard shortcuts, screen-reader text for the canvases, reduced-motion support, and layouts tested down to 360 px wide.

## Run it locally

```bash
git clone https://github.com/raafatzaini/dynamic-systems-lab.git
cd dynamic-systems-lab
python3 -m http.server 8000
# open http://localhost:8000
```

Opening `index.html` directly from disk also works. Recorded narration needs a local server, though, because browsers block audio files loaded from `file://`, so the lab falls back to the device voice.

## Publish with GitHub Pages

1. Push these files to a public repository.
2. Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, then **main** and **/ (root)**.
3. The site appears at https://raafatzaini.github.io/dynamic-systems-lab/ within a minute or two.

## Feedback and contributions

This lab is a work in progress and will improve with your input:

- How are you using it, in a class, a workshop or on your own?
- Does a situation from your field make sense? What would you add or change?
- Anything confusing, broken, or hard to read on a phone?

Use the **Help us improve** button in the lab, or open an [issue](../../issues). Translation fixes and new situations are especially welcome.

## Credits

Conceived by **[Raafat Mahmoud Zaini, PhD](https://www.jmu.edu/cise/people/faculty/zaini-raafat.shtml)**, and built by Claude.
College of Integrated Science and Engineering · Integrated Science and Technology Program · James Madison University

Inspired in part by the TED-Ed lesson *Feedback loops: How nature gets its rhythms* by Anje-Margriet Neutel. English narration was generated with the open-source Kokoro text-to-speech model.

## License

Dynamic Systems Lab © 2026 by Raafat Mahmoud Zaini is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

[![CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
