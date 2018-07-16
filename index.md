---
title: Projects
---

# Projects

Writing efficient user interfaces is the main maxim, here at Vimperator labs.
We often follow the [Vim](http://www.vim.org/) way of doing things,
but extend its principles when necessary.
Towards this end, we've created the liberator library for
[Mozilla](http://www.mozilla.org/) based applications,
to encapsulate as many of these generic principles as possible,
and liberate developers from the tedium of reinventing the wheel.

<div style="background-color: #ffffcc;; border-left: 6px solid #ffeb3b; padding: 0.01em 16px; margin-top: 16px; margin-bottom: 16px">
<p>
<b>NOTE:</b> Vimperator will stop functioning with Firefox 57!
</p>
<p>
Firefox 57 will change its add-on ecosystem to be exclusively based on
[WebExtensions](https://blog.mozilla.org/addons/2016/11/23/add-ons-in-2017/).
While this offers (some) compatibility with extensions written for Chrome and
Microsoft Edge, it removes the possibility to do many advanced stuff which
Vimperator does. Additionally, it would require a full rewrite of Vimperator,
which nobody has volunteered for. Therefore we will stop supporting any Firefox
version later than Firefox 56. Head over to our GitHub page for
[a list of alternatives](https://github.com/vimperator/vimperator-labs#end-of-life-and-alternatives)
or [a detailed discussion](https://github.com/vimperator/vimperator-labs/issues/705).
If you want to have famous last words, you can take a survey
[here](https://docs.google.com/forms/d/e/1FAIpQLSfTvWhTWbWAWpbbeoVM_RkDEQV6dqp4YL9Gt77gNkQHN4pTZA/formResponse)
to inspire future add-on authors what you actually liked about Vimperator
(<b>update:</b> [survey results in CSV]({{ site.url }}/assets/vimperator_exit_eol_survey.csv))
</p>
</div>

Currently, these applications are using this library:

## Vimperator (for Firefox)

![Vimperator Completion]({{ site.url }}/assets/vimperator_completions.png)

Vimperator, the flagship project from Vimperator labs,
creates a Vim-like Firefox.

[**Vimperator**]({{ site.url }}/vimperator) is a [Firefox]({{ site.data.links.firefox }}) browser
extension with strong inspiration from the [Vim]({{ site.data.links.vim }})
text editor, with a mind towards faster and more efficient browsing.
It has similar key bindings and you could call it a modal web browser,
as key bindings differ according to which mode you are in.
For example, it has a special *Hint* mode,
where you can follow links easily with the keyboard only.
Also most functionality is available as commands,
typing `:back` will go back within the current page history,
just like hitting the back button in the toolbar.

## Muttator (for Thunderbird)

![Muttator Minimal]({{ site.url }}/assets/muttator_minimal.png)

Muttator is to Thunderbird what Vimperator is to Firefox.
Combines the best aspects of Vim and Mutt.

[**Muttator**]({{ site.url }}/muttator) is a free add-on for the
[Thunderbird]({{ site.data.links.thunderbird }}) mail client,
which makes it look and behave like the [Vim]({{ site.data.links.vim }}) text editor.
It has similar key bindings and you could call it a modal mail client,
as key bindings differ according to which mode you are in.
For example, the same keys can select the next message while the message list
has focus or can scroll down an existing message when the message preview is
selected.
It also adds commands for accessing most Thunderbird functionality.
E.g., `:contact -lastname "Vimperator" vimperator@mozdev.org` will add
Vimperator's mailing list to your address book.

## Vimium (for Chrome)

[Vimium](https://vimium.github.io/) is a Google Chrome extension written by
[Phil Crosby](http://philc.co/) and [Ilya Sukhar](http://ilya.sukhar.com/) which
provides keyboard shortcuts for navigation and control in the spirit of the Vim
editor.
Due to limitations of the Chrome extension mechanism,
it is not as powerful as Vimperator but is still considered the best
Vimperator-like extension for Chrome.

## Vrapper (for Eclipse)

[Vrapper](http://vrapper.sourceforge.net/home/) is an Eclipse plugin which acts
as a wrapper for Eclipse text editors to provide a Vim-like input scheme for
moving around and editing text.

Unlike other plugins which embed Vim in Eclipse,
Vrapper imitates the behaviour of Vim while still using whatever editor you have
opened in the workbench.
The goal is to have the comfort and ease which comes with the different modes,
complex commands and count/operator/motion combinations which are the key
features behind editing with Vim,
while preserving the powerful features of the different Eclipse text editors,
like code generation and refactoring.

## VsVim (for VisualStudio)

[VsVim](https://marketplace.visualstudio.com/items?itemName=JaredParMSFT.VsVim)
is a Vim Emulation layer for Visual Studio 2010 and above.
It integrates the familiar key binding experience of Vim directly into
Visual Studio's editor.

## Get involved

For now, we have just focused on these three Mozilla applications because of
time constraints.
If you want other host applications like
[Instantbird](http://www.instantbird.com/) or
[Sunbird](http://www.mozilla.org/projects/calendar/sunbird/)
to make use of our liberator library, feel free to [contact us]({{ site.data.links.contact_email }}).
