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
#### Lavender and other colors:
WIP

## CUSTOM LOGO 
- remember to replace the `YOUR LOGO URL.PNG/jpg` with your own server logo hosted on any photo hosting website of your choice/or you can place the logo in your web-dir and write `url(../../YOURLOGO.png)`
```css
.adminDrawerLogo img { content: url(YOUR LOGO URL.png/jpg) !important; } imgLogoIcon { content: url(YOUR LOGO URL.png/jpg) !important; } .pageTitleWithLogo { background-image: url(YOUR LOGO URL.png/jpg) !important; }
```

## Nginx
If you are using nginx as a reverse proxy for Jellyfin, replace the "add_header Content-Security-Policy" in your nginx config with this line below
```
add_header Content-Security-Policy "default-src https: data: blob: http://image.tmdb.org; style-src 'self' 'unsafe-inline' https://fallenbagel.github.io ; script-src 'self' 'unsafe-inline' https://www.gstatic.com/cv/js/sender/v1/cast_sender.js https://www.youtube.com blob:; worker-src 'self' blob:; connect-src 'self'; object-src 'none'; frame-ancestors 'self'";
```

## To enable fanart/logo
- Install the Fanart plugin first
- Go to Dashboard > Library
- For each library you have, go to Manage Library
- Enable Fanart for image fetcher
- Then go to Fetcher Settings and select "Logo"
- Manually scan media library
- Refresh the page once done

## Login Page
![Screenshot 2022-03-21 022640](https://user-images.githubusercontent.com/98979876/159188491-5dc0005c-b36c-4f7f-afcd-1030f4d862fe.jpg)
![Screenshot 2022-03-21 022706](https://user-images.githubusercontent.com/98979876/159188516-9ad682ca-25ad-46cd-aff2-7c2058162340.jpg)

## Blur background with header tabs, avatar and CUSTOM SERVER LOGO
![screenshot1](https://user-images.githubusercontent.com/98979876/159188880-0307b8c7-7a50-461d-9580-a745bb5dea8b.png)
![Screenshot w hoverw](https://user-images.githubusercontent.com/98979876/159189075-423636b9-ba92-4174-935d-59d5e46dd48d.png)
![Screenshot2](https://user-images.githubusercontent.com/98979876/159189097-d2fddd0b-b411-48ae-82b6-296f301548a9.png)
![screenshot3](https://user-images.githubusercontent.com/98979876/159189104-7dd51b97-aefe-44c9-9837-656230be1843.png)

## Dashboard, Sidebar, Shutdown button, Scan Libraries and Text Field border
![Dashboard](https://user-images.githubusercontent.com/98979876/159189141-f1528982-0eaf-479b-a788-44089c6fe5ed.png)
![Hover over scan all libraries](https://user-images.githubusercontent.com/98979876/159189142-4d141e68-4246-45cd-9772-da255c0404f3.png)
![Hover over shutdown](https://user-images.githubusercontent.com/98979876/159189143-395121dc-4ed5-4ffb-a9d6-c866b05851df.png)
![Sidebar](https://user-images.githubusercontent.com/98979876/159189144-12855eff-a9c3-4e5e-9d9b-629096806267.png)
![Text field border](https://user-images.githubusercontent.com/98979876/159189146-f640fb59-b316-48d9-9ad5-455234722a07.png)

