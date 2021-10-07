
### 1. Start the application

To run your site locally, use:

```
npm run dev
```

To run it in production mode, use:

```
npm run build
npm run start
```

### 2. Preparing for Production

You must set the `NEXTAUTH_URL` environment variable with the URL of your site, before deploying to production.

e.g. in your `.env.local` file - `NEXTAUTH_URL=https://example.com`

To do this with Vercel, you can use the [Vercel project dashboard](https://vercel.com/dashboard) or their cli via the `vc env` command:

```
vc env add NEXTAUTH_URL production
```

Do not forget to set the environment variables for the Client ID and Client Secret values for all your configured authentication providers in your hosting providers dashboard, i.e. with Vercel as described above.

## License

ISC

