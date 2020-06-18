## Blog Website

This is a blogging website based on this jekyll [theme](https://github.com/brianmaierjr/long-haul)

### Building

```docker
docker run --rm \
--volume="$PWD:/srv/jekyll" \
-it jekyll/jekyll:3.8 \
jekyll build
```

### Serving

```docker
docker run \
--name newblog \
--volume="$PWD:/srv/jekyll" \
-p 3000:4000 \
-it jekyll/jekyll:3.8 \
jekyll serve --watch --drafts

```
