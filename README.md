# Analyze CSS 🔎📄
For manual improvement, a report preparation tool

***

## Setup 🛠

```
$ git clone https://github.com/t--takai/analyze-css.git
$ cd analyze-css
$ yarn
```

## Running 🚀

## Stop 😇

## Build 📦

***

## Packages

### PARKER

```bash
$ yarn run parker -- {file/to/path}
```

Test result

```bash
$ curl https://raw.githubusercontent.com/necolas/normalize.css/master/normalize.css -s | parker -s
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

✨  Done in 0.76s.
```

The path is executed even with 404.

### StyleStats

```bash
$ yarn run stylestats -- {file/to/path}
```

Test result

```bash
$ stylestats path/to/stylesheet.css
StyleStats!
┌─────────────────────────────────┬──────────────────────────┐
│ Published                       │ June 14, 2017 10:35 AM   │
├─────────────────────────────────┼──────────────────────────┤
│ Paths                           │ path/to/stylesheet.css   │
├─────────────────────────────────┼──────────────────────────┤
│ Style Sheets                    │ 1                        │
├─────────────────────────────────┼──────────────────────────┤
│ Style Elements                  │ 0                        │
├─────────────────────────────────┼──────────────────────────┤
│ Size                            │ 240.0B                   │
├─────────────────────────────────┼──────────────────────────┤
│ Data URI Size                   │ 0                        │
├─────────────────────────────────┼──────────────────────────┤
│ Ratio of Data URI Size          │ 0                        │
├─────────────────────────────────┼──────────────────────────┤
│ Gzipped Size                    │ 158.0B                   │
├─────────────────────────────────┼──────────────────────────┤
│ Rules                           │ 7                        │
├─────────────────────────────────┼──────────────────────────┤
│ Selectors                       │ 12                       │
├─────────────────────────────────┼──────────────────────────┤
│ Simplicity                      │ 58.3%                    │
├─────────────────────────────────┼──────────────────────────┤
│ Average of Identifier           │ 1.250                    │
├─────────────────────────────────┼──────────────────────────┤
│ Most Identifier                 │ 3                        │
├─────────────────────────────────┼──────────────────────────┤
│ Most Identifier Selector        │ .foo .bar .baz           │
├─────────────────────────────────┼──────────────────────────┤
│ Average of Cohesion             │ 1.429                    │
├─────────────────────────────────┼──────────────────────────┤
│ Lowest Cohesion                 │ 2                        │
├─────────────────────────────────┼──────────────────────────┤
│ Lowest Cohesion Selector        │ .foo                     │
├─────────────────────────────────┼──────────────────────────┤
│ Total Unique Font Sizes         │ 2                        │
├─────────────────────────────────┼──────────────────────────┤
│ Unique Font Sizes               │ 12px                     │
│                                 │ 16px                     │
├─────────────────────────────────┼──────────────────────────┤
│ Total Unique Font Families      │ 0                        │
├─────────────────────────────────┼──────────────────────────┤
│ Unique Font Families            │ N/A                      │
├─────────────────────────────────┼──────────────────────────┤
│ Total Unique Colors             │ 3                        │
├─────────────────────────────────┼──────────────────────────┤
│ Unique Colors                   │ #333333                  │
│                                 │ #CCCCCC                  │
│                                 │ RED                      │
├─────────────────────────────────┼──────────────────────────┤
│ Total Unique Background Images  │ 0                        │
├─────────────────────────────────┼──────────────────────────┤
│ Unique Background Images        │ N/A                      │
├─────────────────────────────────┼──────────────────────────┤
│ ID Selectors                    │ 1                        │
├─────────────────────────────────┼──────────────────────────┤
│ Universal Selectors             │ 1                        │
├─────────────────────────────────┼──────────────────────────┤
│ Unqualified Attribute Selectors │ 1                        │
├─────────────────────────────────┼──────────────────────────┤
│ JavaScript Specific Selectors   │ 0                        │
├─────────────────────────────────┼──────────────────────────┤
│ Important Keywords              │ 1                        │
├─────────────────────────────────┼──────────────────────────┤
│ Float Properties                │ 1                        │
├─────────────────────────────────┼──────────────────────────┤
│ Properties Count                │ color: 4                 │
│                                 │ font-size: 3             │
│                                 │ margin: 2                │
│                                 │ float: 1                 │
├─────────────────────────────────┼──────────────────────────┤
│ Media Queries                   │ 0                        │
└─────────────────────────────────┴──────────────────────────┘
```

***

## Meaning of Emoji

| Browse                        | Emoji Code  | Mean                    |
| ----------------------------- | ----------- | ----------------------- |
| :tada: :tada: :tada:          | `:tada:`    | Celebration             |
| :toilet: :toilet: :toilet:    | `:toilet:`  | Be Minimal              |
| :octocat: :octocat: :octocat: | `:octocat:` | Function Addition       |
| :bug: :bug: :bug:             | `:bug:`     | Bug Elimination         |
| :gem: :gem: :gem:             | `:gem:`     | Refactoring             |
| :rocket: :rocket: :rocket:    | `:rocket:`  | Performance Improvement |
| :memo: :memo: :memo:          | `:memo:`    | Documentation           |
| :shit: :shit: :shit:          | `:shit:`    | Fail                    |

***

## Thanks & Resources

* **Reference**
