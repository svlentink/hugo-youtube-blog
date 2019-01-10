# hugo-youtube-blog

This hugo blog theme is 99%
[Aether](https://github.com/josephhutch/aether)
with some tweaks to optimize for youtube videos.

## Config

### Install

Create site
```shell
# https://gohugo.io/getting-started/quick-start/
hugo new site quickstart
cd quickstart
git init

```

install theme
```shell
git submodule add https://github.com/svlentink/hugo-youtube-blog themes/youtube
```

change `config.toml`
```toml
baseURL = "http://testserver.example.com/hugo/quickstart/public/"
languageCode = "en-us"
title = "My youtube channel name"
theme = "youtube"
#googleAnalytics = "Your google analytics tracking ID - optional"

[params]
brand = "Nonni-video"
#homeimg = "URL to the image used for the home button at the bottom of each post - optional"
#bgimg = "URL to the image used for the page background - optional"
```

## Page paremeters

### youtube video page

```
---
title: "Music Clip"
date: 2019-01-09T20:51:14Z
draft: false

youtubeid: "h_m-BjrxmgI"
---

some video description here, lorem ipsum

## Transcript

Hi there, welcome to another video, lorem ipsum
```

### Menu page

For a menu page,
we use `menuname` instead of `youtubeid`.

```                                                                                                                                  
---                                                                                                                                  
title: "About"                                                                                                                  
date: 2019-01-09T20:51:14Z                                                                                                           
draft: false                                                                                                                         
                                                                                                                                     
menuname: "about"                                                                                                             
---                                                                                             

