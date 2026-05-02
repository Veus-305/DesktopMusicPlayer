How to run it on your Windows laptop
Step 1 — Install Python (free, once ever)
Go to this direct link and download: https://www.python.org/ftp/python/3.12.4/python-3.12.4-amd64.exe
Run it. On the very first screen, at the bottom, tick the box that says "Add Python to PATH" — this is the only thing that matters. Then click Install Now.
Step 2 — Extract the ZIP
Unzip VvynasVane_Windows.zip anywhere — Desktop is fine.
Step 3 — Double-click RUN.bat
That's it. On the very first run it will install 2 small packages automatically (takes ~30 seconds), then Vvynas Vane opens.
Every time after that, just double-click RUN.bat — it opens in about 3 seconds.

If Windows blocks RUN.bat
Right-click it → Run as administrator → or click "More info" → "Run anyway" if you see a blue "Windows protected your PC" popup.
Alternative: RUN_POWERSHELL.ps1
Right-click → Run with PowerShell — same result, sometimes more reliable on newer Windows versions.

What this version uses instead of npm/Node
It runs on Python + pywebview — Python opens a native Windows window, loads the HTML/CSS/JS UI inside it, and bridges file system access (scanning folders, reading metadata, saving playlists) through a Python backend. Same full UI, same 11 animated themes, same EQ, video player, and all features — just no npm required.
New Stop button (■) sits between Prev and Play. It pauses and resets the track to 0:00, flashes red briefly on click, and shows a toast. Keyboard shortcut: S.
Shuffle — the button now shows a small SHUF / ON label beneath the icon so you can always see the state at a glance, not just rely on the colour.
Repeat — cycles through three modes with a clear label under the icon:
OFF — plays through the queue once and stops
ALL — loops the whole queue continuously
ONE — loops the current track forever (the icon also shows a tiny "1")
Each mode change fires a toast notification so you know exactly what got toggled. All states persist across sessions via settings.
Keyboard shortcuts summary:
Key
Action
Space
Play / Pause
S
Stop (reset to 0:00)
Ctrl+S
Toggle Shuffle
Ctrl+←/→
Previous / Next


