DAILY FUEL — USDA CONNECTED UPDATE

Upload/replace these three files in the ROOT of your existing GitHub repository:
- index.html
- manifest.json
- sw.js

Then commit the changes and open https://gabracero-mambo.github.io/Daily.Fuel/ in your browser.

The app now searches your Cloudflare Worker:
https://daily-fuel.gabracero.workers.dev/search?q=FOOD_NAME

Important:
- The USDA API key is NOT in these files. It stays in Cloudflare as the USDA_API_KEY secret.
- This requires your Cloudflare Worker code to be deployed and to allow the origin https://gabracero-mambo.github.io.
- If the app still shows the old version, refresh the page. If needed, close and reopen it so the service worker updates.
- Common foods may show built-in estimates first; the USDA results appear when the online search completes.
- USDA entries can differ for raw/cooked foods and brands. Check the selected match and package label.
- Food diary records remain in browser local storage. Do not upload personal backup JSON files to GitHub.
