# DM Toolkit
A system-agnostic tabletop companion (not a VTT) that enhances in-person TTRPG sessions. The DM/GM runs a desktop app that acts as the table's server; players join from their phone browsers over the local network. An optional TV/projector "display" screen can show maps and images to the whole table. One of the base tenants of DM Toolkit is local only, no online subscription or cloud hosting. The only time an internet connection is required is updating the app or adding/updating a ruleset. 

## Tech Stack

- **Node 24 LTS**, **pnpm** workspaces, **TypeScript** (strict) everywhere.
- **React + Vite** (player web app, DM renderer), **Electron** (DM desktop app).
- **Express + socket.io** (embedded server), **`node:sqlite` + Drizzle ORM**
