---
layout: post
title: 安装jekyll失败, 解决方法
---

`$sudo gem install jekyll`

```
Building native extensions.  This could take a while...
ERROR:  Error installing jekyll:
    ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
/usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
    from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
    from extconf.rb:1:in `<main>'

```

解决：

`sudo apt-get install ruby1.9.1-dev`
