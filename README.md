# oded-hexo
My all things web dev blog powered by Hexo
[doc](https://hexo.io/docs/writing.html)

### Creating a post

```bash
hexo new post "Title for post"
```

or using hexo admin

```bash
hexo server -d
open http://localhost:4000/admin/
```

viewing your post locally
```bash
hexo server
```

To deploy to Github Pages run
```bash
hexo generate # generates the public dir from the branch you are on
hexo deploy # pushes to gh-pages branch on GitHub the public dir you've just generated
```

To commit source code to Github master branch run
```bash
git push origin master
```

To commit source code to Bitbucket bitbucket branch run
```bash
git push bitbucket bitbucket
```

Incase the post is in Hebrew add to the `source/_posts/your-post.md` meta headers `language: he`.

*note that regardless of the hexo flow you need to push changes to your github repo.


### Troubleshooting

## re-setup
First make sure you have a working system environment(see later).
Here is a working configuration using node v6 and npm v3
```bash
$hexo -v
	hexo: 3.3.5
	hexo-cli: 1.0.2
	os: Darwin 16.5.0 darwin x64
	http_parser: 2.7.0
	node: 6.10.2
	v8: 5.1.281.98
	uv: 1.9.1
	zlib: 1.2.11
	ares: 1.10.1-DEV
	icu: 58.2
	modules: 48
	openssl: 1.0.2k

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

## cherry picking a commit onto another branch
on the branch you wish the commit would be added execute `git cherry-pick f3d8d47`


