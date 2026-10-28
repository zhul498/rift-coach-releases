# Rift Coach

A free League of Legends coach for ranked. It reads the game the way Riot allows and shows you, live:

- **Champ select:** both teams, which lane each enemy pick is probably playing (updated with every pick), who your lane opponent will likely be, and the runes and first items Master+ players use in that matchup.
- **In game:** a build tree that starts from the items you already own and shows what Master+ players build next, what you can buy with your gold right now, the biggest enemy threat, and both teams' damage and scaling.

It works best on a second monitor. With one monitor, a small overlay shows the essentials over the game.

> **Beta.** Expect rough edges, and please report anything odd (see [Reporting a problem](#reporting-a-problem)).

## Install (Windows)

1. Go to the [latest release](../../releases/latest) and download **RiftCoach-…-windows.zip**. (There's also a single-file **RiftCoach-…-portable.exe** if you prefer; it starts a little slower.)
2. Right-click the zip, choose **Extract All…**, and pick a folder you'll keep, like `Documents\Rift Coach`.
3. Open the folder and double-click **Rift Coach.exe**.
4. Windows will probably show **"Windows protected your PC."** Rift Coach is a small free app that isn't code-signed yet (signing costs money), so Windows doesn't recognize it. Click **More info**, then **Run anyway**. You only have to do this once.

That's it. You don't need Node, git, an account, or an API key. Master+ stats download and update on their own.

**Optional:** right-click **Rift Coach.exe**, then **Show more options**, **Send to**, **Desktop (create shortcut)**.

## Use it

Open Rift Coach before or after League. It connects on its own and comes alive when you enter ranked champ select. It sits idle in other queues; you can change that in Settings.

**Two monitors:** the dashboard opens on the monitor League isn't on and fills it. Vertical monitors are supported.

**One monitor:** the dashboard opens as a normal window for champ select. When the game starts it steps aside and a small overlay appears on the right side of the screen, showing your next item, the biggest threat, and your matchup. The overlay never takes your clicks.

| Keys | What it does |
| --- | --- |
| Ctrl+Shift+D | One monitor: show the full dashboard over the game (press again to go back). Two monitors: bring the dashboard forward. |
| Ctrl+Shift+L | Hide or show the overlay (or the dashboard) |

**Settings** (top right of the dashboard): one or two monitors, which monitor, overlay on or off and where, ranked only, and text size. Changes apply right away.

## Is this allowed?

Rift Coach only reads Riot's official local APIs, the same ones Riot provides for apps like this. It doesn't read game memory, touch game files, or automate anything, and it doesn't track enemy cooldowns or timers. Everything it shows in game is information you could see yourself on the Tab scoreboard. You can't be banned for using it.

## Updates

- **Stats** update automatically, usually a few days into each patch.
- **The app:** when there's a new version, an "Update available" button appears at the top of the dashboard. Download the new zip and extract it over the old folder (your settings are kept).

## Reporting a problem

Open **Settings** and click **Copy diagnostics**, then paste the result along with what happened when you report it. It includes the recent log and your monitor setup, not your account or your files. **Open log folder** shows the full log.

**Common fixes:**

| Problem | Fix |
| --- | --- |
| Nothing happens in champ select | Make sure it's a ranked game, or turn off "Only run in ranked games" in Settings. |
| The overlay doesn't show in game | Set League to **Borderless** (Settings → Video → Window Mode). Exclusive fullscreen hides everything else. Also check Settings → In-game overlay. |
| The dashboard opens on the wrong monitor | Settings → Dashboard monitor. |
| "Couldn't reach Riot's patch data" | Check your internet connection and restart Rift Coach. |
| Antivirus blocks it | Some antivirus apps are wary of new unsigned apps. Add an exception for the Rift Coach folder. |

## Uninstall

Delete the Rift Coach folder. To remove its settings and saved stats too, delete `%APPDATA%\rift-coach`.

---

Rift Coach isn't endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing Riot Games properties. Riot Games and all associated properties are trademarks or registered trademarks of Riot Games, Inc.
