# MazeLab downloads

Install MazeLab using **[MazeLab Manager](https://github.com/DewangTara99/MazeLab-Releases/releases/latest)**. No GitHub or MazeLab sign-in is required to download or use the local application.

| Computer | Download |
|---|---|
| Windows x64 | [MazeLab Manager for Windows](https://github.com/DewangTara99/MazeLab-Releases/releases/latest/download/MazeLabManager-windows-amd64.zip) |
| Apple Silicon Mac | [MazeLab Manager for macOS](https://github.com/DewangTara99/MazeLab-Releases/releases/latest/download/MazeLabManager-darwin-arm64.tar.gz) |
| Linux x64 desktop | [MazeLab Manager for Linux](https://github.com/DewangTara99/MazeLab-Releases/releases/latest/download/MazeLabManager-linux-x86_64.tar.gz) |

Close any older MazeLab runtime first. Extract the manager archive and open `MazeLabManager.exe` on Windows, or run `./MazeLabManager` on macOS/Linux. Choose **Install / update**, then **Open MazeLab**. Each manager includes the matching application for offline installation; Python and video encoding are bundled. Other OS/CPU combinations are not currently supported.

In the application, use **Models & connections** to add a provider API connection or your own worker. In **Builder**, create a maze, select the worker, then **Save and run**. Watch progress in **Runs** and download finalized MP4 playback and results in **Artifacts**. Cloud models require your provider credentials and can incur charges; no model is called just by installing.

The manager verifies signed application updates while open and waits until MazeLab closes before applying them. Pin a version to prevent upgrades. **Uninstall** preserves experiments and credentials by default; deleting data requires explicit confirmation. On Windows, stop MazeLab with Ctrl+C in its console; on macOS/Linux, use **Stop MazeLab** in the manager. Stopping the app cancels active experiments.

If installation reports a startup-check failure, the previous installation and experiment data remain unchanged. Retry **Install / update**. First-attempt local checks intermittently failed during release testing and passed on retry; the cause is not yet confirmed.

The local application requires no account but must not be exposed to the LAN or internet. Source history, credentials and experiment data are not hosted in this download repository.

Initial manager binaries are not Authenticode-signed or Apple-notarized; OS publisher warnings may appear. Update signatures are separate. Do not disable OS security protections. Bundled update metadata expires after 90 days, so keep access to a fresh signed online feed or download a newer manager if an old offline installer expires.

`update-feed.json` is updater metadata, not an application to install. Releases prefixed `payloads-` are infrastructure for automatic updates and corresponding third-party source distribution; use the Manager downloads above. GitHub's automatic Source code archives contain this download page, not the application.
