# LFN Lawncare Services

Single page site for a kid-run lawn care and snow removal crew in South Grandview,
Dubuque IA. Liam, Finn and Nolan.

**Names are always listed Liam, Finn, Nolan** (matching L-F-N) so no one is first.
Do not reorder them.

## What it is

One `index.html`. No build step, no dependencies, no framework. Fonts load from
Google Fonts, everything else is inline.

The page has a **season switch** in the header. It flips the whole thing between
summer mowing and winter snow removal: 36 strings of copy, the service icons, the
hero animation, the palette and the logo ribbon. It opens on the real season
automatically, November through March defaults to snow.

## Deploy

Netlify, publish directory `.`. Push to `main` and it redeploys.

## The form

Netlify Forms, form name `lfn-mow-request`.

- Honeypot field: `bot-field`
- Hidden `season` field records whether the visitor was looking at mowing or snow
- Submits over fetch so the page can show its own confirmation instead of
  bouncing to Netlify's default success page
- Submissions email an adult for review. Kids never see raw submissions.

## Privacy

First names only. No kid phone numbers, no addresses, no photos. Every contact
routes through the form, which an adult manages. Keep it that way.

## Assets

`assets/logo-summer.svg` and `assets/logo-winter.svg`. Letterforms are drawn as
paths, so both scale and print with no font installed. Good for yard signs and
shirts.

## Colors

Ink `#2B2118` · Cream `#FFF6DF` · Sun `#FFD23F` · Tomato `#E8543F` · Grass
`#3FA34D` / `#7ED957`
Winter: Ice `#9AD4F5` · Deep blue `#2E6FA7` · Snow `#FFFFFF` · Pale sky `#E8F4FD`

Type: Fredoka headings, Nunito body, Caveat handwriting.

## Prices as built

Summer: $30 small, $45 medium, $60 big. $10 off a new neighbor's first cut.
Winter: $15 walks and steps, $30 driveway, $45 both. Salt +$5. Six inches or more
is double.

Spring and fall cleanup (shown in both seasons, not part of the season switch):
priced per job by the bags actually filled. $20 per bag (Ricky's call), $20 per
bundle of sticks, $40 smallest job (two bags). The crew quotes a guess on the callback and adjusts these numbers
as they learn how long jobs take.

Cost-of-goods math for reference (this came to about $9 a bag, so $20 leaves room
for learning and slow jobs): about $2.50 of goods per bag
(30 gallon paper bag about $0.50 to $0.80 plus the $1.75 City of Dubuque yard waste
sticker), plus labor of $75 an hour for the crew divided by an assumed 12 bags an
hour, about $6.25. A bundle of sticks costs about $3.50 in goods (brush tie plus
sticker). The 12 bags an hour and $75 an hour are assumptions. Time the first few
jobs and update this. Re-check City sticker and tie prices each season.

The city only takes paper bags with a yellow sticker, 40 pounds max, and brush
bundles 3 inches thick or less. Set out for the regular city yard waste day, April
through November.

## Links

Printed material links to `/?season=winter#book`. `?season=winter|summer` forces the
season, otherwise the month decides.
