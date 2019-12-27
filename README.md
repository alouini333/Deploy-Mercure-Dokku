# Deploy your Mercure Hub to Dokku
---
In y case, I deployed [Mercure](https://mercure.rocks/) on Dokku using Dockerfile

1. Create a new application on Dokku `dokku apps:create <app-name>`
2. Config your environment variables `dokku config:set <app-name> JWT_KEY=your_key ALLOW_ANONYMOUS=1 CORS_ALLOWED_ORIGINS=* PUBLISH_ALLOWED_ORIGINS=your_origin`
3. Once the environment variables are set. Deploy and let Dokku do his magic, go to your directory and Deploy `git push dokku master`.

PS: don't forget to init your git repo and add Dokku as a remote to name the app, on your local machine.
