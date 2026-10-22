# Goldcrest Plumbing & Bathrooms website

Website for Goldcrest Plumbing Ltd and Goldcrest Bathrooms Ltd, Preston.

- `index.html` – the whole site (pages switch with the menu: Home, Plumbing, Bathrooms, Our work, Reviews, About, Contact)
- `img/` – job photos
- `logo.png` – logo

Every push to `main` deploys the site to GitHub Pages automatically (`.github/workflows/deploy.yml`).

## Live Google reviews and Instagram posts

Near the bottom of `index.html` there is a settings block:

```js
window.GOLDCREST = {
  googleMapsKey: "",   // Google Maps JavaScript API key, restricted to the website's address
  googlePlaceId: "",   // Google Place ID for Goldcrest Plumbing & Bathrooms
  beholdFeedUrl: ""    // JSON feed URL from behold.so for @goldcrest.ltd
};
```

Once filled in, the Reviews page shows the latest Google reviews and live rating, and the Our work page shows the latest Instagram posts. Both load live on every visit.
