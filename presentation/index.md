---
title       : Energy Consumption
subtitle    : In my renovated house
author      : Bakhouz
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      #
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Description

The Shiny App I wrote displays energy consumption information:

- gas
- electricity
- water

for the years 2012 to 2014.

---
## Details

Every Sunday, I write down in an Excel sheet the figures displayed by the
different meters.

These data are diffed, week by week, so that I get the week's consumption.

Further more, a formula is applied to compute an estimate price (expressed in
EUR) for the week's consumption.

---
## Example

Here are the first 10 lines of the Excel file (for the columns which interest
me, the ones I show in the barplot):


```
## Warning in file(file, "rt"): cannot open file 'C:/Users/abakhouz/Documents/
## src/refcard-R/course-project/consumption.csv': No such file or directory
```

```
## Error in file(file, "rt"): cannot open the connection
```

```
## Error in subset.default(data, select = c(Date, PriceGas, PriceElec, PriceWater)): argument "subset" is missing, with no default
```

---
## Lessons learned

- Necessary to use reactive function as soon as I have 2 inputs or more.

- In the renderPlot function, the name of the dataframe must be followed by
  parentheses.

---
## Conclusion

- Writing the application + these slides took me around 3 hours.
  That's pretty excellent for making such a huge work available (displayable,
  testable) by third parties.  A wonder, in fact.

- With these R technologies, I really feel I stand on the shoulders of giants.
