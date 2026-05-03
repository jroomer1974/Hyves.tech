# Hyves.Tech Website

A complete redesign with the look and feel of Farmforce — deep navy, lime accents,
bold typography. All pages use "Join the Hive" as the primary CTA.

## Files
- `index.html` — Homepage
- `how-we-work.html` — How We Work (4-step model + crops table)
- `projects.html` — Projects (Cacao-Tech + Citrus-Tech case studies)
- `about.html` — About (origin story, team, universities, values)
- `partner.html` — Partner page (3 audiences, contact form, process)
- `style.css` — Shared stylesheet
- `logo.jpg` — Bee logo

## To swap in real photos

The hero of `index.html` uses placeholder gradients for 3 photos. To replace
with real images:

1. Add your photos to the folder (e.g. orchard.jpg, farmer.jpg, robot.jpg)
2. In `index.html`, find the hero-photo divs and replace the class names:
   - `class="hero-photo hero-photo-1 photo-orchard"` 
     → `class="hero-photo hero-photo-1" style="background-image: url('orchard.jpg');"`

Same pattern for the case study images on the Projects page.

## Publishing on GitHub Pages

1. Create a free account at github.com
2. Create a new repository called `hyves-tech` (Public)
3. Click "uploading an existing file" → drag ALL files into the window → Commit
4. Settings → Pages → Source: main branch → Save
5. Live at: https://YOURUSERNAME.github.io/hyves-tech

## Connect your hyves.tech domain

In GitHub Pages settings, add custom domain: `hyves.tech`
At your domain registrar (where you bought hyves.tech), add these DNS records:

  Type: A    Name: @    Value: 185.199.108.153
  Type: A    Name: @    Value: 185.199.109.153
  Type: A    Name: @    Value: 185.199.110.153
  Type: A    Name: @    Value: 185.199.111.153
  Type: CNAME Name: www  Value: YOURUSERNAME.github.io

DNS changes take 1-24 hours.

## Connecting the contact form

The form on partner.html is currently visual only. To make it work:

1. Sign up free at formspree.io
2. They'll give you a form URL like https://formspree.io/f/abcXXXX
3. In partner.html, find: <button class="btn btn-primary btn-arrow" type="button">
4. Wrap the form in: <form action="https://formspree.io/f/abcXXXX" method="POST">
5. Change button to type="submit"
6. Add name="..." attributes to each input

Takes 5 minutes, requires no backend, free for low volumes.

## Things to update

- Replace team card initials (HT, VN, EC) with real names + photos
- Add real photos in the hero and project sections
- Get WUR logo added once approved
- Update Cacao-Tech project stats with real numbers when available
- Update Citrus-Tech stats once the RMIT robot is field-tested
