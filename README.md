# Shreya Thakur — Portfolio Website

A single-page interactive portfolio showcasing projects, skills, and contact details.

## Tech

Single self-contained HTML/CSS/JS, no build step. Everything (markup, styling, and scripts) lives in one file (`index.html`).

## Live

[https://portfolio-website-nine-lovat-74.vercel.app](https://portfolio-website-nine-lovat-74.vercel.app)

## Local preview

Open `index.html` in a browser.

> Note: the contact form (Web3Forms/FormSubmit) requires the page to be served over a real `https://` domain — it will not deliver mail when `index.html` is opened directly as a `file://` path.

## Contact form setup

The contact form is currently wired to **Web3Forms** (`https://api.web3forms.com/submit`), with a **FormSubmit.co** version kept commented out in the script as a fallback alternative.

### Web3Forms (active)
1. Go to [web3forms.com](https://web3forms.com) and generate a free access key using `shreyathakurindia@gmail.com`.
2. In `index.html`, find `const WEB3FORMS_ACCESS_KEY='YOUR_WEB3FORMS_ACCESS_KEY';` and replace the placeholder with the real key.
3. Submissions send full details to `shreyathakurindia@gmail.com` and trigger an auto-reply to the visitor: *"Thank you for connecting! Shreya Thakur has received your message and will get in touch with you soon."*

### FormSubmit.co (fallback, currently commented out)
If switching back to FormSubmit, note its one-time activation requirement:
1. The **first** submission sends an activation email to `shreyathakurindia@gmail.com`.
2. The **"Activate"** link in that email must be clicked before *any* mail — including the visitor auto-reply — will be delivered. Check Spam/Promotions if it doesn't appear.
3. FormSubmit only works reliably when the page is served from a real `https://` domain (e.g. Vercel), not opened locally as `file://`.
