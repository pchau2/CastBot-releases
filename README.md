# CastBot

Hands-free voice commands for your Twitch stream. Say a trigger word, then a
command, and CastBot clips, moderates chat, switches OBS scenes or starts an ad
break — without you leaving your game.

**[⬇ Download the latest version](https://github.com/pchau2/CastBot-releases/releases/latest)**

Windows 10 or 11, 64-bit. This repo holds the downloads only.

---

## Setting it up

**1. Run the installer.**
Windows will say the publisher is unknown — click **More info → Run anyway**.
CastBot isn't code-signed yet (certificates are expensive for a small
project), so that warning shows on every unsigned app, not just this one.

It installs for you alone, so there's no admin prompt.

**2. Get a product key.**
Join the [CastBot Discord](https://discord.gg/SXKXbytRne) and run **`/getkey`**
in any channel. The bot DMs you a key. Paste it into CastBot when it asks.

**3. Sign in to Twitch.**
**Settings → Connections → Log in with Twitch.** A code appears, Twitch opens
in your browser, you type the code in. There's no developer account to create
and nothing to copy into a config file.

**4. Press START BOT**, go live, and say your trigger word.

---

## Using it

Say your trigger word, wait for the listening chip, then say a command:

| Say | What happens |
|---|---|
| clip that | Clips the last 30s and posts the link in chat |
| time out | Lists recent chatters — say a name or number to time them out |
| change scene | Lists your OBS scenes — say one to switch |
| run ads | Starts an ad break (affiliate and partner channels) |

Changed your mind mid-command? Say **cancel**.

Missed you? Press **Ctrl+Shift+C**, or click **CLIP NOW**. Every press also
teaches CastBot what your voice sounds like, so it misses you less often.

Commands only run while you're connected to Twitch **and** live. The pill in
the top-left corner tells you where you stand.

---

## Good to know

**OBS is optional.** You only need it for scene switching and alert sounds.
Enable its WebSocket server under **Tools → WebSocket Server Settings**.

**Gaming in exclusive fullscreen?** Any always-on-top window makes Windows drop
a fullscreen game to the desktop. CastBot never steals focus, but its listening
chip is still an on-top window — turn it off under **Settings → General →
Gameplay** and you'll get sound and voice confirmation instead. Borderless
windowed is unaffected.

**Your settings live in `%LOCALAPPDATA%\CastBot`.** Config, logs and anything
CastBot learns about your voice stay there, so updating the app doesn't lose
them. Uninstalling asks before deleting them.

**Updating:** download the new installer and run it. It replaces the old
version in place.

---

## Something wrong?

Ask in the [Discord](https://discord.gg/SXKXbytRne). If CastBot is misbehaving,
**Settings → Logs** has what it was doing at the time.
