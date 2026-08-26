# Privacy Policy (Static)

Simple static Privacy Policy page served with Node.js `serve`.

## Structure

```
privacy-policy/
├── public/
│   └── index.html          # The privacy policy page
├── package.json
├── Dockerfile
├── docker-compose.yml
└── .dockerignore
```

## Run locally

```bash
cd privacy-policy
npm install
npm start
```

Open: http://localhost:3000

## Deploy with Dokploy

1. Create a new **Compose** application in Dokploy.
2. Point it to this folder (or paste the `docker-compose.yml` content).
3. Dokploy will build the image and run the container on port `3000`.
4. Attach a domain / enable HTTPS in Dokploy.

That's it. No Nginx needed — pure Node `serve`.
