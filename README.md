# foodswiper-site

The public pages Apple requires for I Feel Like Food: support, privacy policy, terms of use and prize
rules. Plain HTML, served by GitHub Pages at `https://weemalcy.github.io/foodswiper-site/`. The app
links to these exact paths (`AppLinks` in foodswiper-ios).

## Before publishing

1. Replace every `[PLACEHOLDER]` (name, address, support email, legal basis, retention period,
   governing law), and have a solicitor review the texts.
2. Keep `rules.html` in step with the in-app copy (`PrizeRulesView.swift`). Apple requires the rules
   inside the app (guideline 5.3.2).

## Publishing

1. Create a **public** repo `weemalcy/foodswiper-site` on GitHub and push this folder to `main`.
2. Repo Settings → Pages → Source: *Deploy from a branch*, branch `main`, folder `/ (root)`.

When the terms or privacy policy change in a way people must agree to again, bump `TermsVersion.current`
in the app too, and everyone is asked to accept at their next launch.
