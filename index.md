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

Currently, these applications are using this library:

## Vimperator

![Vimperator Completion]({{ site.url }}/assets/vimperator_completions.png)

Vimperator, the flagship project from Vimperator labs,
creates a Vim-like Firefox.

**Vimperator** is a [Firefox]({{ site.data.links.firefox }}) browser
extension with strong inspiration from the [Vim]({{ site.data.links.vim }})
text editor, with a mind towards faster and more efficient browsing.
It has similar key bindings and you could call it a modal web browser,
as key bindings differ according to which mode you are in.
For example, it has a special *Hint* mode,
where you can follow links easily with the keyboard only.
Also most functionality is available as commands,
typing `:back` will go back within the current page history,
just like hitting the back button in the toolbar.

## Muttator

![Muttator Minimal]({{ site.url }}/assets/muttator_minimal.png)

Muttator is to Thunderbird what Vimperator is to Firefox.
Combines the best aspects of Vim and Mutt.

**Muttator** is a free add-on for the
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

## Get involved

For now, we have just focused on these three Mozilla applications because of
time constraints.
If you want other host applications like
[Instantbird](http://www.instantbird.com/) or
[Sunbird](http://www.mozilla.org/projects/calendar/sunbird/)
to make use of our liberator library, feel free to [contact us]({{ site.data.links.contact_email }}).
