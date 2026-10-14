# Outside AI

Static Astro site for Outside AI, deployed on Cloudflare Pages.

## Commands

```sh
npm install
npm run build
npm run preview
```

Production URL: https://outside-ai.com/

## Website

Outside AI offers affordable custom AI tools for small and medium businesses, working with their existing systems, and always-on personal assistants for executives, families, and individuals.

Pages: home, `/services/`, `/testimonials/`, and `/consultation/`.

The consultation page follows the date-selection approach of the Cusoon scheduler. Visitors choose a future weekday, time window, and time zone, then review and send a prefilled email to `keith@outside-ai.com`. It does not check live availability or automatically reserve a time. Requests require email confirmation.

Testimonials are clearly disclosed fictional examples until real customer reviews are available.

For temporary Cloudflare previews, run `npm run preview -- --host 127.0.0.1 --port 4321` and `cloudflared tunnel --url http://127.0.0.1:4321 --no-autoupdate`. The generated URL lasts only while both processes are running. Preview hostnames are allowed in the Astro server configuration.
