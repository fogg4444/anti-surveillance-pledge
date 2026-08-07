# No Mass Surveillance Pledge

A Jekyll site asking city council members and candidates in Contra Costa County
to commit, in writing, to keeping mass surveillance out of their cities.

## Run it locally

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000/anti-surveillance-pledge/

## Publish it

Push to `main`, then in the repo go to **Settings → Pages** and set
**Source: Deploy from a branch**, **Branch: main / (root)**.
The site appears at `https://fogg4444.github.io/anti-surveillance-pledge/`.

## Before launch — things to replace

- `_config.yml` — `contact_email`, and `form_url` if you use a Google Form or Tally form for signatures
- `_data/officials.yml` — delete the SAMPLE rows, add real cities and real people only after you've contacted them
- `about.html` — the two `[PLACEHOLDER]` blocks
- `index.html` — the "Why no exceptions" section should cite two or three
  specific, linked, verifiable incidents before this goes public

## Adding someone to The Record

Edit `_data/officials.yml`. `status` is one of `signed`, `declined`, `silent`, `pending`.

## Custom domain

Add a `CNAME` file containing the domain, set `url` to the domain in `_config.yml`,
and set `baseurl` to `""`.
