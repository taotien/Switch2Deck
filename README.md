# Switch2Deck

Tutorial and scripts setting up Nintendo Switch homebrew and emulation using
just the Steam Deck. I'll also include some tips and links.

---

## What you need

- Nintendo Switch, homebrew-able
- RCM-jig
- Steam Deck (RIP Q2+); but also this will apply to any if not all Linux
  machines
- USB-C **data** cable
- Enough storage space
- (optional) USB-C hub for desktop-mode convenience / or setup KDE Connect
  (see Tips)

## Step 1 - Steam Deck

I recommend going to the tips section to make interacting with your Deck's
desktop mode easier, as you might want a mouse and keyboard.

Downloads:

- [JTegraNX.jar](https://github.com/dylwedma11748/JTegraNX/releases/latest).
- [Adoptium JRE 17](https://adoptium.net/temurin/releases) or other JRE should
  be ok, this one can also be used and is recommended for PolyMC, a great
  Minecraft launcher.
- Emudeck
- payloads

Put all the downloads in an easy to access folder.

### Running Java & JTegraNX

To run the payload injector, open a terminal (default on Deck is Konsole) and
navigate to where your downloads are. Execute java on the JTegraNX.jar file as
root. The java binary path should be [your java download]/bin/java. You can
press TAB to automatically fill in longer parts of file and folder names.

```bash
cd Switch2Deck
sudo ./jdk-17.0.3+7-jre/bin/java -jar JTegraNX.jar
```

## Step 2 - Homebrew

## Step 3 - Backups

## Step 4 - Emulation

### Save files

Save files are stored in a different location that what the yuzu tutorials say,
because Emudeck (and all applications you'll install with the Discover store)
installs the Flatpak version of your programs. All of their files will be under
their own folders in `/home/deck/.var/app/`.

After adding a game, find its ID number, then locate the save folder with the
same ID under `~/.var/app/org.yuzu_emu.yuzu/data/yuzu/nand/user/save/[game ID]`.

---

## Tips

### KDE Connect

KDE Connect is a companion app for the KDE desktop environment which the Deck
uses. It has many features, one of which is the remote input. Depending on your
connection there may a bit of latency, but it's a good alternative if you don't
have a USB-C hub or haven't set up the Steam desktop controller bindings for
desktop use.

Follow [this great PSA by u/DevOpsIsAMindset](https://www.reddit.com/r/SteamDeck/comments/tb7h13/kde_connect_is_available_on_the_steam_deck/).

Once you have it set up on the Deck, get the app (all popular platforms
available) for your computer or phone set up as well, and pair the 2 devices.

### Syncthing

## References & Thanks

- [yuzu](https://yuzu-emu.org/help/quickstart)
- Reddit u/DevOpsIsAMindset
- Reddit u/turdfergusn

Thank you again to u/turdfergusn for encouraging me to make this!

<!--  TODO

- license

-->
