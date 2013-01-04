---
layout: post
title: "Octopressを入れてみた"
date: 2012-10-21 18:24
comments: true
categories: [octopress, blogging]
---
今まで長いこと、レンタルサーバ（[Inetd](http://inetd.co.jp/))に自分で入れた[tDiary](http://tdiary.org/)を使って日本語ブログを書いてきたのだが、どうもバージョンを3.1.1に上げたあたりからNoMemoryErrorが頻出するようになり、記事の更新がうまくできずに困っていた。最新は3.1.4だが、やはりダメである。

おそらくはtDiaryのせいではなくて、レンサバのスペックがチープなのが問題なのではないかと思うのだが（今時まだレンサバなのかよという話もある）、いずれにせよtDiaryはそろそろ潮時かなという気分もあって、このところ他のブログ・プラットフォームを物色していた。当初は[WordPress](http://wordpress.org/)にしようと思い、準備もできていたのだが、[Atsuya Takagi](http://atsuya.github.com/)さんに

{% oembed https://twitter.com/atsuya/status/258335683117215744 %}

とか煽られてやばい汁が脳内で分泌されたので、[Octopress](http://octopress.org)をちょっと試してみる気になったのである。そういえば、いつの間にか[\ay](http://arika.org/)先生もOctopressに乗り換えていた。Ruby界隈では流行りなんですかね。私はRuby使いではないのでよくわかりませんけど…。

Octopressはいわゆる静的ブログ・システムだ。基本的にリクエストがあるたびにサーバ上でウェブコンテンツを生成する普通のブログ・システムと違い、コンテンツをあらかじめ手元で整形、生成しておいて、それをサーバにアップロードするという手続きを踏む。このタイプのものは昔からいろいろあるが、個人的には以前[Nanoblogger](http://nanoblogger.org/)というのを使ったことがあって、それなりに気に入っていた。なのでなんだか懐かしい感じですね。

インストールは若干ややこしいが、Debian向けには[How to install Octopress on Debian](http://jroberthunter.net/blog/2012/05/09/how-to-install-octopress-on-debian/)が参考になった。実のところRuby 1.9xやbundlerを自前で入れる必要はない（ruby1.9.1やbundlerのdebを入れればOK）ので、あとは[本家サイトのドキュメント](http://octopress.org/docs/)を見ながらやっていけばそんなに苦労せず導入できると思う。