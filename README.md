# *python-docx* module for Sublime Text packages

**_Note that this dependency has not yet been submitted to the Package Control
dependencies repository; thus, it is not actually available for use at this
time. Once it has been submitted and accepted as a Package Control dependency,
this message will be removed._**

This is the *python-docx* module bundled as a
[Package Control](https://packagecontrol.io) dependency for use by
[Sublime Text](https://www.sublimetext.com) packages.

  - [*python-docx* @ GitHub](https://github.com/python-openxml/python-docx)
  - [*python-docx* @ PyPI](https://pypi.org/project/python-docx/)
  - [*python-docx* @ Read the Docs](https://python-docx.readthedocs.io)

## How to use this dependency

In order to tell Package Control that your package requires the *python-docx*
module, create a `dependencies.json` file in your package root with the
following contents:

``` json
{
   "*" : {
      ">=3000" : [
         "lxml",
         "docx"
      ]
   }
}
```

Note that *python-docx* itself requires the
[*lxml*](https://pypi.org/project/lxml) module, which is hosted as a Package
Control dependency [here](https://github.com/eerohele/sublime-lxml). Be aware
that the *lxml* dependency may have its own platform/version restrictions.

Once you have your `dependencies.json` file in place, you can run the
`Package Control: Satisfy Dependencies` command in Sublime Text to make Package
Control install the dependencies for you locally.

Then, once you have all necessary dependencies available locally, you can use
any *python-docx* `import` directives you may need, such as
`from docx import Document`.

See also:
[Documentation on Dependencies](https://packagecontrol.io/docs/dependencies)