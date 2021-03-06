Client side live preview of Markdown for Gollum with syntax highlighting.

[Click for demo.](http://bootstraponline.github.com/livepreview/public)

Uses code/assets from:

0. [ace](https://github.com/ajaxorg/ace)
0. [gollum](https://github.com/github/gollum)
0. [jquery](https://github.com/jquery/jquery)
0. [sizzle](https://github.com/jquery/sizzle)
0. [notepages](https://github.com/fivesixty/notepages)
0. [pagedown](https://code.google.com/p/pagedown/)
0. [retina_display_icon_set](http://blog.twg.ca/2010/11/retina-display-icon-set/)
0. [debounce](https://github.com/cowboy/jquery-throttle-debounce)
0. [requirejs](https://github.com/jrburke/requirejs)

See licenses folder for details.

# Updating gollum
```
css/
images/
js/
licenses/
index.html
readme.md
```


# Dependency Notes

## Ace
Using master branch at [dbab677c413aec097bf2e7f95a9e245a4526ce88](https://github.com/ajaxorg/ace/commit/dbab677c413aec097bf2e7f95a9e245a4526ce88).

- Copy `ajaxorg/ace/lib/ace` to `/public/js/ace/lib/ace`
- `public/js/ace/lib/ace/ext/static_highlight.js` has been modified to disable gutter rendering. [#799](https://github.com/ajaxorg/ace/pull/799)
- `public/js/ace/lib/ace/theme/github.css` `public/js/ace/lib/ace/theme/github.js` are custom theme files. [#798](https://github.com/ajaxorg/ace/pull/798)

## jQuery & Sizzle
Using jQuery v1.7.2.

- Download latest production version from [jquery.com](http://www.jquery.com).

## Pagedown
The [Pagedown code](https://code.google.com/p/pagedown/source/list) used is from revision `3151a581819f39123b0b5fd1ca9e26cebdcaa873`, May 31, 2012. Markdown.Converter.js has been enhanced to support Gollum style code highlighting. Markdown.Sanitizer.js has been fixed to not remove h4-6.

https://code.google.com/p/pagedown/source/detail?r=3151a581819f39123b0b5fd1ca9e26cebdcaa873

- The h4-6 fix has been submitted for upstream inclusion. [#29](https://code.google.com/p/pagedown/issues/detail?id=29)
- livepreview has various additions to pagedown so it can't be replaced by upstream unpatched.
