# Release a new version

## Releases 
Find SHA [here](https://www.ruby-lang.org/en/news/2022/04/12/ruby-2-7-6-released/)
Update env vars in `Dockerfile`

Then build image and push it

```shell
# To list platforms available
docker buildx ls 
docker buildx build --platform linux/amd64 -t prettotech/ruby-jemalloc:x.x.x .
docker login -u prettotech 
> enter pw in 1password
docker push prettotech/ruby-jemalloc:x.x.x
```

