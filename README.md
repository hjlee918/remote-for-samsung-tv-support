# Remote for Samsung TV

Support page for **Remote for Samsung TV**, a Stream Deck plugin that controls Samsung smart TVs (Tizen, 2016 and later, including Neo QLED, QLED, OLED and The Frame): remote keys, power, volume, apps, inputs and Stream Deck + dials. Get it on the [Elgato Marketplace](https://marketplace.elgato.com/).

## Get help

- **Found a bug?** [Open a bug report](../../issues/new?template=bug_report.yml).
- **Have an idea?** [Suggest a feature](../../issues/new?template=feature_request.yml).

Please search [existing issues](../../issues) first.

## Requirements

- Windows 10 or later, or macOS 12 or later.
- Stream Deck 7.1 or later.
- A Samsung smart TV (Tizen, 2016 or later) on the same network as the computer.

## Setup

1. Turn the TV on.
2. Drag any **Remote for Samsung TV** action onto a key, for example **Remote Button**.
3. In its settings, click **Search**, choose your TV, and click **Pair**. If nothing is found, type the TV's IP address and click **Search** again. The IP address is in the TV's settings under **General → Network → Network Status → IP Settings**; the exact menu names vary by model.
4. **Allow** "Stream Deck" when the TV asks, using the TV's remote.
5. Choose what the key does. Add more keys for other actions; they all share the pairing.

**To turn the TV on from Stream Deck**, turn on **Power On with Mobile** in the TV's settings: **General → External Device Manager → Device Connection Manager** on recent models, or **General → Network → Expert Settings** on older ones.

**More than one TV?** Click **Add TV** in any key's settings and pair it the same way. Each key or dial then has a **Control** menu for choosing its TV; the first TV paired is the default.

## The actions

| Action | What it does |
|---|---|
| **Remote Button** | Any key of the TV's remote: arrows, OK, Back, Home, Exit, Settings, Tools, Info, Source, playback, channels, numbers, color buttons, subtitles, the picture mode key and more. Can also type text into a search field, open a web page, or go to a channel by number. Optional **Hold** and **Double press** commands. |
| **Power** | Power on / off, power on, power off, or the power key (Art Mode on The Frame). A green dot shows when the TV is on. |
| **Volume** | Volume up or down (hold to repeat), mute, or a set level. The key shows the TV's volume when the TV reports it. |
| **Open App** | Opens an app from the TV's list, or any other installed app by its app ID (choose **Other app (by its ID)…**), optionally straight to a YouTube video. The key shows the app's icon, with a bar while it's on screen. |
| **Input** | Switches to HDMI 1–4, the next input, or opens the TV's Source list. |
| **TV Dial** (Stream Deck +) | Volume, channels, navigation, playback, apps or inputs. The touch strip shows the TV's name and volume, or the app or input being chosen. |

## Troubleshooting

- **Search finds nothing:** make sure the TV is on and on the same network as the computer, then enter its IP address and search again. Some routers and mesh Wi-Fi systems block automatic discovery.
- **No request appears on the TV, or pairing fails:** turn the TV on fully (not in standby) and try **Pair** again. If you chose **Deny** by mistake, open the TV's **General → External Device Manager → Device Connection Manager → Device List**, remove "Stream Deck" (or set it to Allow), and pair again.
- **Keys say "TV is off" while the TV is on:** the TV's IP address may have changed. The plugin looks for the TV again on its own; if that doesn't work, reserve a fixed IP address for the TV in your router, then click **Forget** and pair again.
- **Power on doesn't work:** turn on **Power On with Mobile** in the TV's settings (see Setup). Some TVs can only be woken over a wired connection, or for a while after they were turned off.
- **The volume level doesn't show:** the TV reports its volume while its own speakers are in use. With a soundbar or receiver, the volume keys still work but the level isn't known.
- **An app isn't in the Open App list:** choose **Other app (by its ID)…** and enter the app's ID. The app must be installed on the TV. If the key shows the ID instead of the app's name, the TV doesn't list that ID; check it.
- **HDMI 1–4 keys don't switch input:** not every model has direct HDMI keys. Use **Source** or **Next input** instead.
- **The Frame:** **Power off** turns the TV off fully; the **Power key** switches Art Mode on and off.
- **Windows asks whether to allow network access:** choose **Allow** so the plugin can find and control your TV on your local network.

When reporting a bug, attach the latest log from:

- **macOS:** `~/Library/Application Support/com.elgato.StreamDeck/Plugins/com.johnlee.samsungtvremote.sdPlugin/logs/`
- **Windows:** `%APPDATA%\Elgato\StreamDeck\Plugins\com.johnlee.samsungtvremote.sdPlugin\logs\`

## Privacy

The plugin collects no personal data and connects only to your TV on your local network. See the [Privacy Policy](PRIVACY.md).

## Open-source software

The plugin includes open-source software; see `THIRD_PARTY_NOTICES.txt` inside the plugin.

---

Samsung, Tizen, SmartThings, Neo QLED and The Frame are trademarks of Samsung Electronics Co., Ltd. This plugin is not affiliated with, sponsored by, or endorsed by Samsung Electronics Co., Ltd.
