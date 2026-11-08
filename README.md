# azazazbrainxvanyi
A local music player that lives on your desktop.

Please use Windows 10 or 11. Windows 7 hasn't been adapted for yet—sorry, Win7!

## Getting Started

Extract the entire folder, then open either **启动播放器.cmd** or **启动播放器.vbs**.

The floating window appears when the player starts, and the app also runs in the system tray. That's the small icon area on the right side of the Windows taskbar, sometimes tucked away behind the upward arrow. Right-click the SimpleM icon for a few options, including starting with Windows, showing the track list, and exiting the app.

**On its first run, the player will try to enable startup with Windows. If you don't want that, just uncheck it in the tray menu.**

The first time you launch it, click the **folder icon** at the top and choose a music folder. It is a local music player, after all. You can create an empty folder and gradually add songs, but if you already have a folder full of MP3s, even better!

MP3, WAV, WMA, M4A, AAC, and FLAC are supported. Whether a particular file plays depends on its encoding and Windows' media support.

Nested folders work too. Create a few subfolders inside your main folder to organize your favorite songs. When you select the main folder, its subfolders are loaded as well.

Finally, double-click a song and enjoy the music. The player remembers your music folder next time, but won't start playing automatically.

## The Window

When the window isn't pinned, clicking another app automatically hides it. The music keeps playing; press **Alt + S** to bring it back.

If you want it to stay on your desktop, click the **pin** in the upper-left corner. Pinning keeps it on top; click again to return to automatic hiding.

Drag the empty area at the top to move the window somewhere convenient.

The × in the upper-right corner only hides the window. To close the player completely, right-click its tray icon and choose **Exit**. If you can't find the window, double-click the tray icon or run the launcher again to bring it back. This won't open a second player.

## Keyboard Shortcuts

- **Alt + S**: Show the player; press again to hide it. Works while you're in other apps too.
- **Space**: Play / pause.
- **↑ / ↓**: Move the selection in the track list.
- **Enter**: Play the selected track, or expand/collapse the selected folder heading.
- **End**: Jump down to the next folder heading.
- **Esc**: Clear the search while you're in the search box.

Except for Alt + S, these shortcuts work inside the player. While you're typing in the search box, Space and the arrow keys keep their normal editing behavior, so you won't accidentally trigger playback controls halfway through typing.

If another app has already claimed Alt + S, you can still double-click the tray icon to show the player.

## Mouse Controls

**Find a song:** Type a title, artist, or album into the search box to see results immediately. Artist and album information comes from the music file's tags; if those are missing, search by title instead. Searching only filters the displayed list—it doesn't change the playback scope to the search results.

**Skip tracks and seek:** Click Previous or Next to change tracks. Click or drag the progress bar to jump to the part you want to hear.

**Reorder songs:** Clear the search, then drag a song up or down and drop it at the insertion line. You can only reorder tracks within the same folder. This doesn't move the files on disk.

**Add new songs:** Choose your music folder first, then drag audio files into the track list. All six formats mentioned above work, and you can mix them in a single drop! Drop near a track to choose an insertion position, or onto a folder heading to import into that folder.

Importing makes a copy, so **the original file stays where it was**. If a filename already exists, the new copy gets a number rather than overwriting the existing song. Other formats and folders are skipped, and files aren't converted to another format.

**Delete songs:** Right-click a track to move it to the Recycle Bin, or select it in the list and press Delete. But is it really worth it? This moves the actual file on disk to the Recycle Bin, rather than merely removing it from the list, and deleting a single track won't ask for confirmation again. If you delete something by mistake, recover it from the Recycle Bin.

You can also right-click to delete a subfolder. This asks for confirmation first, then moves the folder and everything inside it to the Recycle Bin. The library's root folder can't be deleted this way.

**Playback mode:** This is the fourth button from the left in the playback controls. Left-click to cycle through Repeat all, Repeat one, and Shuffle. Right-click to switch the scope between **All tracks** and **Current folder**. The current folder is the one containing the playing track; its subfolders aren't included.

**Volume:** The speaker icon changes with the volume: one, two, or three sound waves for low, medium, or high volume, and a cross when muted. Hover over the speaker and scroll to adjust the volume. You can also click it to open the volume slider, then drag or scroll. Middle-click the speaker to mute, and middle-click again to restore the volume.

Not sure what an icon does? Hover over it to read its tooltip.

## A Few More Things

- Click a folder heading in the list to expand or collapse it.
- The horizontal-lines button to the right of the search box switches between standard and compact views. Right-click it to expand all folders, collapse all folders, or locate the current track.
- Double-click the large song title at the top to find the currently playing track. This also clears the search and expands the relevant folders.
- Want a smaller window? Uncheck **Show track list** in the tray menu, and turn it back on whenever you need it.
- Songs added to your music folder appear automatically. If they haven't shown up yet, try the refresh button at the top. Also check whether a search filter is still active or the folder is collapsed.
- To find the file you're listening to, right-click the tray icon and choose **Show current track in File Explorer**.

The player remembers settings such as volume, playback mode, window position, pin status, and track order. Exit normally through the tray menu when you're done so it can save everything properly.

If you want to move the app, exit it first, move the entire program folder, then launch it from the new location.

## If Something Goes Wrong

If it won't open, first check whether it's already in the tray. Then make sure the app has been fully extracted and all its files are together. It needs Windows' scripting components, so it may not start if scripts are disabled on your computer.

If a song won't play, try another one that you know works. Supporting a file extension doesn't guarantee that every encoding will play.

For troubleshooting, paste this into the File Explorer address bar:

```text
%LOCALAPPDATA%\SimpleDesktopMusic
```

This is where the settings are stored. `player.log` may contain details about saving, scanning, or importing problems. Normally, you don't need to touch any of these files.

---

The app's features were built with gpt6-astra-light! (Thanks to OpenAI for the help.)

I renewed Plus this morning and spent most of the afternoon on this. I'd say it was worth it.

I'd never even seen a .ps1 file before! GPT really knows its stuff!

That's the end of readme.md. (I was originally going to write it by hand, and had even finished a 764-character version, but Skynet's awakening is already irreversible 😭. If anything here makes absolutely no sense, GPT definitely wrote that bit.)
