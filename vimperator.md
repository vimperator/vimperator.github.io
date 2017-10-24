---
title: Vimperator
---

# Vimperator

**Vimperator** is a [Firefox]({{ site.data.links.firefox }}) browser extension
with strong inspiration from the [Vim]({{ site.data.links.vim }}) text editor,
with a mind towards faster and more efficient browsing.
It has similar key bindings and you could call it a modal web browser,
as key bindings differ according to which mode you are in.
For example, it has a special *Hint* mode,
where you can follow links easily with the keyboard only.
Also most functionality is available as commands,
typing `:back` will go back within the current page history,
just like hitting the back button in the toolbar.

However, Vimperator does not try to be a 100% Vim clone,
it rather brings Vim's ideas to the 21st century.
This means making use of new graphical capabilities but also of faster computers.
Furthermore, great care is taken into making its command line interface more
consistent and easier to use,
while still being a powerful extension for advanced users.

But Vimperator is more than just a simple command interface to Firefox —
it is a complete development environment as well.
If you are a web developer, you can enjoy an interactive JavaScript shell —
even with completion support.
Or if you want to extend Vimperator,
you can easily do that by just dropping a JavaScript file in its plugin
directory. Browse through our [wiki]({{ site.data.links.wiki}}) pages for nice
tips to customize Vimperator and for
[frequently asked questions]({{ site.data.links.faq }}).
If you have more questions, you can visit us on IRC,
in #vimperator on [freenode](http://www.freenode.net/).

## Credits

Vimperator was initially written by Martin Stubenschrott and has found many
[invaluable contributers]({{ site.data.links.github }}/graphs/contributors)
who helped out fixing bugs and adding new features. 

If you appreciate the work on Vimperator and want to encourage us working on it
more, you can send us greetings, patches, or donations:

[![Make a Donation]({{ site.url }}/assets/paypal_donations.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=8323006)
[![Make a Donation]({{ site.url }}/assets/flattr_donations.png)](http://flattr.com/thing/146785/Vimperator)

If you rather prefer getting some nice products for your money,
you can also support us by buying some cool
[merchandise](http://www.zazzle.com/maxauthority*) like t-shirts or mugs.
Of course, as we believe in free, open source software,
only support us financially if you really like Vimperator and the money doesn't
hurt — otherwise just use it, recommend it and like it :) 

## Download

<div style="background-color: #ffffcc;; border-left: 6px solid #ffeb3b; padding: 0.01em 16px; margin-top: 16px; margin-bottom: 16px">
<p>
<b>NOTE:</b> Vimperator will stop functioning with Firefox 57!
</p>
<p>
Firefox 57 will change its add-on ecosystem to be exclusively based on <a
href="https://blog.mozilla.org/addons/2016/11/23/add-ons-in-2017/">WebExtensions</a>.
While this offers (some) compatibility with extensions written for Chrome and
Microsoft Edge, it removes the possibility to do many advanced stuff which
Vimperator does. Additionally, it would require a full rewrite of Vimperator,
which nobody has volunteered for. Therefore we will stop supporting any Firefox
version later than Firefox 56. Head over to our GitHub page for <a
href="https://github.com/vimperator/vimperator-labs#end-of-life-and-alternatives">a
list of alternatives</a> or <a
href="https://github.com/vimperator/vimperator-labs/issues/705">a detailed
discussion</a>.
If you want to have famous last words, you can take a survey <a
href="https://docs.google.com/forms/d/e/1FAIpQLSfTvWhTWbWAWpbbeoVM_RkDEQV6dqp4YL9Gt77gNkQHN4pTZA/formResponse">here</a>
to inspire future add-on authors what you actually liked about Vimperator.
</p>
</div>


Downloads are hosted on the official Firefox Add-ons repository at
[addons.mozilla.org](https://addons.mozilla.org/en-US/firefox/addon/vimperator/),
where you can always find the latest version:

{% include button.html name="Download Vimperator" link=site.data.links.download %}

[Release Notes](https://raw.githubusercontent.com/vimperator/vimperator-labs/master/vimperator/NEWS) |
[Other Versions](https://addons.mozilla.org/en-US/firefox/addon/vimperator/versions/) |
[Source Code]({{ site.data.links.github }})

## Features

- Vim-like key bindings (`h`, `j`, `k`, `l`, `gg`, `G`, `0`, `$`, `ZZ`, `<C-f>`, etc.)
- Ex commands (`:quit`, `:open www.foo.com`, ...) with a proper command line
- Tab completion available for all commands, showing suggestions while you type
- Hint mode (start with `f` to follow a link)
- Extensions! Yes, you can extend Vimperator's functionality with [scripts](http://vimpr.github.io/) just like you can extend Firefox with extensions
- Explore JavaScript objects with `:echo window` and even context-sensitive tab completion
- Easily customizable GUI (easily hide all GUI elements with `:set gui=`)
- Ability to `:source` JavaScript files, and to use a `~/.vimperatorrc` file with syntax highlighting if you install [vimperator.vim](https://github.com/vimperator/vimperator.vim)
- Easy quick searches (`:open foo` will search for "foo" in google, `:open ebay terminator` will search for "terminator" on eBay) with support for Firefox keyword bookmarks and search engines
- Count supported for many commands (`3<C-o>` will go back 3 pages)
- Beep on errors
- Marks support (`ma` to set mark 'a' on a webpage, `'a` to go there).
- QuickMarks support (quickly go to previously marked web pages with `go{a-zA-Z0-9}`).
- `:map` and `:command` support (and `feedkeys()` for script writers).
- `:time` support for profiling
- Move the text cursor and select text with Vim keys and a visual mode
- External editor support
- Macros to replay key strokes
- AutoCommands to execute action on certain events
- A comprehensive `:help` system, explaining all commands, mappings and options
- Much more...

## Screenshots

[![Vimperator Hints]({{ site.url }}/assets/vimperator_hints.png)]({{ site.url }}/assets/vimperator_hints.png)
Hints allow to follow links with the keyboard

[![Vimperator Completion]({{ site.url }}/assets/vimperator_completions.png)]({{ site.url }}/assets/vimperator_completions.png)
Vimperator's completion system 

[![Vimperator Javascript]({{ site.url }}/assets/vimperator_javascript.png)]({{ site.url }}/assets/vimperator_javascript.png)
Exploring the DOM of the web page

## Scripts

While Vimperator offers already lots of cool features,
we cannot and don't want to include every feature directly in the core.
Therefore a motivated group of hackers called [vimpr](http://vimpr.github.io/)
provides many enhancements for the Vimperator experience.
You can add [plugins](https://github.com/vimpr/vimperator-plugins) which add
new commands or mappings.
Install these plugins by copying them to the **~/.vimperator/plugin/**
directory (or **%HOME%\vimperator\plugin** on Windows) unless noted differently.

If you don't care about features but just use Vimperator for the sexy looks,
you can also theme that by using color schemes.
You can install them by copying them to the **~/.vimperator/colors/** directory
(**%HOME%\vimperator\colors** on Windows) and use it with `:colorscheme <name>`.

## Bugs

Unexpected features - sometimes also called bugs - are listed in our
[issue tracker](https://github.com/vimperator/vimperator-labs/issues).
You can also file feature requests there.
