Profile card (static) with a Dynamic Island clock.

Files added:
- `index.html` — main HTML (clock + island + keyboard support)
- `style.css` — styling and responsive behavior
- `avatar.svg` — placeholder avatar (replace with your `avatar.png` if preferred)
- `roblox-icon.svg` — placeholder Roblox icon (replace as needed)

How to run (Windows PowerShell):

Open the file directly (double-click) or run a simple static server:

```powershell
# from the project folder (c:\code for discord)
Start-Process .\index.html
# or, to serve over localhost if you want to test fetches/CSP/etc:
python -m http.server 8000; Start-Process http://localhost:8000/index.html
```

Notes:
- Replace `avatar.svg` and `roblox-icon.svg` with your PNGs if you prefer. Update the `img` srcs in `index.html` accordingly.
- The island supports hover expansion on larger screens and tap/keyboard toggle on mobile/accessibility devices.
- If you want the time in a different timezone, change `timeZone` in the script inside `index.html`.
