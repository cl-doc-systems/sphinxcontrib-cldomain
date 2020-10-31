How to build the documentation
==============================

- install `Roswell <https://github.com/roswell/roswell>`_.

- install the `cldomain <http://40ants.com/cldomain/>`_ Sphinx extension
  to build Common Lisp projects' documentation:

  ::
     
     ros install 40ants/cldomain

- create a `Python virtual env <https://virtualenv.pypa.io/en/stable/installation/#installation>`_:

  ::
     
     virtualenv env
     source env/bin/activate
     pip install pipenv

- and install the Python dependencies:

  ::
     
     PIPENV_PIPFILE=docs/scripts/Pipfile pipenv install

- now build the doc:

  ::

     cd docs
     make html

- and open the generated doc with your browser:

  ::

     open build/html/index.html
