# Hint of Colors
Jellyfin CSS Theme

Hint of Colors is a fork of Hint of Green CSS but with different colors (main being lavender but it's up to your choice). Although the green theme looks similar to hint of green, it is heavily modified to my liking (includes library in mobile, profile pictures, better login screen, better item logo,....etc.)

<sub><sup> * (Blue, orange, red, etc; WIP). </sup></sub>

## Tested on
- Chrome, Firefox, Safari and common Jellyfin applications
- Jellyfin 10.6 - 10.8.0

## Features
- Colours are based on a pastel palatte
- A lot of the features of hint of green but REVAMPED
- Selection of different colors(Lavender, blue, orange, red, etc; WIP).

Just like hint of green CSS, this theme can be considered as heavy but should work on almost all clients.

## Installation
There will be **SEPERATE** channels for each colors. Newer colors are WIP.

**_Required_** Go to Settings > Home > Home screen section 1: > select `My Media (small)`
This step is necessary for the theme to be applied to library buttons.

Copy this code into Dashboard > General > Custom CSS
#### Lavender (Main):
```css
@import url('https://fallenbagel.github.io/Hint-of-Colors/lavender.css');
```
or
#### Green:
```css
@import url('https://fallenbagel.github.io/Hint-of-Colors/green.css');
```
or
## Other colors (WIP)


## CUSTOM LOGO 
- Remember to replace the `YOUR LOGO URL.PNG/jpg` with your own server logo hosted on any photo hosting website of your choice/or you can place the logo in your web-dir and write `url(../../YOURLOGO.png)`
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
![image](https://user-images.githubusercontent.com/98979876/173200609-43064591-fec9-4fb5-b8fe-2fd2a31d59da.png)
![image](https://user-images.githubusercontent.com/98979876/173200640-35b261ec-4921-40ae-aa77-fd591796e1e6.png)

## Blur background with header tabs, avatar and CUSTOM SERVER LOGO
![image](https://user-images.githubusercontent.com/98979876/173200722-e8859932-cb5b-46e6-938c-357a5db0be9b.png)

## Library Buttons Hover
![image](https://user-images.githubusercontent.com/98979876/173200743-c235679a-c819-4ce9-883e-17110dce0b32.png)

## Play Card Hover
![image](https://user-images.githubusercontent.com/98979876/173200750-0c3a5fa0-5697-454f-a953-4e60a6c96463.png)

## Item Detail Movies
![image](https://user-images.githubusercontent.com/98979876/173201082-128b037e-f2f5-48f6-86e6-7c363cb629e5.png)
![image](https://user-images.githubusercontent.com/98979876/173201108-7cabe70a-a128-4bcf-9bc4-134798104b2c.png)

## Item Detail Series
![image](https://user-images.githubusercontent.com/98979876/173201125-70eb74b9-7e02-4f08-ba09-aa9b552d17b5.png)
![image](https://user-images.githubusercontent.com/98979876/173201137-dc2a9c48-8fa8-4dba-84b9-592300f8e1ce.png)
![image](https://user-images.githubusercontent.com/98979876/173201152-be92cdff-3485-47fb-8f08-035b4b7bb1fe.png)
![image](https://user-images.githubusercontent.com/98979876/173201161-f8202548-d300-40db-a326-c2768ad459bd.png)


## Dashboard
![image](https://user-images.githubusercontent.com/98979876/173200966-2432e179-56b1-4306-8f71-8b22e6e244ca.png)

## Dashboard Activity
![Untitled-1](https://user-images.githubusercontent.com/98979876/173200833-9a380603-8ca1-4bad-8f4d-64f8e75f6f57.png)

## Scan Libraries (hover)
![image](https://user-images.githubusercontent.com/98979876/173200968-018c5391-0d13-4aca-a4da-8e1fbc7a6083.png)

## Shutdown (hover)
![image](https://user-images.githubusercontent.com/98979876/173200972-cd51fe50-2c92-40c3-8922-2712ede37879.png)

## Text field and tick boxes
![image](https://user-images.githubusercontent.com/98979876/173200992-54c07c53-725c-44a4-95d5-912af9606150.png)

## Sidebar
![image](https://user-images.githubusercontent.com/98979876/173200997-f7c8bd99-047a-4fc6-b816-71cbdd7a7da9.png)

