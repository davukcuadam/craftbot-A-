# craftbot-AI
local minecraft AI bot

CraftBot AI

An open-source artificial intelligence companion (bot) desktop application for Minecraft that runs entirely on the power of your own computer. No paid external APIs are used

Initial Startup Flow
Select one of the Noob / Normal / Pro levels → "Lock and Start" (this decision is permanent and cannot be changed again).
The application downloads the selected Ollama model (actual progress percentage is displayed; it may take a few minutes the first time).
On the control panel, enter the server IP/port, bot name, language, theme color, and custom behavior note, then click "Connect and Join the Game".

Model stages (approximate dimensions are based on Ollama's own data):

Stage Model Size
Noob llama3.2:1b ~1.3 GB
Normal llama3.2:3b ~2 GB
Pro llama3.1:8b ~4.9 GB (~up to 6 GB)
 Honest notes (important!)
The voice-to-text (TTS) feature uses msedge-tts and requires internet as the only exception (free, no key required). When closed, the application operates completely offline. If TTS fails, the application does not crash; it silently continues in text mode.
Small models (Noobs) may sometimes struggle to fully grasp the action format (###ACTIONS###) — this is a natural limitation of small models and not an error. The Pro tier is much more consistent.
While the code was being developed, it could not be tested against a real Minecraft server (there is no network access/client in this environment); it was written adhering to the mineflayer/Electron APIs. If there is a small problem on the first attempt (e.g. share the error message (an event name, a version incompatibility), we will quickly fix it together.
If a package version cannot be found during npm install, package.You can delete the version number of that package in the JSON file and install the latest version with the command `npm install <package-name>`.
 Contributors & Licenses
Electron (MIT) — desktop application framework
Mineflayer & mineflayer-pathfinder (MIT) — Minecraft bot engine
minecraft-data (MIT) — block/item database
Ollama (MIT) - local artificial intelligence engine/launcher
msedge-tts (MIT) — optional voice reading
Minotar (https://minotar.net ) - public, keyless Minecraft skin visualization service (used only for shooting images, any skin files are not distributed with this project)

CraftBot AI's own code is shared under the MIT license (see  LICENSE). All libraries used have permissive open source licenses.
