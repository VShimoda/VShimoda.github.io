---
layout: post
title:  "First Commit"
date:   2017-05-04 22:25:58 +0900
categories: jekyll github
---

# First Commit

初めてのgithub pagesです。  
ゆるゆるとblogとして、その週にあったことを書き溜めていきたいと思います。  
私の所感も多いに混ざるのでお読みになる方は注意してください。

## Github Pages

調べる限りでは、Privateにできないようです。
> Organizationとして組織内の人間だけに知らせたいということであれば、この機能は使えないのであしからず。

内部的には [jekyll](https://jekyllrb-ja.github.io/) を使用しているとのことです。
> 公開前にjekyllでローカル確認できます。jekyllはgemなのでruby製ですね。
> 普段ruby使わないのでアレコレ言わないですが、bundlerが実行されるようで、  
> プラグインの管理なんかもそっちでやれるのかも。  

### Jekyll ディレクトリ構成

```
.
├── _config.yml
├── _drafts
|   ├── begin-with-the-crazy-ideas.textile
|   └── on-simplicity-in-technology.markdown
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-why-every-programmer-should-play-nethack.textile
|   └── 2009-04-26-barcamp-boston-4-roundup.textile
├── _data
|   └── members.yml
├── _site
└── index.html
```
[ここ](http://jekyllrb-ja.github.io/docs/structure/)に書いてあるのですが、基本的に使うところは限られているので、サクッと紹介すると

* _config.yml
  > ここで設定情報色々代える。名前とかblogタイトルとか

* _posts
  > blog投稿するとこで、YYYY-MM-DD-title.extで、私の場合、markdownなので、.extは.mdです。


### Github pagesへの投稿

github pagesはちょっと普通と違ってbranchをgh-pagesとしてここにdeployするようです。
こうすることによってgithub pages用の内容とcodeを分けれるのだとか

