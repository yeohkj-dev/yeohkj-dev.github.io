# 🐻 Pocket Penny – free expense tracker for Android

A cute, simple expense tracker that installs on your Android home screen, works offline,
and exports your records to CSV. No account, no ads, data stays on your phone.

## Features
- Add expenses and income: amount, category (emoji icons), date, note
- Tap any record to edit or delete it
- Monthly view with Expenses / Income / Balance totals, records grouped by day
- Stats tab: donut chart and per-category breakdown
- Export to CSV (this month, or everything) – save to Downloads or share to Drive / email / WhatsApp
- Import a Pocket Penny CSV back (backup restore; duplicates are skipped)
- Manage categories: add, rename, change icon, remove; set your currency symbol
- Works fully offline after the first load
- Optional Google Drive sync between phones (private app folder in your own Drive)

CSV columns: `Date, Type, Category, Amount, Currency, Note` (UTF-8, opens in Excel and Google Sheets).

## Put it on your phone (free)

Live at https://yeohkj-dev.github.io

1. Open that link in **Chrome on your Android phone**.
2. Tap the ⋮ menu → **Add to Home screen** / **Install app**.

For a real `.apk`, paste the link into https://www.pwabuilder.com and choose **Android**.
Then add the generated `assetlinks.json` to `.well-known/` in this repo.

## Run it on your computer

```
python -m http.server 8781 --directory pocket-penny
```
then open http://localhost:8781

## Important
Your data lives in the browser storage of the phone. Uninstalling the app or clearing Chrome's
site data deletes it – export a CSV now and then as a backup.
