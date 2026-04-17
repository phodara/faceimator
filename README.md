# New Face Emulator

Open `index.html` in a browser to prototype a face and iterate on expression geometry.

Why this exists:

- The simulator uses normalized numeric parameters instead of image assets.
- The preview is drawn with simple geometric primitives so it stays close to what we can reproduce on the ESP32 with Adafruit GFX.
- The JSON export is meant to become the handoff format for porting expressions into `src/main.cpp`.

Current workflow:

1. Open `newface-emulator/index.html`.
2. Pick a preset expression.
3. Tweak the sliders until the face reads correctly.
4. Copy the JSON block.
5. Port the values into the firmware drawing code.
