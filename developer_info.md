---
title: Developer Info
---

{% include menu.html %}

# Developer Info

The official Vimperator source code is hosted on
[GitHub]({{ site.data.links.github }}).
In order to work on any of our projects, you will need to get the repository first:

```
git clone https://github.com/vimperator/vimperator-labs/
```

If you don't plan to actively work on the project,
you can still [monitor changes]({{ site.data.links.github}}/commits/master)). 

## Build a Project

You can then build any vimperator labs project by doing:

```
cd vimperator-labs/<project>
make xpi
```

For example, you can build Vimperator by doing:

```
cd vimperator-labs/vimperator
make xpi
```

This will produce an XPI file in the vimperator-labs/downloads folder.

To build all applications, you can use:

```
cd vimperator-labs
make xpi
```

### Required Software to Build

- zip
- gmake, awk, sed, sh, echo 

While most developers use a Unix-like operating system, you can also build
Vimperator on Windows with the help of
[MinGW](http://www.mingw.org/)'s MSYS,
[Cygwin](http://www.cygwin.com/), or
[SFU](http://en.wikipedia.org/wiki/Microsoft_Windows_Services_for_UNIX).

## Update

 Whenever you want to update your local repository to the latest version use:

```
git pull
```

Creating and installing a new XPI file after each update is cumbersome,
therefore there is a simple way to always use the latest Vimperator version
after an update.
To do so, simply replace the
`{MY_FIREFOX_PROFILE}/extensions/vimperator@mozdev.org` *directory* with a text
file of the same name containing the full path of your vimperator/ directory.
This works analogous for the Muttator project.

## Submit Patches

We all hope that just cloning/updating the repository is not enough for you and
you start writing your own enhancements or fix some bugs.
When you think your updated code is ready send us a pull request on GitHub.

**Note:** For any new or changed feature, asciidoc documentation and an entry
in the NEWS file is **required** for the patch to be accepted.
