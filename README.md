# DappyKit + Farcaster + Vercel Template

This is a Quiz Typescript Frame template for Farcaster integrated with DappyKit. The template is ready to deploy on Vercel. A KV storage must be created to store user sessions for the project to work.

In the `./quiz.json` file, a list of questions and answers is stored.
The project is configured in Vercel through environment variables. Here is the list of variables:
- `APP_OWNER_FID` - a unique user number in Farcaster, the application administrator.
- `APP_PK` - an ETH-compatible private key in 0x format for signing messages.
- `APP_SHARE_URL` - the link to the Frame itself after deployment, needed to share the Quiz with other users.
- `APP_AUTH_URL` - not required. The link to the authorization Frame. You can provide your own if the standard one doesn't fit.
- `APP_TITLE` - not required. The title of your application.
- `KV_NAMESPACE` - not required. A unique namespace for your application. Required only if multiple applications use the same KV storage.

## Installation
```
npm ci
npm run dev
```

Go to http://localhost:5173/api/dev
