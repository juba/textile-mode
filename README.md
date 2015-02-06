# textile-mode
An emacs major mode for Textile markup language editing.

## What is textile ?

Textile is a markup language created by the author of *TextPattern*. It is used by some content management systems, wikis, and there are libraries to convert Textile into HTML for Ruby, Python or PHP.

More information on the markup can be found here :

http://www.textism.com/tools/textile/

http://hobix.com/textile/


## Manual installation

Installation of Textile-mode is really nothing original. Put the file in a directory into your load-path, and then add the following into your .emacs :

```
(require 'textile-mode)
```

Then you can toggle manualy the major mode with `M-x` `textile-mode` or you can associate it with a file extension with :

```
(add-to-list 'auto-mode-alist '("\\.textile\\'" . textile-mode))
```

## Bugs - Troubleshooting

If the syntax highlighting doesn't seem to be synchronized with your text, you can refresh it manually on a paragraph with `M-g` `M-g`, or globally by turning font-locking off and on.

There are some known limitations in the syntax highlighting : see the source code introduction for details.
