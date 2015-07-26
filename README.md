# config
Some system config files

Conky scripts contain:
 1. A script that shows Transmission speeds (circle working)
 2. A script that shows Nzbget speeds (circle working)
 3. A script that shows Now Playing. Source CMUS/Spotify
 4. A script that shows the current weather/temp (+icon)
 5. A script that show the public IP
 6. A script that shows upcoming TV Shows from Sonarr
 7. A script that shows upcoming movies from CouchPotato

Known bug: CouchPotato script is a little wonky sometimes. If .release_date (from the json that's fetched through the API) does not contain a value for "dvd", then the last movie in your wanted list gets shows too without a date. Removing and re-adding the movie that causes this often fixes it. Also CouchPotato is a bit inaccurate with the dates.

Note: Several conky script rely on underscore-cli to parse the json. Please make sure you have it installed and it's available in your $PATH.
