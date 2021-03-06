![Moleculer logo](http://moleculer.services/images/banner.png)

# moleculer-console-tracer [![NPM version](https://img.shields.io/npm/v/moleculer-console-tracer.svg)](https://www.npmjs.com/package/moleculer-console-tracer)

Simple tracer service to print metric traces to the console. 
***Do not use it in production. Just for prototyping and testing.***

![Console Tracing screenshot](https://user-images.githubusercontent.com/306521/37969145-560ad38a-31d0-11e8-87f5-7a531181926b.png)

_Don't execute multiple instances because it is not a centralized tracing solution._

# Features

# Install

```bash
$ npm install moleculer-console-tracer
```

# Usage

```js
// services/metrics.tracer.js

const Tracer = require("moleculer-console-tracer");

module.exports = {
    mixins: [Tracer],
    settings: {
        width: 100,
        gaugeWidth: 50
    }
});

// moleculer.config.js
module.exports = {
    // ...
    metrics: true,
    // ...
}
```

<!-- AUTO-CONTENT-START:USAGE -->
<!-- AUTO-CONTENT-END:USAGE -->

<!-- AUTO-CONTENT-TEMPLATE:USAGE
{{#hasExamples}}
{{#each examples}}
{{{this}}}
{{/each}}
{{/hasExamples}}
-->



# Settings

<!-- AUTO-CONTENT-START:SETTINGS -->
| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
| `width` | `Number` | `80` | Table width. |
| `gaugeWidth` | `Number` | `40` | Gauge width. |

<!-- AUTO-CONTENT-END:SETTINGS -->

<!-- AUTO-CONTENT-TEMPLATE:SETTINGS
| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
{{#each this}}
| `{{name}}` | {{type}} | {{defaultValue}} | {{description}} |
{{/each}}
{{^this}}
*No settings.*
{{/this}}

-->

# Actions
<!-- AUTO-CONTENT-START:ACTIONS -->
<!-- AUTO-CONTENT-END:ACTIONS -->

<!-- AUTO-CONTENT-TEMPLATE:ACTIONS
{{#each this}}
## `{{name}}` {{#each badges}}{{this}} {{/each}}
{{#since}}
_<sup>Since: {{this}}</sup>_
{{/since}}

{{description}}

### Parameters
| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
{{#each params}}
| `{{name}}` | {{type}} | {{defaultValue}} | {{description}} |
{{/each}}
{{^params}}
*No input parameters.*
{{/params}}

{{#returns}}
### Results
**Type:** {{type}}

{{description}}
{{/returns}}

{{#hasExamples}}
### Examples
{{#each examples}}
{{this}}
{{/each}}
{{/hasExamples}}

{{/each}}
-->

# Methods

<!-- AUTO-CONTENT-START:METHODS -->
<!-- AUTO-CONTENT-END:METHODS -->

<!-- AUTO-CONTENT-TEMPLATE:METHODS
{{#each this}}
## `{{name}}` {{#each badges}}{{this}} {{/each}}
{{#since}}
_<sup>Since: {{this}}</sup>_
{{/since}}

{{description}}

### Parameters
| Property | Type | Default | Description |
| -------- | ---- | ------- | ----------- |
{{#each params}}
| `{{name}}` | {{type}} | {{defaultValue}} | {{description}} |
{{/each}}
{{^params}}
*No input parameters.*
{{/params}}

{{#returns}}
### Results
**Type:** {{type}}

{{description}}
{{/returns}}

{{#hasExamples}}
### Examples
{{#each examples}}
{{this}}
{{/each}}
{{/hasExamples}}

{{/each}}
-->

# Test
```
$ npm test
```

In development with watching

```
$ npm run ci
```

# License
The project is available under the [MIT license](https://tldrlegal.com/license/mit-license).

# Contact
Copyright (c) 2016-2018 MoleculerJS

[![@moleculerjs](https://img.shields.io/badge/github-moleculerjs-green.svg)](https://github.com/moleculerjs) [![@MoleculerJS](https://img.shields.io/badge/twitter-MoleculerJS-blue.svg)](https://twitter.com/MoleculerJS)
