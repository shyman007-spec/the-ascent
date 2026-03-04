# The Ascent — Setup Notes

## Live website
- **GitHub Pages URL**: https://shyman007-spec.github.io/the-ascent/
- **Custom domain**: theascentpathway.com (DNS setup — see below)
- **GitHub repo**: https://github.com/shyman007-spec/the-ascent
- **GitHub account**: shyman007-spec / jonnyblenkin@gmail.com

## How to make changes to the website
1. Edit `index.html` in this folder
2. Open terminal in this folder and run:
   ```
   git add index.html
   git commit -m "describe what you changed"
   git push
   ```
3. GitHub rebuilds the site automatically — live within ~1 minute

## Contact form
- Powered by **Web3Forms** (free, 250 submissions/month)
- Submissions go to: **jonnyblenkin@gmail.com**
- Account: web3forms.com (set up under Waller's account)
- Access key in the form: `6df167d7-6abc-4bff-9b43-f8ca324078b5`
- No login needed unless you want to change the destination email

## Email (hello@theascentpathway.com)
- Incoming mail forwarded via **ImprovMX** (free)
  - improvmx.com — set up to forward to jonnyblenkin@gmail.com
  - MX records added in 123-reg DNS
- Outgoing — Jonny replies from Gmail using "Send mail as"
  - Set up in Gmail → Settings → Accounts and Import → Send mail as

## Domain & DNS
- Registrar: **123-reg** — login at 123-reg.co.uk with Jonny's account
- Domain: theascentpathway.com + theascentpathway.co.uk
- DNS records added:
  - MX records for ImprovMX (email forwarding)
  - A records / CNAME pointing to GitHub Pages (website)

## SSH / Git setup (developer machine)
- SSH key for Jonny's GitHub at: `~/.ssh/id_ascent`
- SSH config routes `github-ascent` → github.com using that key
- Personal GitHub uses the default `~/.ssh/id_ed25519` key
- To push as Jonny: remote is already set to `git@github-ascent:shyman007-spec/the-ascent.git`

## Key files
- `index.html` — the live website (edit this directly)
- `website-v2.html` — previous working copy (kept for reference)
- `favicon.svg` — browser tab icon
- `images/` — all images including `mood-landscape.png` (hero photo)
- `fonts/` — Cormorant Garamond TTF files
