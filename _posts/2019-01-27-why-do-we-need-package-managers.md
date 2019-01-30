---
title: Why do we need package managers?
layout: post
---

When programming, we don't need to reinvent the wheel every time. In order words, if something has
been done before, we don't need to write the same code again to do the same thing. We can just use the
previously written code. These libraries are well tested so they have less bugs and faster performance.

Package managers come into play to keep track of our external libraries.

For example, for NPM ( node package manager ) uses package.json to keep track of external libraries.
When you execute `npm install [package-name]` inside the terminal, NPM will add the package name to `package.json` along with the version and
install it inside the `node_modules` package.

Then, the `node_modules` folder is ignored inside `.gitignore` so that the `node_modules` folder
doesn't get pushed to Github. We don't want to push external libraries to Github.

Now, if someone clones your code to their device, all they have to do is run `npm install` and NPM will install the required package from `package.json`.

I gave NPM as an example, but other package managers work in a similar way.
