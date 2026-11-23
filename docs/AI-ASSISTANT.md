# Anthem + an AI assistant — one-page guide

Ask Claude (or any MCP-capable assistant) to build your Sunday: songs, announcement graphics, the service order, even driving the screens. Everything runs on your Mac; Anthem talks to the assistant locally, nothing is uploaded by Anthem.

## 1. Set up (once, ~2 minutes)

1. Install **Anthem** on your Mac and open it once. (Mac only for now.)
2. **Settings ▸ Remote control → ON** (the assistant uses the same local connection as the phone remote).
3. Tell your assistant where the connector is:
   - **Claude Code:** `claude mcp add anthem /Applications/Anthem.app/Contents/MacOS/anthem-mcp`
   - **Claude Desktop:** add to `~/Library/Application Support/Claude/claude_desktop_config.json`, then restart Claude:
     ```json
     { "mcpServers": { "anthem": { "command": "/Applications/Anthem.app/Contents/MacOS/anthem-mcp" } } }
     ```
4. Keep Anthem **running** while you chat. Test it: *"Look at my Anthem overview."*

## 2. What to ask for

| You say | It does |
|---|---|
| "What's in this Sunday's service?" | Reads the plan, songs, decks, themes, what's on screen |
| "Add *Way Maker* and *10,000 Reasons* with chords" | Finds them on Ultimate Guitar and imports them (no lyrics typed out) |
| "Add a song called … with these lyrics" | Creates it; edits keep what you didn't mention |
| "Make a slide deck for the sermon points" | Title / point / text / verse / picture slides |
| "Design an announcement graphic for the youth retreat on 5 Dec" | Draws a 1920×1080 slide, shows you a preview, adds it to a deck |
| "Set up Sunday 24 Nov: countdown 9:55, worship, scripture Psalm 23, sermon, offering" | Replaces the service order for that date |
| "Show Psalm 23 / next slide / black screen / alert 'Parking full'" | Drives the live screens |
| "What does the screen show right now?" | Sends it a picture |

## 3. Good habits

- **Check before Sunday.** Ask it to *show you* each graphic and the finished plan; fix by talking ("bigger date, darker background").
- **Safe edits.** Anthem backs up songs, decks and plans before an AI change (at most every 10 minutes, in Application Support ▸ Anthem ▸ Backups).
- **Copyrighted lyrics.** Let it import published songs from Ultimate Guitar rather than writing them out from memory.
- **Live screens.** Driving the projector is real and immediate; leave "go live" to the operator unless you ask.

## 4. If it doesn't work

- *"Anthem settings not found"* → open Anthem once on this Mac.
- *Can't connect* → Anthem must be running with **Remote control ON**.
- Graphic looks cut off → say so; it redraws it.
- Still stuck → [open an issue](https://github.com/Rtnkr/anthem/issues/new/choose).

