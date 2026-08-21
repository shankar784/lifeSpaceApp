# LifeSpace website

Static site for the LifeSpace Android app. No build step — plain HTML, CSS and one small script.

```
index.html              landing page
privacy-policy.html     privacy policy (has placeholders to fill in)
assets/                 icons, social card, screenshots
```

## Publish on GitHub Pages

1. Create a **public** repo. If you name it `lifespace`, the site will live at
   `https://YOURNAME.github.io/lifespace`.
2. Upload the contents of this folder to the repo root — not the folder itself.
   `index.html` must sit at the top level.
3. Repo **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
4. Wait 1–2 minutes, then open the URL. Pages shows it at the top of that settings screen.

## Fill in before you share the link

- [ ] `privacy-policy.html` — replace every yellow-highlighted placeholder
- [ ] `privacy-policy.html` — delete the `<div class="editme">` block at the top
- [ ] `index.html` — replace `REPLACE-WITH-YOUR-EMAIL@example.com` in the footer
- [ ] Both files — confirm the feature descriptions match what the app actually does

The privacy policy is a starting template, not legal advice. Google Play rejects policies
with unfilled template text, and a policy that misdescribes your data handling is a policy
violation in itself.

## Later: custom domain and app-ads.txt

A `github.io` URL is fine for signing up with an ad network. Before you optimise revenue,
move to a domain you own:

1. Buy a domain (Cloudflare or Namecheap, roughly ₹800–1,200/year).
2. Repo **Settings → Pages → Custom domain**, and add the DNS records GitHub shows you.
3. Set that domain as the **Developer website** on your Play Store listing.
4. Add an `app-ads.txt` file at the domain root, containing the exact lines your ad network
   gives you after you create ad units.

Don't add `app-ads.txt` yet. An empty or placeholder file tells crawlers that *no one* is
authorised to sell your inventory, which is worse than having no file at all. Add it only
once you have real publisher IDs.

## Assets

Screenshots here are resized to 620px wide and converted to WebP (about 800 KB total,
down from 20 MB). Keep your full-resolution 1242×2208 PNGs — you'll need those for the
Play Store listing.
