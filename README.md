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
