# Toto World Production v3

Toto World is an Arabic-first personalized children's story platform. This repository contains the deployable Production v3 bundle plus the Render Blueprint used to unpack and run the Node application.

## Deployment bundle
- `source-bundle.tar.gz` — application source, Story Engine, admin flow, checkout, legal pages and server code.
- `assets-bundle.tar.gz` — compressed demo/reference artwork used by the Beta build.
- `render.yaml` — Render Blueprint. It unpacks both bundles during build, installs Node dependencies, mounts persistent storage, and starts the application.

## Product capabilities
- Parent-first Magic Preview
- Boy/girl Arabic grammar-aware story personalization
- Reading levels for ages 4–5, 6–7, 8–9
- Golden Story 01: Toto on the Farm
- Dynamic text layer separate from generated artwork
- Customer access tokens for order/photo protection
- OpenAI image-generation integration points
- Moyasar checkout and server-side payment verification
- Admin QA/generation/approval workflow
- Parent order/data deletion route
- Privacy, Terms, Refund and Contact pages

## Go-live approach
Deploy the Blueprint to a Beta hostname first (recommended: `beta.toto-world.com`). Keep AI generation and live payments disabled until the Beta flow has passed a full end-to-end order review. Then add the OpenAI and Moyasar secrets in the hosting provider's environment settings — never commit secrets to GitHub.

## Important
Legal pages are Beta operational drafts. Insert the final legal entity, CR/VAT details, support email/phone and obtain appropriate legal/privacy review before public paid launch.
