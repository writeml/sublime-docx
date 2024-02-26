# The *python-docx* module for Sublime Text plugins

![tag](https://img.shields.io/github/tag/writeml/sublime-docx.svg)
![pypi](https://img.shields.io/pypi/v/python-docx.svg)

> [!IMPORTANT]
> This distribution is paused at v0.8.11, which is the most recent version to
> still support Python v3.3. As of Package Control v4, newer versions of this
> library -- which support newer versions of Python -- are pointed directly to
> their official release packages at PyPI.
>
> It is highly recommended that you update your Sublime Text plugins to target
> the most recent version of Python possible (v3.8 as of Feb 2024). See
> [the Sublime Text API - Python Version documentation](https://www.sublimetext.com/docs/api_environments.html#python-version)
> for more (and the most recent) infomation.

This is the *python-docx* module bundled as a
[Package Control](https://packagecontrol.io) dependency for use by
[Sublime Text](https://www.sublimetext.com) plugins.

  - [*python-docx* @ GitHub](https://github.com/python-openxml/python-docx)
  - [*python-docx* @ PyPI](https://pypi.org/project/python-docx/)
  - [*python-docx* @ Read the Docs](https://python-docx.readthedocs.io)

## How to use this dependency

In order to tell Package Control that your plugin requires the *python-docx*
module, create a `dependencies.json` file in your plugin root with the
following contents:

``` json
{
   "*" : {
      ">=3000" : [
         "lxml",
         "python-docx"
      ]
   }
}
```

Note that *python-docx* requires the [*lxml*](https://pypi.org/project/lxml)
module, which is hosted as its own Package Control dependency
[here](https://github.com/eerohele/sublime-lxml). Be aware also that this
dependency may have its own platform/version restrictions.

Once you have your `dependencies.json` file in place, you can then run the
`Package Control: Satisfy Dependencies` command in Sublime Text, which will tell
Package Control to download and install these dependencies. Once that's
finished, you will then be able to use any *python-docx* `import` directives you
may need, such as `from docx import Document`.

See also:
[Documentation on Dependencies](https://packagecontrol.io/docs/dependencies)