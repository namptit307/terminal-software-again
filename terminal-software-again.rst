FOSSAsia Summit 2018
====================

.. figlet:: TUI/CLI Software Again

.. code:: yaml

     Name     : Masayuki Igawa (Twitter/GitHub/freenode: masayukig)
     Slide URL: https://github.com/masayukig/terminal-software-again
     Date     : 13:50-14:09, Sunday, March 25 2018

.. container:: handout

   Most of the people really like webUI and/or smartphone UI. We think
   they are really fancy and cool. However, it sometimes requires
   complicated operation with a mouse, swipe and taps. Moreover, it's
   really hard to tell the operation to the others. We need a lot of
   screenshots to do that. Instead of that, there are a lot of CUI/CLI
   tools as alternatives. They are really simple but powerful and
   fast. In this session, audience can see the benefit of CUI/CLI
   tools. As a developer, GUI is really hard to make a fancy and modern
   design software. We actually have a lot of options not only GUI
   applications but also CUI/CLI applications.

   I really love CUI/CLI applications recently. Because it's fast,
   lightweight and can be operated with only a keyboard not mouse. In
   this talk, I'll give ...

DISCLAIMER
==========

.. cowsay:: These slide are my own opinion.


Agenda
======

* Who am I?
* What is this talk?
* GUI/TUI/CUI/CLI apps examples, Pros/Cons
* Useful libraries
* Conclusion

Who am I?
=========

.. container:: progressive

   * Open Source Programmer (mostly OpenStack)

     * Quarity Assurance (Tempest, stestr..)
   * Working at SUSE
   * Linux User

GUI, TUI, CUI, CLI?
===================

* GUI: Graphical User Interface

* TUI: Text-based User Interface

  * Vim, Emacs, Mutt, Gertty, presentty, etc..
* CLI: Command-Line interface, CUI: Character-based User Interface

  * CLI and CUI are same. Sometimes, it's confusing with TUI.

What is this talk?
==================

* I like TUI/CLI applications!

  * There are a lot of benefits of TUI/CLI apps
  * TUI/CLI apps aren't scary.
  * But I also like GUI ones :)

* Some examples of TUI/CLI/GUI applications


By the way
==========

.. container:: progressive

   * Do you prefer using TUI/CLI apps to GUI (or just **apps** :)
     ones?
   * The answer could be "It depends"..


What kind of applications do we use usually?
============================================

.. container:: progressive

   * Text Editors

     * Vim/Emacs
     * Atom, Eclipse, PyCharm
   * Mail/Chat

     * Mutt, Alpine, WeeChat
     * Thunderbird, XChat
   * Code review

     * gertty (see demo)
     * GitLab, Gerrit
   * presentation

     * TeX, presentty (This!)
     * Impress(LibreOffice)
   * Blog

     * pelican
     * WordPress


What kind of applications do we use usually? - cont.
====================================================

.. container:: progressive

   * Automation

     * Ansible, Chef, Puppet
     * Jenkins
     * Imagine, if Ansible has only GUI? Selenium/Web Scraping = Nightmare?
   * Virtualization

     * Docker, Kubernetes, OpenStack

   .. code::

      -> CLI(not TUI) applications are good for automation


GUI Pros/Cons
====================================

.. container:: progressive

   * :) Easy to start to use (e.g. Scratch)
   * :) Good for a graph dashboard
   * :( Slow (sometimes)
   * :( Complicated

     * Library dependency, UI, bad for automation (e.g. Click here, there...)


TUI/CLI Pros/Cons
===============================

.. container:: progressive

   * :) Fast

     * Narrow bandwidth
     * Poor computer
     * No mouse needed (can be used)

       * Keep the arms position
       * Easy to show how to use
   * :) Simple

     * Easy to show how to use
     * Library dependency

   * :( Difficult to start to use
   * :( Difficult to show graphs and/or images


How to make it? - Useful libraries and commands
===============================================

* urwid: https://pypi.python.org/pypi/urwid (console user interface library for Python)
* cliff: https://pypi.python.org/pypi/cliff (framework for building command line programs)
* figlet: http://www.figlet.org/ (making large letters out of ordinary text)
* jp2a: https://github.com/cslarsen/jp2a (simple JPEG to ASCII converter)

  * jp2a 1.0.8 works but not in 1.0.7..

    .. code:: bash

       $ sudo zypper install libjpeg8-devel automake
       $ git clone https://github.com/cslarsen/jp2a
       $ autoreconf -vi
       $ ./configure --with-jpeg-prefix=/usr/local \
         --with-curl-config=`which curl-config` --enable-curl
       $ make -j && make -j install


.. handout:: Show quick demos if we have the time.


Conclusion
==========

.. container:: progressive

   * CLI/TUI apps are NOT scary, but there is a learning curve
   * CLI/TUI apps should be Fast, Simple, Easy to use
   * CLI apps are very useful for automation
   * Graphs, Images might be better on GUI applications
   * Making CLI/TUI application is (also) fun! and good for starting point

     * Not only just using it, but also making feedbacks


Appendix
========

* Web browser

  * Lynx, w3m, curl, wget
* bug management

  * boartty
* IoT

  * mqtty
* Games

  * ....? :-p
* Similar talk

  * https://www.youtube.com/watch?v=3O60E9CpyJA
