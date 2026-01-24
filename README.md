# Hugo Static Site

Created with [Hugo Quick Start](https://gohugo.io/getting-started/quick-start/).  

Also installed Node `http-server` which can be used to server the static generated site.

```sh
# Run site locally
hugo server

# Run static site locally
cd public  
http-server -o public
# more info/help: http-server --help
# localhost:8080 (default port)

# Run with "draft" pages/posts
hugo server -D
# or
hugo server --buildDrafts
```

To create new content, use the `hugo new content` command:  
```sh
hugo new content posts/my-second-post.md

# or specify an archetype/kind (see archetypes/ folder)
hugo new content --kind posts post/my-post.md

# Create a new Article
hugo new content --kind articles article/creating-content.md
```

### Hugo Themes

Themes for consideration:  
* [Mainroad](https://themes.gohugo.io/themes/mainroad/) - simple, clean   
* [LoveIt](https://github.com/dillonzq/LoveIt) - elegant but advanced theme with many features including vast social medio link options
* [BeautifulHugo](https://github.com/halogenica/beautifulhugo) - mobile menu, clean layouts
* [Jane](https://github.com/xianmin/hugo-theme-jane) - decent structure and feature support, mobile menu, social links  
* [Universal](https://github.com/devcows/hugo-universal-theme) - robust feature set and capabilities
* [Hextra](https://themes.gohugo.io/themes/hextra/) looks nice; likes social media sharing

Features to consider:
* Flexible layout for Mobile
* OpenGraph meta tag support
* Blog support: posts, categories, tags, RSS feed  

If you want to pay for a theme there is [BestHugoThemes.com/](https://www.besthugothemes.com/)

