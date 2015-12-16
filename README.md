#Pisces

A chic Hexo theme. Written with Less and ejs.

## Demo

[demo site](http://deacyn.com)

Index page:
![](http://7xp53l.com1.z0.glb.clouddn.com/ying_mu_kuai_zhao_2015-12-16_xia_wu_8.59.16.png)
![](http://7xp53l.com1.z0.glb.clouddn.com/ying_mu_kuai_zhao_2015-12-16_xia_wu_9.11.13.png)

Post page:
![](http://7xp53l.com1.z0.glb.clouddn.com/ying_mu_kuai_zhao_2015-12-16_xia_wu_9.02.55.png)

Tag page:
![](http://7xp53l.com1.z0.glb.clouddn.com/ying_mu_kuai_zhao_2015-12-16_xia_wu_9.03.32.png)


## Features

  - Dynamically navigation menu support.
  - Tags cloud design, different frequency with different color.
  - Duoshuo comment widget, zh-CN and zh-TW support.
  - Article layout style design learn from [知乎专栏](http://zhuanlan.zhihu.com/5mlstudio).
  - Mobile-optimized
  - Beautiful cover design learn from [hexo-theme-cover]()


## Install


- Install theme:

	```
	cd your-hexo-folder
	git clone z themes/pisces
	```
- Install [hexo-renderer-less](https://github.com/hexojs/hexo-renderer-less.git)

	```
	npm install hexo-renderer-less --save
	```

## Enable

- Site setting

	In `your-hexo-folder/_config.yml`:

	```
	theme: pisces
	```
	Pisces offers three languages to select which you can find in `your-hexo-folder/themes/pisces/languages/` folder. You can set in `your-hexo-folder/_config.yml`:

	```
	i18n_dir: :lang
	# zh-CN or zh-TW or en
	language: zh-CN
	```

	More options can be checked out in [Hexo - Official Site](https://hexo.io/docs/)


- Create pages

	Pisces offers you the customized categories & tags pages.
	But you need to create these pages in `your-hexo-folder/source` folder manually.

	For instance, to create a `tags` page, you may create a `index.md` file
	at `source/tags/` folder with the following contents:

	```
	title: tags
	layout: tags
	---
	```

	And `categories` page is also similar.

- Post tips
	if you want to show different cover image in your perticular post instead of index cover image, for instance Sketch post, you need to set in your post:

	```
	layout: post
	title: Sketch
	photos:
  		- /img/IMG_001.PNG
	```


## Configuration

In `your-hexo-folder/themes/pisces/_config.yml`:

```
menu:
  home: /
  rss:
  tags: /tags
  categories: /categories

cover:
    enable: true
    url: /img/home-bg0.jpg

tags_comment:
  l: 中文名称
  l: 英文术语

categories_comment:
  l: 语言分类
  l: 粗分类


baidu_tongji: true

comment_provider: duoshuo
duoshuo:
  short_name: deacyn

nav_always: true

social:
  github: https://github.com/your_name
  weibo: https://weibo.com/your_name
  twitter: https://twitter.com/your_name
```

* **menu** - Navigation menu
* **rss** - RSS link
* **fancybox** - Enable [Fancybox](http://fancyapps.com/fancybox/)
* **comment_provider** - if you want to use duoshuo, fill your DuoShuo ID in `duoshuo.short_name`
* **baidu_tongji** - BaiduTongji ID. Supports Baidu Tongji.
* **nav_always** - Set true if you want to see the Navigation menu all the time even if you scroll the page.
* **tags_comment** - You can add some comments in tags cloud page.
* **categories_comment** - You can add some comments in categories cloud page.
* **cover** - Set cover for your site. let `cover.enable` true and write` cover.url`

## License

This theme is provided under [MIT License](http://opensource.org/licenses/MIT).




