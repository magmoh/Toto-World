# Toto World Production v3

End-to-end Beta application for personalized children's stories.

## Included
- Arabic RTL sales site and Magic Preview
- Parent consent before child-photo processing
- Customer access token protecting order data and images
- Boy/girl grammar-aware Story Engine
- Age bands 4–5, 6–7, 8–9
- Golden Story 01: Toto on the Farm, 12 pages
- AI image-generation integration points using child reference + locked Toto reference
- Dynamic text layer separate from AI artwork
- Moyasar checkout and server-side payment verification
- Demo payment mode
- Admin generation/approval workflow
- Parent order deletion endpoint
- Privacy / Terms / Refund / Contact pages
- Persistent storage via `DATA_DIR`
- Render Blueprint + Dockerfile
- QC, smoke and preflight scripts

## Local run
```bash
cp .env.example .env
npm install
npm run smoke
npm run qc
npm start
```
Open `http://localhost:3000`.

## Production
See `DEPLOYMENT.md`.

## Important
Do not put OpenAI or Moyasar secret keys in browser code. The legal pages are operational Beta drafts and must be reviewed for the final legal entity before public sales.
