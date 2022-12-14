# Overwolf app <--> ALS

Below is an overview of the basic flow between the Overwolf app and Apex Legends Status website.

## General Flow
### App installation and user retrieval
* Overwolf app will ask the user for a valid API key which they enter manually.
* Overwolf app checks https://apexlegendsstatus.com/systems_overwolf/ow_user for valid user for that API key.
* If key is valid Overwolf app saves API key and username.

### App game data collection
* User starts game
* Overwolf app sends message to https://apexlegendsstatus.com/systems/overwolf/ow_event notifying of game start.
* Overwolf app collects event data during game.
* Overwolf app sends all game data to https://apexlegendsstatus.com/systems/overwolf/ow_event when game is done.

## More reading
* [API Key information](docs/api_key.md)
* [User retrieval API detail](docs/ow_user.md)
* [OW Event API detail](docs/ow_event.md)

