# November Costing — Windows Updates

Official Windows update channel for November Costing.

This repository distributes application updates only. It does not contain kitchen databases, recipes, purchasing prices, accounting spreadsheets, Google Drive configuration, uploads or backups.

## Using updates

Install the private initialization package supplied to your kitchen once. Thereafter the application checks this channel when it starts and periodically while running, downloads verified updates in the background, and installs after a normal exit and successful local backup. It does not restart the app while you are editing a recipe.

Kitchen data stays in `%APPDATA%\November Costing`. Software updates and Google Drive ingredient-price synchronization are separate functions. This is not multi-device recipe synchronization.

## Release files

Each stable release provides a Windows x64 NSIS installer, `latest.yml`, an installer blockmap, and an Ed25519-signed `november-update.json` manifest. The application verifies the signed manifest and installer digest before staging an update.

Do not upload private initialization packages or local database backups to this public repository.
