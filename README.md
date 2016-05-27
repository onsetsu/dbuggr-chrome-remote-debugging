# dbuggr-chrome-remote-debugging
Testing Chrome's remote debugging protocol and facilities 

---

## setting up a basic example
- `clone` this repo
- navigate to that local repo in console
- install the node-inspector npm package with `npm install node-inspector --save`
- according to [this chromium blog post](http://blog.chromium.org/2011/05/remote-debugging-with-chrome-developer.html) start chrome with remote debugging enabled "PATH\TO\YOUR\chrome.exe" --remote-debugging-port=9222 --user-data-dir=remote-profile`
- Navigate this chrome instance to the page you want to debug
- Start another chrome instance regularly and navigate it to http://localhost:9222
- The links there represent all pages, service worker and plugins running on the chrome to debug
  - choose the page you want to debug

Probably should continue by starting to look into [Blink DevTools](http://www.chromium.org/blink).
