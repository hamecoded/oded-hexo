# oded-hexo
My all things web dev blog powered by Hexo
[doc](https://hexo.io/docs/writing.html)

### Creating a post

```bash
hexo new post "Title for post"
```
viewing your post locally
```bash
hexo server
```

To deploy to Github run
```bash
hexo generate
hexo deploy
```

Incase the post is in Hebrew add to the `source/_posts/your-post.md` meta headers `language: he`.

*note that regardless of the hexo flow you need to push changes to your github repo.


### Troubleshooting

## re-setup
First make sure you have a working system environment(see later).
Here is a working configuration using node v6 and npm v3
```bash
$hexo -v
	hexo: 3.2.2
	hexo-cli: 1.0.2
	os: Darwin 14.5.0 darwin x64
	http_parser: 2.7.0
	node: 6.3.1
	v8: 5.0.71.57
	uv: 1.9.1
	zlib: 1.2.8
	ares: 1.10.1-DEV
	icu: 57.1
	modules: 48
	openssl: 1.0.2h

	npm: 3.10.3
```

If you wish to upgrade you can use the ``ncu`` command through module [npm-check-updates](https://www.npmjs.com/package/npm-check-updates)

```bash
	rm -rf node_modules
	npm install --no-optional 

```

Incase you'll need to update npm
```bash
sudo npm i -g npm
```

or maybe just reinstall hexo
```bash
npm install hexo --no-optional --save
```
## a working system environment

you'll need npm (node v6 lts) and hexo-cli `npm install -g hexo-cli`
