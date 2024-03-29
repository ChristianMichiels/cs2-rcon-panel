# CS2 RCON Web Panel

## Usage (Without Docker)
- Install NodeJS 18.0 or higher
- Run `npm install` in the root project folder
- Run `npm install -g nodemon` to install nodemon
- Run `nodemon app.js` in the root project folder
- Default login credentials can be changed from db.js

## Usage (Using Docker Compose)

`version: "3.3"
services:
  rconpanel:
    build: https://github.com/ChristianMichiels/cs2-rcon-panel.git
    ports:
      - "3000:3000"
    restart: unless-stopped`

## Abilities 

- Setup Competitive/Wingman gamemodes
- Pause/Unpause/Restart match
- List and restore round backups
- Start Knife/Warmup/Live rounds (CFGs are in cfg folder, sent via RCON)
- Send RCON Commands to the server

## Todo

- Add teams and players
- Add password option while setting up the server
- Improve UX/UI
- Improve/clean code (This is my first time working with node :P)
- Create executable

## Screenshot

![Screenshot](https://github.com/ChristianMichiels/cs2-rcon-panel/blob/master/image.png)

## Limitations

- Cannot get logs, feeds (log_address is not present in CS2 as of now)

## License

MIT
