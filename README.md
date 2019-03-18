# hugo-hello

## Preparation

### Install Hugo

`$ go get -u github.com/gohugoio/hugo`

### Clone hugo-hello

`$ git clone --recurse-submodules https://github.com/cary205/hugo-hello.git`

## Edit

### Add Some Content

`$ hugo new post/my-first-post.md`

### Start the Hugo server

include content marked as draft on http://localhost:1313/: 

`$ hugo server -D`

...or binding ip and port: 

`$ hugo server --bind 0.0.0.0 -p 8080`

## Deployment

### Set Worktree

`$ mkdir public`

`$ git worktree add -B gh-pages public  origin/gh-pages`

### Deployment of Project Pages From Your gh-pages branch

`$ rm -rf public/*`

`$ hugo`

`$ cd public && git add --all && git commit -m "Publishing to gh-pages" && cd ..`

`$ git push origin gh-pages`

## Ref.

[HUGO Quick Start](https://gohugo.io/getting-started/quick-start/)

[Ananke, A theme for Hugo](https://github.com/budparr/gohugo-theme-ananke)

[HUGO blog theme](https://github.com/Tazeg/hugo-blog-jeffprod)