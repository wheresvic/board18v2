# board18

This repository is a fork of the board18 repository created by Richard Price. Board18 is a web application designed to enable playing 18xx style games online. It features a map, stock market and tile laying without any rules enforcements. Those are up to the players and are dependent upon the game being played.

For documentation on see `Documentation/Readme.txt`.

For all intents and purposes the master branch will be kept uptodate with the upstream master branch.

## optional public registration

This repository also features a branch `feat/optional-public-registration` which enables a true/false configuration parameter `ENABLE_REGISTRATION` (default `true`). Changing this parameter to false will disable the registration function and only the admin user will thereafter be allowed to register users. This might be useful in case you would like to run the instance on a local network for LAN play.

### installation

Checkout this repository and switch to `feat/optional-public-registration` branch. Switch to the `makedist` folder and run `./BOARD18make` script to create an installation package.

Follow the main board18 instructions on creating the database and installation. After the intial admin user has been registered, you can disable public registration by changing flag in `php/config.php`.
