# KI-Chat – lokale iPhone-Web-App

Die App ist eine PWA: Chats, Einstellungen und API-Key bleiben in Safari auf dem jeweiligen Gerät. Es gibt keinen Python-Server und keine Online-Datenbank.

## Kostenlos veröffentlichen

1. Erstelle einen kostenlosen Account bei [GitHub](https://github.com/signup) und ein neues **öffentliches** Repository, zum Beispiel `ki-chat`.
2. Lade den gesamten Inhalt dieses Ordners (`KIChatPWA`) über **Add file → Upload files** hoch.
3. Im Repository: **Settings → Pages → Deploy from a branch → main / (root) → Save**.
4. Nach kurzer Zeit ist die Adresse `https://DEIN-NAME.github.io/ki-chat/` verfügbar.
5. Öffne diese Adresse auf dem iPhone in **Safari**. Tippe auf **Teilen** → **Zum Home-Bildschirm** → **Hinzufügen**.

Beim ersten Start trägst du unter Einstellungen deinen NVIDIA-API-Key ein. Er wird nur in der lokalen iPhone-Datenbank gespeichert. Die App funktioniert nicht im Privatmodus, weil Safari dort Daten löschen kann.

> Hinweis: Die NVIDIA-Schnittstelle muss Anfragen aus dem Browser (CORS) akzeptieren. Wenn Safari eine CORS-Fehlermeldung zeigt, lässt sich das ohne kostenpflichtigen Server nicht direkt umgehen; dann kann ein kostenloser Cloudflare-Worker als reiner API-Vermittler ergänzt werden, während Chats weiter lokal bleiben.
