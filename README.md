# Fitness Warehouse NYC Website
Landing page for Fitness Warehouse NYC

Use Node 24+:
```bash
nvm use
```

Install Dependencies:
```bash
npm i
```

Run Locally:
```bash
npm run dev
```

Build:
```bash
npm run build
```

---

# DNS Setup

## Domain & Services

- **Domain registrar:** Dynadot
- **Website hosting:** Netlify
- **Website:** `https://fitnesswarehousenyc.com`
- **Email provider:** Dynadot
- **Email address:** `jim@fitnesswarehousenyc.com`

## DNS Records

Manage DNS in Dynadot under **My Domains → Manage Domains → fitnesswarehousenyc.com → DNS Settings**.

### Website

| Type | Host | Value |
|---|---|---|
| A | `@` | `75.2.60.5` |
| CNAME | `www` | `fitness-warehouse-nyc.netlify.app` |

These records point the apex domain and `www` subdomain to Netlify.

### Email

Use the MX records and any additional DNS records specified in the Dynadot email setup instructions for the email service purchased.

Do not guess the mail server values. Keep the website records above when adding email records.

## Netlify Configuration

In Netlify's Domain management settings, add:

- `fitnesswarehousenyc.com`
- `www.fitnesswarehousenyc.com`

Choose a primary domain and configure the other to redirect to it. Ensure HTTPS is enabled.

## Verification Checklist

- [ ] Apex domain loads the website.
- [ ] `www` loads the website or redirects to the apex domain.
- [ ] HTTPS works on both domain names.
- [ ] `jim@fitnesswarehousenyc.com` can send and receive email.
