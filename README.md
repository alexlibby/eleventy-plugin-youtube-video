# Eleventy YouTube Plugin

An [11ty](https://www.11ty.dev/) plugin that displays a selected YouTube video on the page.

- [Installation](#installation)
- [Usage](#usage)
- [Output](#output)
- [Licence](#licence)


## Installation

```shell
npm install eleventy-plugin-youtube-video
```


## Usage

In your [Eleventy config file](https://www.11ty.dev/docs/config/) (`.eleventy.js` by default):
```js
const youTube = require('eleventy-plugin-youtube-video');

module.exports = function(eleventyConfig) {
  eleventyConfig.addPlugin(youTube);
}
```

Then, depending on your template engine (Liquid by default) insert the shortcode into your post as follows

```
// Liquid (.liquid) or Nunjucks (.njk):
{% youtube 'ix5mPa6D7ZA', 'YouTube Video' %}
```
- where:
```
- ix5mPa6D7ZA    : take this from the v= part of any YouTube video url, i.e. https://www.youtube.com/watch?v=ix5mPa6D7ZA
- 'YouTube Video': the caption for the video, set to appear underneath in the center.
```

## Output:
![image](https://user-images.githubusercontent.com/16504949/147837765-8103b4ad-3673-4023-ac37-5c294f76c575.png)

## Licence
[MIT](https://choosealicense.com/licenses/mit/)
