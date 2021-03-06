Handwritten documentation
=========================

I think the ability to write a large pieces of documentation which aren't bound to
a function, class or module is an important feature. This way you can tell the user
about some toplevel abstractions and give a bird eye view on the library or system.

For example, handwritten parts of the documentation can provide some code snippets
to demonstrate the ways, how to use the library:

.. code-block: lisp

   (loop repeat 42
         collect (foo "bar" 100500))

And when you are talking about some function or class, you can reference it.
For example, if I'm talking about ``foo`` function, I can reference it like this
``:cl:function:`example/app:foo``` and it will appear in the code as
the link :cl:function:`example/app:foo`.

Please, note, that if you don't include the documentation on
:cl:function:`foo <example/app:foo>` function, Sphinx will
complain with this warning:

::

   WARNING: Unused symbol doc EXAMPLE/APP:FOO type function

And this text ``:cl:function:`example/app:foo``` will not become a link.

To learn, how to fix this problem, read about :ref:`Autogenerated API`.
