# TableTap site

```
index.html               TableTap landing page (reads assets/site.json)
assets/site.json         demo list + contact links: the one file you edit
assets/                  logo badge, cover, favicon
demo/                    public demos: demo/cafe, demo/restaurant, demo/bakery
demo/cards/              printable QR cards (customer + owner) for the 3 demos
tools/client-kit.html    make a new client's menu file + QR cards (open it on the live site)
_template/index.html     blank menu page (not published, kept for reference)
<client-name>/index.html one folder per paying client
```

## Add a new client (about 10 minutes)
1. Open the client's demo sheet in Google Sheets, File > Make a copy, and replace the items/prices.
   Share it: "Anyone with the link: Viewer" + the owner's Gmail as Editor.
2. Open the copy on its "القائمة" tab and copy the browser address (it must contain `#gid=`).
3. Open `https://tabletapmenu.github.io/tools/client-kit.html`, fill in the form, press "Generate".
4. Download `index.html`, create a folder named after the client in this repo (Add file > Create new file:
   type `clientname/index.html`, paste the content; or Upload files into a new folder).
5. Wait ~1 minute, open `https://tabletapmenu.github.io/clientname/`, then print the cards from the kit.

Folder names are permanent once QR codes are printed: never rename them.
Landing page contents (demo list, Facebook / WhatsApp / Instagram buttons) come from `assets/site.json`.
Edit that file on GitHub (pencil icon) and commit: no HTML changes needed. Leave a contact value empty to hide its button.
