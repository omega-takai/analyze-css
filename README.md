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

### Package - PARKER

```bash
$ yarn run parker -- {file/to/path}
```

Test result

```bash
$ yarn run parker -- node_modules/normalize.css/normalize.css
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

### Package - StyleStats

```bash
$ yarn run stylestats -- {file/to/path}
```

Test result

```bash
$ yarn run stylestats -- node_modules/normalize.css/normalize.css
$ stylestats -p node_modules/normalize.css/normalize.css
 StyleStats!
┌─────────────────────────────────┬────────────────────────────────────────────┐
│ Published                       │ February 15, 2018 12:48 PM                 │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Paths                           │ node_modules/normalize.css/normalize.css   │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Style Sheets                    │ 1                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Style Elements                  │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Size                            │ 6.1KB                                      │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Data URI Size                   │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Ratio of Data URI Size          │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Gzipped Size                    │ 1.7KB                                      │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Rules                           │ 33                                         │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Selectors                       │ 54                                         │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Declarations                    │ 56                                         │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Simplicity                      │ 61.1%                                      │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Average of Identifier           │ 1.685                                      │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Most Identifier                 │ 4                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Most Identifier Selector        │ [type="search"]::-webkit-search-decoration │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Average of Cohesion             │ 2.606                                      │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Lowest Cohesion                 │ 12                                         │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Lowest Cohesion Selector        │ legend                                     │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Total Unique Font Sizes         │ 5                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Unique Font Sizes               │ 1em                                        │
│                                 │ 2em                                        │
│                                 │ 75%                                        │
│                                 │ 80%                                        │
│                                 │ 100%                                       │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Total Unique Font Families      │ 2                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Unique Font Families            │ inherit                                    │
│                                 │ monospace, monospace                       │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Total Unique Colors             │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Unique Colors                   │ N/A                                        │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Total Unique Background Images  │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Unique Background Images        │ N/A                                        │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ ID Selectors                    │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Universal Selectors             │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Unqualified Attribute Selectors │ 8                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ JavaScript Specific Selectors   │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Important Keywords              │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Float Properties                │ 0                                          │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Properties Count                │ font-size: 6                               │
│                                 │ display: 5                                 │
│                                 │ padding: 4                                 │
│                                 │ -webkit-appearance: 4                      │
│                                 │ line-height: 3                             │
│                                 │ margin: 3                                  │
│                                 │ box-sizing: 3                              │
│                                 │ overflow: 3                                │
│                                 │ font-family: 3                             │
│                                 │ height: 2                                  │
├─────────────────────────────────┼────────────────────────────────────────────┤
│ Media Queries                   │ 0                                          │
└─────────────────────────────────┴────────────────────────────────────────────┘
✨  Done in 0.64s.
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
