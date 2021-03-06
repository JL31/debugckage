debugckage
==========

This package contains functions to help debugging :

- dprint : function that enables to print the name and the value of the input parameter of the function


You can install it through pip :

.. code-block:: python

    pip install debugckage


Exemples of use :

.. code-block:: python

    >>> from debugckage import dprint
    >>>
    >>> var1 = 10.0
    >>> dprint(var1)
    var1 : 10.0

    >>> from debugckage import dprint
    >>>
    >>> def test():
    >>>     """
    >>>         test function
    >>>     """
    >>>
    >>>     var2 = "a"
    >>>     dprint(var2)
    >>>
    >>> test()
    var2 = "a"
    
    >>> from debugckage import dprint
    >>>
    >>> class Test():
    >>>     """
    >>>         test class
    >>>     """
    >>>
    >>>     def __init__(self):
    >>>         """
    >>>             class constructor
    >>>         """
    >>>
    >>>         self.var3 = 45
    >>>
    >>>     def test_method():
    >>>         """
    >>>             test method
    >>>         """
    >>>
    >>>             dprint(self.var3)
    >>>
    >>> t = Test()
    >>> t.test_method()
    [ class instance is : "t" ] self.var3 = 45


The code has been developped under Python 3.7 ans is under the WTFPL_ license.

.. _WTFPL: https://fr.wikipedia.org/wiki/WTFPL
