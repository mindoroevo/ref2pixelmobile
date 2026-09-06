# Mindoro Pixel Studio – Privacy Policy

Static English and German privacy policy for Mindoro Pixel Studio (formerly Ref2Pixel).

This repository currently hosts the public privacy policy via GitHub Pages.

The page content is generated from `src/app/legal-content.js` in the app repository
(`C:/Users/User/r2p_mobil`). Its existing inline styles are preserved. Both languages
are included in the HTML; no JavaScript, advertising or analytics scripts are needed.

From the app repository, verify that the local website matches the app:

```powershell
node scripts/render-privacy-page.mjs --check C:/Users/User/Documents/github/ref2pixelmobile/index.html
```

After editing the app's privacy text, generate an `apply_patch` patch with:

```powershell
node scripts/render-privacy-page.mjs --patch C:/Users/User/Documents/github/ref2pixelmobile/index.html
```

Apply that patch, then run the check again. The renderer does not write, commit,
push or publish files. Publishing still requires the repository's normal GitHub
Pages workflow. The existing `app-ads.txt` is separate and is not regenerated.

Before publishing, review the operational and legal checklist in the app repository's
`docs/PRIVACY-MAINTENANCE.md`. Text updates do not configure AdMob consent messages
or update Google Play's Data safety declarations.

Live page:
https://mindoroevo.github.io/ref2pixelmobile/
