# Training Plan

English · [Русский](README.ru.md)

A small workout planner that turns a four-week template into a checklist of sets.
Edit exercise maxima for a month; the app recalculates displayed weights and remembers completed sets on your device.
The useful idea is to keep the plan, calculated loads and next unfinished workout on one screen.

## Run

No build step or account is required.

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000`. For installation on a phone, serve the files over HTTPS with GitHub Pages and add the page to the home screen.
The interface is Russian. The public starter values and percentages are artificial examples.
They are not the author's training records or an individualized training prescription.

## Features and limits

- Four weeks, three workout days per week, editable exercise maxima and set completion.
- Estimated one-repetition maximum and rounded weights derived from the template.
- Saved progress in browser `localStorage`; no server or synchronization.
- Offline page after its assets have loaded successfully.

The exercise list and template are defined in `index.html`. There is no program editor. A text box supports JSON export and import.
The month selector extends through December 2026; after that it shows the current month.
Clearing site data loses saved progress. Keep your own backup before changing browsers or hosting origins.

## Origin

A standalone personal tool, generalized into a reusable example. No upstream GitHub project was identified in the source or history.

Maxima can be changed only for a future month.

## License

Own source: MIT.
