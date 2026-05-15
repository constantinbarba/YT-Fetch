# YT-Fetch

graph TD
    A[Chrome Extension UI] -->|Sends URL| B(Service Worker)
    B -->|Native Messaging| C{Windows Registry}
    C -->|Points to| D[Host Manifest JSON]
    D -->|Launches| E[Batch Launcher]
    E -->|Executes| F[Python Bridge]
    F -->|Calls| G[yt-dlp Engine]
    G -->|Downloads to| H[Local Disk]
