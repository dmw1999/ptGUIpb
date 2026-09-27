# ptGUIpb — Python Tkinter GUI Prompt Builder

ptGUIpb is a desktop helper for people who want a Tkinter GUI but would rather describe it than write every widget by hand. You toggle the UI pieces you want, optionally pick what the app should *do*, and ptGUIpb builds a prompt you paste into an LLM.

It does **not** generate the GUI itself. It writes the request.

## Intended use

1. Check the layouts, widgets, dialogs, and behaviors you care about.
2. Optionally choose an example function (resize an image, convert txt→pdf, ping a host, and so on) and add a free-text extra request.
3. Copy or export the live prompt.
4. Paste it into Grok, ChatGPT, Claude, Gemini, Copilot, Perplexity, or a local tool such as LM Studio.
5. Use the generated Tkinter script as a starting point.

The live prompt always starts with:

"Make a Python Tkinter GUI with"

Each enabled feature is appended with a comma. Example functions and extra notes come after that list.

## What the builder includes

**Feature toggles** (tabs: Window, Menus, Widgets, Dialogs, Style)  
Window size and layout, menus and shortcuts, common widgets, file dialogs, theming, validation, logging, and similar requests people usually make for a first Tkinter tool.

**Example functions**  
Starter jobs so the LLM knows the app’s purpose, not only which widgets to draw.

**Live prompt**  
Updates as you toggle. Right-click to copy; **Copy Prompt** and **Export as .txt** are also available (`Ctrl+L` / `Ctrl+S`).

**Themes**  
Options → Theme: Light, Dark (black/white), Retro.

**Help**  
- How the builder works  
- Links to hosted LLMs and local options (LM Studio / Bionic)  
- “Help me pick the right LLM” — short notes on which models covered which kinds of Tkinter requests, plus a suggestion from your current toggles  
- Source answers can be saved to the Desktop and opened in Notepad  

## How to run it

Python 3.8+ with Tkinter (the standard python.org Windows install is enough). No extra packages to **run** the app.

```bash
python python_tkinter_gui_prompt_builder.py
```

## What it is not

- Not an IDE and not a visual form designer  
- Not a substitute for reading the script an LLM returns  
- Not limited to the bundled example functions — the extra-request box is there for anything else you want the generated GUI to do

Please Note: Code was generated via https://grok.com.

To find all releases visit: https://github.com/dmw1999/ptGUIpb/releases
