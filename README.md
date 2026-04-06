# Redirect-Repository fuer jorgmartindigital.de

Dieses Repository dient nur dazu, die alte Domain auf die neue Domain weiterzuleiten:
- Quelle: xn--jrgmartindigital-mwb.de
- Ziel: https://joergmartindigital.de

## Dateien

- CNAME: alte Domain (Punycode)
- index.html: Redirect fuer Startseite und normale Aufrufe
- 404.html: Redirect fuer Unterseiten/Fallback

## GitHub Pages

1. Repository auf GitHub anlegen (z. B. joergmartindigital-redirect)
2. Inhalt dieses Ordners hochladen
3. Pages aktivieren: Deploy from branch main / root
4. Custom domain setzen: xn--jrgmartindigital-mwb.de
5. Enforce HTTPS aktivieren, sobald verfuegbar

## DNS (alte Domain in Strato)

Apex (@) auf GitHub Pages:
- A 185.199.108.153
- A 185.199.109.153
- A 185.199.110.153
- A 185.199.111.153

Optional AAAA:
- 2606:50c0:8000::153
- 2606:50c0:8001::153
- 2606:50c0:8002::153
- 2606:50c0:8003::153

www:
- CNAME auf <dein-github-username>.github.io

Hinweis: Ohne gueltiges HTTPS-Zertifikat auf der alten Domain wird bei https-Aufrufen eine Browserwarnung erscheinen.
Mit GitHub Pages + Custom Domain fuer die alte Domain kann GitHub das Zertifikat bereitstellen.
