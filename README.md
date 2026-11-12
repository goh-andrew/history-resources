# history-resources

Study games for IGCSE History (China). Open `index.html` to pick a game.

## Online rooms for Croissant Bomb

One-device mode works with no setup. Online rooms need a free Firebase Realtime Database (about 5 minutes, once):

1. Go to [console.firebase.google.com](https://console.firebase.google.com), add a project (you can turn Analytics off).
2. In the left menu open **Build > Realtime Database**, click **Create database**, pick a location, and start in **locked mode**.
3. Open the database's **Rules** tab, replace everything with the contents of `database.rules.json`, and click **Publish**.
4. Open **Project settings** (gear icon) > **Your apps**, click the web icon `</>`, register an app, and copy the `firebaseConfig` values into `firebase-config.js`. Check that `databaseURL` is filled in.
5. Commit and push. On the site, one person picks **Online room > Create a room** and shares the four-letter code or invite link.

The free Spark plan allows 100 people connected at once, which is plenty for a class. The host's browser runs the game, so if the host closes the tab the room ends.
