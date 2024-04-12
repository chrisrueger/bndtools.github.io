# Bndtools.org Main Website
=====================

This repository holds the bndtools.org website hosted at [https://bndtools.org][bndtools].
This web site is maintained as markdown and turned into HTML by [Jekyll][jekyll]
using [GitHub Pages](https://help.github.com/articles/what-are-github-pages/).

## Local development

- install ruby 2.7
- call `./run.sh` on the commandline

This should install jekyll and start a local webserver at:

- http://127.0.0.1:4000/

Start editing markdown `.md` files. Jekyll will auto-detect changes and reload the website. Some changes require a restart (e.g. changes to `_config.yml`)

### CSS Styling for Code Highlighter

- jekyll uses `rouge` code highlighter
- see `_config.yml` and section `syntax_highlighter_opts`
- also see this website https://jekyll-themes.com/brazacz/rouge-themes for examples
- rouge is compatible with and can use 'pygments' styles (see https://pygments.org/styles/)
- these styles can be generated with the command 

The following commands locally will help to generate the .css files for the pygment styles:

```
gem install rouge

# show a list of supported styles
rougify help style

# go to the css folder
cd css

# generate the css
rougify style monokai > monokai.css
```

Then reference the `.css` file in `_includes/head.html `



## Feedback

Feedback is always welcome.
For general discussions use the <bndtools-users@googlegroups.com> list.
We also have the <bndtools-dev@googlegroups.com> list for discussions on the development of bndtools.

Bugs and issues for the [https://bndtools.org][bndtools] website should go to <https://github.com/bndtools/bndtools.github.io/issues>

## Contributing

Want to hack on the bndtools.org website? See [CONTRIBUTING.md](CONTRIBUTING.md) for information on building, testing and contributing changes.

They are probably not perfect, please let us know if anything feels
wrong or incomplete.

## License

The contents of this repository are made available to the public under the terms of the [Eclipse Public License v1.0](http://www.eclipse.org/legal/epl-v10.html).

[bndtools]: https://bndtools.org
[jekyll]: http://jekyllrb.com/
