# Hint of Colors
Jellyfin CSS Theme

This is a fork of Hint of Green CSS (Very beautiful css), however, I modified this to better suite my taste to include library in mobile, profile pictures, better login screen, better item logo,....etc. **AND BEST OF ALL, NOT JUST LIMITED TO GREEN**(Lavender, blue, orange, red, etc; WIP).

## Tested on
- Chrome, Firefox, Safari and common Jellyfin applications
- Jellyfin 10.6 - 10.8.0

## Features
- Colours are based on a pastel palatte
- A lot of the features of hint of green but REVAMPED
- Selection of different colors(Lavender, blue, orange, red, etc; WIP).

Just like hint of green CSS, this theme can be considered as heavy but should work on almost all clients (maybe except safari).

## Installation
There will be **SEPERATE** channels for each colors. Newer colors are WIP.

Copy this code into Dashboard > General > Custom CSS
#### Green:
```css
@import url('https://fallenbagel.github.io/Hint-of-Colors/green.css');
```
or
#### Lavender:
WIP

## Nginx
If you are using nginx as a reverse proxy for Jellyfin, replace the "add_header Content-Security-Policy" in your nginx config with this line below
```
add_header Content-Security-Policy "default-src https: data: blob: http://image.tmdb.org; style-src 'self' 'unsafe-inline' https://fallenbagel.github.io ; script-src 'self' 'unsafe-inline' https://www.gstatic.com/cv/js/sender/v1/cast_sender.js https://www.youtube.com blob:; worker-src 'self' blob:; connect-src 'self'; object-src 'none'; frame-ancestors 'self'";
``
## To enable fanart/logo
- Install the Fanart plugin first
- Go to Dashboard > Library
- For each library you have, go to Manage Library
- Enable Fanart for image fetcher
- Then go to Fetcher Settings and select "Logo"
- Manually scan media library
- Refresh the page once done
