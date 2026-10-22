# Goldcrest Plumbing & Bathrooms website

Website for Goldcrest Plumbing Ltd and Goldcrest Bathrooms Ltd, Preston.

- `index.html` – the whole site (pages switch with the menu: Home, Plumbing, Bathrooms, Our work, Reviews, About, Contact)
- `img/` – job photos
- `logo.png` – logo

Every push to `main` deploys the site to GitHub Pages automatically (`.github/workflows/deploy.yml`).

## Live Instagram posts

Near the bottom of `index.html`:

```js
window.GOLDCREST = {
  beholdFeedUrl: "https://feeds.behold.so/..."   // JSON feed URL from behold.so for @goldcrest.ltd
};
```

The Our work page loads the latest @goldcrest.ltd posts from this feed on every visit.
