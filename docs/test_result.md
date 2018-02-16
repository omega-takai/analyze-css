# Execution result

I did a test run of the package. Below is a description of what type of report is done.

## Table of Contents

- [analyze-css](#analyze-css)
- [list-selectors](#list-selectors)
- [CSS Shampoo](#css-shampoo)
- [PARKER](#parker)
- [StyleStats](#stylestats)

## analyze-css

```bash
$ yarn run analyze-css node_modules/normalize.css/normalize.css
$ analyze-css --pretty --file node_modules/normalize.css/normalize.css
{
  "generator": "analyze-css v0.12.5",
  "metrics": {
    "base64Length": 0,
    "redundantBodySelectors": 0,
    "redundantChildNodesSelectors": 0,
    "colors": 0,
    "comments": 70,
    "commentsLength": 3495,
    "complexSelectors": 0,
    "duplicatedSelectors": 0,
    "duplicatedProperties": 1,
    "emptyRules": 0,
    "expressions": 0,
    "oldIEFixes": 0,
    "imports": 0,
    "importants": 0,
    "mediaQueries": 0,
    "notMinified": 1,
    "multiClassesSelectors": 0,
    "parsingErrors": 0,
    "oldPropertyPrefixes": 1,
    "propertyResets": 0,
    "qualifiedSelectors": 0,
    "specificityIdAvg": 0,
    "specificityIdTotal": 0,
    "specificityClassAvg": 0.39,
    "specificityClassTotal": 21,
    "specificityTagAvg": 0.83,
    "specificityTagTotal": 45,
    "selectors": 54,
    "selectorLengthAvg": 1,
    "selectorsByAttribute": 17,
    "selectorsByClass": 0,
    "selectorsById": 0,
    "selectorsByPseudo": 12,
    "selectorsByTag": 37,
    "length": 6052,
    "rules": 33,
    "declarations": 56
  },
  "offenders": {
    "oldPropertyPrefixes": [
      "html { -webkit-text-size-adjust: 100% } // was required by UC Browser for Android 9.9, iOS Safari 9.3 and earlier @ 13:3"
    ],
    "duplicatedProperties": [
      "abbr[title] {text-decoration: underline dotted} @ 80:3"
    ]
  }
}
✨  Done in 0.28s.
```

## list-selectors

```bash
$ yarn run list-selectors node_modules/normalize.css/normalize.css --pretty --include selectors
$ list-selectors node_modules/normalize.css/normalize.css --pretty --include selectors
{
    "selectors": [
        "::-webkit-file-upload-button",
        "a",
        "abbr[title]",
        "b",
        "body",
        "button",
        "button::-moz-focus-inner",
        "button:-moz-focusring",
        "code",
        "details",
        "fieldset",
        "h1",
        "[hidden]",
        "hr",
        "html",
        "img",
        "input",
        "kbd",
        "legend",
        "optgroup",
        "pre",
        "progress",
        "samp",
        "select",
        "small",
        "strong",
        "sub",
        "summary",
        "sup",
        "template",
        "textarea",
        "[type=\"button\"]",
        "[type=\"button\"]::-moz-focus-inner",
        "[type=\"button\"]:-moz-focusring",
        "[type=\"checkbox\"]",
        "[type=\"number\"]::-webkit-inner-spin-button",
        "[type=\"number\"]::-webkit-outer-spin-button",
        "[type=\"radio\"]",
        "[type=\"reset\"]",
        "[type=\"reset\"]::-moz-focus-inner",
        "[type=\"reset\"]:-moz-focusring",
        "[type=\"search\"]",
        "[type=\"search\"]::-webkit-search-decoration",
        "[type=\"submit\"]",
        "[type=\"submit\"]::-moz-focus-inner",
        "[type=\"submit\"]:-moz-focusring"
    ]
}
✨  Done in 0.45s.
```

## CSS Shampoo

```bash
$ yarn run csss node_modules/normalize.css/normalize.css
$ csss --files node_modules/normalize.css/normalize.css
CSSS START

Looking for muliple selectors in
node_modules/normalize.css/normalize.css

DUPLICATE: sub
    line 117
    line 125
    sharing 0 properties

DUPLICATE: sup
    line 117
    line 129
    sharing 0 properties

DUPLICATE: button
    line 152
    line 168
    line 178
    line 187
    sharing 1 property

DUPLICATE: input
    line 152
    line 168
    sharing 1 property

DUPLICATE: select
    line 152
    line 178
    sharing 1 property

DUPLICATE: textarea
    line 152
    line 253
    sharing 1 property

Duplicate selectors: 14

CSSS END
✨  Done in 0.48s.
```

## PARKER

```bash
$ yarn run parker node_modules/normalize.css/normalize.css
$ parker node_modules/normalize.css/normalize.css
PARKER-JS
Total Stylesheets: 1
Total Stylesheet Size: 6052
Total Rules: 33
Total Selectors: 54
Total Identifiers: 66
Total Declarations: 56
Selectors Per Rule: 1.6363636363636365
Identifiers Per Selector: 1.2222222222222223
Specificity Per Selector: 4.722222222222222
Top Selector Specificity: 20
Top Selector Specificity Selector: [type="button"]:-moz-focusring
Total Id Selectors: 0
Total Unique Colors: 0
Unique Colors:
Total Important Keywords: 0
Total Media Queries: 0
Media Queries:

✨  Done in 0.33s.
```

The path is executed even with 404.

## StyleStats

```bash
$ yarn run stylestats node_modules/normalize.css/normalize.css
yarn run v1.3.2
$ stylestats --prettify --format json node_modules/normalize.css/normalize.css
{
  "Published": "February 16, 2018 1:07 PM",
  "Paths": "node_modules/normalize.css/normalize.css",
  "Style Sheets": 1,
  "Style Elements": 0,
  "Size": "6.1KB",
  "Data URI Size": "0",
  "Ratio of Data URI Size": "0",
  "Gzipped Size": "1.7KB",
  "Rules": 33,
  "Selectors": 54,
  "Declarations": 56,
  "Simplicity": "61.1%",
  "Average of Identifier": "1.685",
  "Most Identifier": 4,
  "Most Identifier Selector": "[type=\"search\"]::-webkit-search-decoration",
  "Average of Cohesion": "2.606",
  "Lowest Cohesion": 12,
  "Lowest Cohesion Selector": "legend",
  "Total Unique Font Sizes": 5,
  "Unique Font Sizes": "1em\n2em\n75%\n80%\n100%",
  "Total Unique Font Families": 2,
  "Unique Font Families": "inherit\nmonospace, monospace",
  "Total Unique Colors": 0,
  "Unique Colors": "N/A",
  "Total Unique Background Images": 0,
  "Unique Background Images": "N/A",
  "ID Selectors": 0,
  "Universal Selectors": 0,
  "Unqualified Attribute Selectors": 8,
  "JavaScript Specific Selectors": 0,
  "Important Keywords": 0,
  "Float Properties": 0,
  "Properties Count": "font-size: 6\ndisplay: 5\npadding: 4\n-webkit-appearance: 4\nline-height: 3\nmargin: 3\nbox-sizing: 3\noverflow: 3\nfont-family: 3\nheight: 2",
  "Media Queries": 0
}
✨  Done in 0.49s.
```
