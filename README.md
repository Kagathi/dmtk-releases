# DM Toolkit
A system-agnostic tabletop companion (not a VTT) that enhances in-person TTRPG sessions. The DM/GM runs a desktop app that acts as the table's server; players join from their phone browsers over the local network. An optional TV/projector "display" screen can show maps and images to the whole table. One of the base tenants of DM Toolkit is local only, no online subscription or cloud hosting. The only time an internet connection is required is updating the app or adding/updating a ruleset. 

## Tech Stack

- **Node 24 LTS**, **pnpm** workspaces, **TypeScript** (strict) everywhere.
- **React + Vite** (player web app, DM renderer), **Electron** (DM desktop app).
- **Express + socket.io** (embedded server), **`node:sqlite` + Drizzle ORM**

# Backstory
This piece of software is something I have been playing around with for years. The first iteration of this was a website written in c# back in late 2015 for my first group. Since then it has gone though several iterations with different groups and campaigns. Now with the help of AI I have been able to get the software to a state where I am happy to share it with the public. So feel free to take the app for a spin and let me know if you find any bugs or want additional features added in. 
