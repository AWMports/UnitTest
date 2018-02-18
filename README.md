AWMports\ezcUnitTest
====================

This is a port of the `zetacomponents/UnitTest` package to use PSR-4 namespaced
class and filename structure.

The initial fork is of `zetacomponents/UnitTest` version 1.0.2

This fork is likely broken and should currently not be used. Well, um, except
to help identify what I broke in my hair-brained idea.

__THIS FORK SHOULD NOT YET BE USED__


About AWMports
--------------

AWMports (prounounced ‘A W Imports’) is a collection of Composer installable PHP
libraries that either predate PHP-FIG or otherwise do not use namespaced
classes in a manner that is easily compatible with PSR-4 style auto-loaders.

Initial attempts will be to port Zeta Components and perhaps some abandoned PECL
packages.

AWMports is a project of Alice Wonder Miscreations.


About Zeta Components
---------------------

The Zeta Components website is at [zetacomponents.org](http://zetacomponents.org/)

Current development takes place on [github](https://github.com/zetacomponents)

It is a *fantastic* collection of re-usable PHP libraries and their code also
is one of the better ways to learn about PHP object oriented programming, with
actual real-world implementations of many techniques I confess I really did not
have a good grasp on before reading their code.


Minor Changes from Upstream
===========================

Within the `src/` directory, all classes are now in a single directory and thus
also within a single namespace, `\AWMports\ezcUnitTest`.


Library and Application Porting
-------------------------------

To port existing libraries and applications from zetacomponents/UnitTest to
AWMports/ezcUnitTest:

    Zeta Components Class Name        Namespaced Equivalent
    ------------------------------------------------------------------------------
    ezcTestCase                   --> \AWMports\ezcUnitTest\TestCase
    ezcTestImageCase              --> \AWMports\ezcUnitTest\TestImageCase
    ezcTestConstraintSimilarImage --> \AWMports\ezcUnitTest\ConstraintSimilarImage
    ezcTestRegressionSuite        --> \AWMports\ezcUnitTest\RegressionSuite
    ezcTestRegressionTest         --> \AWMports\ezcUnitTest\RegressionTest
