# Konversions-Web-App-Vorlage
Dies ist ein [Next.js](https://nextjs.org/) Projekt, initialisiert mit [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## App Konfigurieren
Erstelle eine Datei namens `.env.local` im aktuellen Verzeichnis und kopiere den Inhalt aus `.env.example`. Setze den folgenden Inhalt:
```
# APP ID
NEXT_PUBLIC_APP_ID=
# APP API Schlüssel
NEXT_PUBLIC_APP_KEY=
```

Weitere Konfigurationen in der Datei `config/index.ts`:   
```js
export const APP_INFO: AppInfo = {
  titel: 'Chat APP',
  beschreibung: '',
  urheberrecht: '',
  datenschutzrichtlinie: '',
  standard_sprache: 'zh-Hans'
}

export const isShowPrompt = true
export const promptTemplate = ''
```

## Erste Schritte
Zuerst, installiere Abhängigkeiten:
```bash
npm install
# oder
yarn
# oder
pnpm install
```

Dann starte den Entwicklungsserver:

```bash
npm run dev
# oder
yarn dev
# oder
pnpm dev
```
Öffne [http://localhost:3000](http://localhost:3000) in deinem Browser, um das Ergebnis zu sehen.

## Mit Docker verwenden

```
docker build . -t <DOCKER_HUB_REPO>/webapp-conversation:latest
# jetzt kannst du es auf Port 3000 zugreifen
docker run -p 3000:3000 <DOCKER_HUB_REPO>/webapp-conversation:latest
```

Öffne [http://localhost:3000](http://localhost:3000) in deinem Browser, um das Ergebnis zu sehen.

## Mehr Erfahren

Um mehr über Next.js zu erfahren, sieh dir die folgenden Ressourcen an:

- [Next.js Dokumentation](https://nextjs.org/docs) - erfahre mehr über Next.js Funktionen und API.
- [Next.js lernen](https://nextjs.org/learn) - ein interaktives Next.js Tutorial.

Du kannst auch [das Next.js GitHub-Repository](https://github.com/vercel/next.js/) besuchen - dein Feedback und Beiträge sind willkommen!

## Auf Vercel deployen

> ⚠️ Wenn du [Vercel Hobby](https://vercel.com/pricing) verwendest, wird deine Nachricht aufgrund der Vercel-Beschränkung gekürzt.

Die einfachste Art, deine Next.js-App zu deployen, ist die Verwendung der [Vercel-Plattform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) von den Schöpfern von Next.js.

Sieh dir unsere [Next.js-Deployment-Dokumentation](https://nextjs.org/docs/deployment) für weitere Details an.
