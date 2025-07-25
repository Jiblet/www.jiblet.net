# www.jiblet.net
[www.jiblet.net](https://www.jiblet.net), a VERY minimal site.
For now, it’s a splash page that redirects to a custom **418: I'm a teapot** error. Why? It was late and I needed *something*.

## 🫖 Contents
- `index.html` - Redirects immediately to `/418.html`
- `418.html` - "I'm a teapot" error page
- `.gitignore` - Keeps Vim temp files and OS cruft out of version control

## 🛠️ Intent
Might one day become link portal to rival the jiblet.net of the early 2000s.
For now, it's a monument to questionable decision-making.

## 🪞 Deployment

This site is served using [Caddy](https://caddyserver.com/) with the following configuration:

```caddyfile
www.jiblet.net {
    root * /srv/www.jiblet.net
    file_server
}
```

Content lives at `/srv/www.jiblet.net` on the host system. No extra rewrite logic, no TLS directives—just pure static delivery.

## 🧾 License
Unlicensed. If you want to use it, that's a you problem. 

