.. _developers:

*******************
Developer Resources
*******************


.. _developers-getting-started:

New Developers
==============

Contributing to open source projects can be intimidating. We recommend checking
out the following resources to get started:

- `Open Source Guide <https://opensource.guide/>`_
   A concise guide for contributing to open source projects.
- `first-contributions <https://github.com/firstcontributions/first-contributions>`_
   A github repository that gives a quick step-by-step introduction to forking
   repositories and creating pull requests and a high-level overview of the
   general contribution workflow listed in the 
   `Open Source Guide <https://opensource.guide/>`_.


How to Contribute
=================

We recommend creating an issue for a new feature, bug fix, or other modification
to pyEPR or starting with an existing issue marked as 
`good first issue <https://github.com/zlatko-minev/pyEPR/issues?q=is%3Aissue+is%3Aopen+label%3A"good+first+issue">`_.


Style Recommendations and Best Practices
----------------------------------------

To improve the readability of source code, documentation, and git commit
messages, we have compiled some simple guidelines for developer contributions.


* Source Code Formatting
    - Class names set in camel case, i.e. ``MyClass`` has the first and second
      sub-word capitalized
.. code-block:: python

    class MyClass(object):
        """
        The finest of the classes
        """
        def __init__(self, *args, **kwargs):
            """
            Class constructor for a generic set of arguments in args and keyword
            arguments in kwargs
            """
..

    - Underscore-separated names for functions ``my_first_function``
    - Include doc-strings under the function definition and class definitions
      describing the basic operation of the function, its inputs, and its
      outputs 
.. code-block:: python

    def my_first_function(x, y, **kwargs):
        """
        Arguments:
        =========

        x:          list of independent variables
        y:          list of dependent variables

        Returns:
        =======

        """

        return x**2 + y**2
..

* Documentation Formatting


* Git Commit Formatting
    - For commit messages, we recommend that developers follow the guidelines
      outlined in `<https://chris.beams.io/posts/git-commit/>`_
    - Here is quick summary of the above blog post:
        1. Separate the subject of the commit from the body with a new line and
           provide a detailed explanation in the body::

            Add new feature to fix #XXX

            Detailed explanation of problem
            With why the change(s) were made
            Wrap to 72 characters

        2. Limit subject to 50 characters, this makes ``git log --oneline``
           easier to browse through commit history
