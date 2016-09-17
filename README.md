Talkwork is a PHP 5.4+ app framework grounded in modularity, simplicity of code,
versatility, and speed. It targets web and CLI usage scenarios.

This project is in the pre-alpha stage of development (i.e. in the womb).

I am developing this with two specific uses in mind: a website CMS and a
CLI-based IRC bot. Hopefully such divergent aims will easily lead toward
flexibility in unforeseen ways.

File structure:
core/    (all framework code)
  - lib/   (holds the cores of the core, mwahahaha)
    - dbal/    (Doctrine's db abstraction layer lets me support *SQL engines)
    - talkwork/    (all the classes that make up the full framework functionality)
  - autoload.json  (tells the autoloader what rule(s) to load)
  - autoloader.php (the class autoloader code)
  - tw-init.php    (sets up the Talkwork environment before the app starts)
  - twautoloadrule.php (Talkwork's rule for how to autoload classes)
tests/       (all code for testing the framework)
index.php    (the file you would execute to start your app)
php.ini      (some custom PHP settings we want in place)
tw-config.php    (the settings you will start up Talkwork with)
twdb.sql     (sample database contents)

The name was actually generated by Wordoid (which I discovered thanks to Chris
Pirillo), and I liked it enough to contrive a meaning for it: it is a framework
to facilitate communication (hence, "talk").
Yeah, I know it's weak. You got a better idea? Talk to me.

Any code contribution is welcomed and, in fact, requested.