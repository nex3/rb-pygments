# rb-pygments

This is a wrapper for the [Pygments](http://pygments.org) syntax highlighter.
It can be used to highlight a wide variety of languages in a wide variety of formats.

## Usage

All functionality is available through the {Pygments} module.
Highlighting is done via the {Pygments.highlight highlight} method,
like so (reformatted for readability:

    Pygments.highlight("Some.ruby(:code)", :ruby, :html, :nowrap => true)
      #=> <span class="no">Some</span>
          <span class="o">.</span>
          <span class="n">ruby</span>
          <span class="p">(</span>
          <span class="ss">:code</span>
          <span class="p">)</span>

Stylesheets and such can be retrieved via the {Pygments.style style} method.

## Requirements

yard-pygments requires that Pygments be installed.
Since Pygments is written in Python, it needs to be installed manually.
If you've got [`easy_install`](http://peak.telecommunity.com/DevCenter/EasyInstall), you can do

    !!!sh
    easy_install Pygments

Otherwise, it can be downloaded [here](http://pypi.python.org/pypi/Pygments).
