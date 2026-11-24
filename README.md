# VAT-2027

An interactive concept of how an Irish VAT return could be prepared with AI agents doing the groundwork and people making the decisions.

It walks through a bi-monthly VAT3 return for a fictional Dublin company, Liffey Lane Interiors Ltd, from the client's data export to filing. Agents read, match, classify and check every invoice and show their working. The adviser team reviews the judgement calls, signs off and files. Along the way it covers the reverse charge, EU sales and the VIES statement, recovery restrictions, the reconciliation to the ledger and the return pack.

Live: [davej91.github.io/VAT-2027](https://davej91.github.io/VAT-2027/)

## Who it's for

Indirect tax practitioners, finance teams and product people who want to see what agent-assisted compliance work might look like in practice. It is meant to start a conversation, not to be used for a real return.

## What's in it

- A ten-step walkthrough: start, map, verify, classify, review, restrictions, reconcile, return, sign-off and file.
- A simulated team chat with a client view and an adviser view, plus live cursors for the cast.
- Charts, a reconciliation bridge and a printable return pack.
- A tutorial mode and a "watch the team" mode if you'd rather not click through yourself.

## Running it locally

It is a single self-contained `index.html` with no build step and no dependencies. Open it in a browser, or serve the folder:

```
python3 -m http.server 8000
```

Then go to http://localhost:8000.

## Deployment

GitHub Pages serves `index.html` from the root of the `main` branch. The `.nojekyll` file tells Pages to serve the files as they are. Every push to `main` redeploys the site.

## Caveats

- Everything is simulated. All entities, people, VAT numbers and figures are fictional, and no filing or payment ever happens.
- The page makes no network requests. Its content security policy blocks them, and fonts and icons are embedded.
- Progress is saved in your browser's local storage. Use Restart to clear it.
- Tax references are illustrative and should be checked against current Revenue guidance before relying on them.
