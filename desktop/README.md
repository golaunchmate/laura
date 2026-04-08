# LaunchMate Desktop App

A Tauri-based desktop application for LaunchMate, providing native integrations and a seamless founder experience.

## Tech Stack

- **Frontend**: Next.js 15 (reuses LaunchMate web app)
- **Backend**: Tauri (Rust)
- **Styling**: Tailwind CSS with LaunchMate brand colors

## Features

- Native desktop notifications
- System tray integration
- Offline mode support
- Telegram bot integration
- AI mentor chat
- Dashboard with founder metrics

## Development

```bash
# Install dependencies
npm install

# Run in development mode
npm run tauri dev

# Build for production
npm run tauri build
```

## Project Structure

```
desktop/
├── src-tauri/           # Tauri backend (Rust)
│   ├── src/
│   │   └── main.rs      # Main entry point
│   ├── Cargo.toml       # Rust dependencies
│   └── tauri.conf.json  # Tauri configuration
├── src/                 # Frontend (Next.js)
│   └── app/
├── package.json
└── README.md
```

## Configuration

The app uses LaunchMate's brand colors:
- Navy Dark: #14234a
- Navy Medium: #233d7e
- Blue Primary: #5473c6
- LaunchMate Blue: #263051

## Integration with LaunchMate

This desktop app wraps the existing LaunchMate web application and adds:
1. Native window controls
2. System tray for quick access
3. Push notifications for mentor messages
4. Offline storage for local data
5. Telegram bot bridge for mobile access

## Platform Support

- Windows: .exe installer
- macOS: .dmg and .app
- Linux: .deb and .AppImage

## Next Steps

1. Run `npm create tauri-app@latest` to initialize
2. Copy LaunchMate frontend to src/
3. Configure tauri.conf.json for your environment
4. Add native features (notifications, tray)
5. Build and test on target platforms
