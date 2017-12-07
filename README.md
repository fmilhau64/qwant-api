# Qwant API

<p align="center">
<img height="150" width="auto" src="https://www.qwant.com/favicon.png" /><br>
Unofficial API wrapper for qwant
</p>

## :postbox: NPM

[![](https://nodei.co/npm/qwant-api.svg?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/qwant-api)

<hr>

## :wrench: Installation

```Assembly
npm i qwant-api
```

<hr>

## :white_check_mark: Features

Qwant Feature support
  
| web | images | news | social |
| :---: | :---: | :---: | :---: |
| :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |

<hr>

## :bulb: Usage

```javascript
qwant.search(<category>, { <options> }, <callback>{ /*...*/ });
```

**Categories:**

- web
- images
- news
- social

**Options:**

| Option | Required | Type | Default | Explanation |
|--------|----------|------|---------|-------------|
| query | **Yes** | string | none | The term(s) to search |
| count | no | integer | 1 | The ammount of results |
| offset | no | integer | 0 | The index of the first result |

**Example:**

```Javascript
var qwant = require("qwant-api");

qwant.search("web", { query: "test", count: 10, offset: 1 }, function(err, data){
    if (err) return console.log(err);
    console.log(data);
});
```

<hr>

## :nut_and_bolt: Dependencies

- [request](https://www.npmjs.com/package/request)

<hr>

## :clipboard: TODO:

Everything.

<hr>

## :copyright: Copyright & Disclaimer

`Copyright (c) 2017 NullDev`

This is **NOT** an official API Wraper for [Qwant](http://qwant.com).
