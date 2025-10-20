# iTerm2 — Post-bootstrap steps

After bootstrapping the dotfiles, complete these steps to finish switching to iTerm2.

1. Import the color preset (manual)
- Open the .itermcolors file from the repo:
```bash
open packages/iterm2/.config/iterm2/Musings.itermcolors
```
- In iTerm2: Preferences → Profiles → Colors → Color Presets → Import... → select the imported preset → apply it.

2. Set font and size
- In iTerm2: Preferences → Profiles → Text → set Font to "FiraCode Nerd Font" and size (e.g. 14).
- Use Other Actions → Set as Default if you want this for all profiles.

3. (Recommended) Load preferences from the repo
- In iTerm2: Preferences → General → Preferences:
  - Check "Load preferences from a custom folder or URL".
  - Point it to: /Users/amit/workspace/dotfiles/packages/iterm2/.config/iterm2
- Save current settings to that folder (Preferences → General → Save settings to folder) or commit a prepared preferences file into that folder.

4. Verify
- Restart iTerm2, open a new window and confirm the color preset and font are applied.

Notes
- The .itermcolors file must be imported once manually; after that, enabling "Load preferences from a custom folder" will allow the repo to manage settings.
- If you want automated imports or a preconfigured plist, add/export com.googlecode.iterm2.plist into packages/iterm2/.config/iterm2 and enable repo prefs.
