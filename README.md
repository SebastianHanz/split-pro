<p align="center" style="margin-top: 12px">
  <a href="https://splitpro.app">
  <img width="100px"  style="border-radius: 50%;" src="https://splitpro.app/logo_circle.png" alt="SplitPro Logo">
  </a>

  <h1 align="center">SplitPro</h1>
  <h2 align="center">An open source alternative to Splitwise</h2>

<p align="center">
    <a href="https://splitpro.app"><strong>To our App »</strong></a>
    <br />
    <br />
  </p>
</p>

## Über diese App

SplitPro zielt darauf ab, eine Open-Source-Lösung zum Teilen von Ausgaben mit Freunden bereitzustellen.

Es soll ein vollständiger Ersatz für Splitwise sein.

Aktuell sind die meisten wichtigen Funktionen vorhanden.

- Ausgaben mit Einzelpersonen oder Gruppen hinzufügen
- Gesamtsalden über alle Gruppen hinweg
- Unterstützung für mehrere Währungen
- Hochladen von Rechnungen für Ausgaben
- PWA-Unterstützung (installierbar als Web-App)
- Ungleiche Aufteilung von Ausgaben (Anteile, - Prozentsätze, genaue Beträge, Anpassungen)
- Push-Benachrichtigungen
- Herunterladen deiner Daten
- Import von Splitwise

**Der Funktionsumfang wird ständig erweitert**

---

## Wieso

Splitwise ist eine der besten Apps, um Ausgaben und Rechnungen hinzuzufügen.

Ich verstehe, dass jede App Geld verdienen muss; schließlich wurde viel Aufwand in Splitwise gesteckt. Mein Hauptproblem ist jedoch, wie sie dies umgesetzt haben.

Die Monetarisierung durch Pro-Funktionen oder Werbung ist in Ordnung, aber Geld für das Hinzufügen von Ausgaben (einer Kernfunktion) zu verlangen, ist frustrierend.

Ich habe nach anderen Open-Source-Alternativen gesucht (um ehrlich zu sein, könnte jedes geschlossene Produkt dasselbe tun, und ich habe keinen Grund, das Gegenteil anzunehmen).

Ich habe eune gute App [spliit.app](https://spliit.app/) von [Sebastien Castiel](https://scastiel.dev/) gefunden, aber sie ist für mich kein vollständiger Ersatz für Splitwise und passt nicht zu meinem workflow. Probiert sie aus und schaut wie sie zu euch passt.

_Darum habe ich mich entschlossen dieses Projekt zu beginnen_

## Tech stack

- [NextJS](https://nextjs.org/)
- [Tailwind](https://tailwindcss.com/)
- [tRPC](https://trpc.io/)
- [ShadcnUI](https://ui.shadcn.com/)
- [Prisma](https://www.prisma.io/)
- [Postgres](https://www.postgresql.org/)
- [NextAuth](https://next-auth.js.org/)

## Getting started.

### Anforderungen

- Node.js (Version: >=18.x)
- PostgreSQL
- pnpm (recommended)

## Docker

We provide a Docker container for Splitpro, which is published on both DockerHub and GitHub Container Registry.

DockerHub: [https://hub.docker.com/r/ossapps/splitpro](https://hub.docker.com/r/ossapps/splitpro)

GitHub Container Registry: [https://ghcr.io/oss-apps/splitpro](https://ghcr.io/oss-apps/splitpro)

You can pull the Docker image from either of these registries and run it with your preferred container hosting provider.

Please note that you will need to provide environment variables for connecting to the database, redis, aws and so forth.

For detailed instructions on how to configure and run the Docker container, please refer to the Docker [Docker README](./docker/README.md) in the docker directory.

## Developer Setup

### Install Dependencies

```bash
corepack enable
```

```bash
pnpm i
```

### Setting up the environment

- Copy the env.example file into .env
- Setup google oauth required for auth https://next-auth.js.org/providers/google or Email provider by setting SMTP details
- Login to minio console using `splitpro` user and password `password` and [create access keys](http://localhost:9001/access-keys/new-account) and the R2 related env variables

### Run the app

```bash
pnpm d
```

## Sponsors

We are grateful for the support of our sponsors.

### Our Sponsors

<a href="https://hekuta.net/en" target="_blank">
  <img src="https://avatars.githubusercontent.com/u/70084358?v=4" alt="hekuta" style="width:60px;height:60px;">
</a>
