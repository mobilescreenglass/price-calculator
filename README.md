# Price Calculator

A web page that shows the sale price needed to hit a 55% gross margin.

The employee enters:
- Material cost ($)
- Labor hours (per man)

## Assumptions (fixed in the code)
- 2 men work on every project.
- Each man is paid $30 per hour.
- Labor hours entered are per man. 3 hours entered = 6 total labor hours = $180 labor cost.
- Gross margin target is 55% of the sale price.

## Formula
```
labor cost = hours x 2 men x $30
total cost = material cost + labor cost
sale price = total cost / 0.45, then rounded to the nearest $5
```

Example: $100 materials, 3 hours -> ($100 + $180) / 0.45 = $622.22 -> shown as $620

## Changing the assumptions
Edit the three constants (`MEN`, `RATE`, `MARGIN`) near the bottom of `index.html`, then commit and push. Update this README to match.

## Hosting
GitHub Pages, served from the `main` branch root.
