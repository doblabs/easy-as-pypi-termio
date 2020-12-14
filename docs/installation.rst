############
Installation
############

.. |virtualenv| replace:: ``virtualenv``
.. _virtualenv: https://virtualenv.pypa.io/en/latest/

.. |workon| replace:: ``workon``
.. _workon: https://virtualenvwrapper.readthedocs.io/en/latest/command_ref.html?highlight=workon#workon

To install system-wide, run as superuser::

    $ pip3 install easy-as-pypi-termio

To install user-local, simply run::

    $ pip3 install -U easy-as-pypi-termio

To install within a |virtualenv|_, try::

    $ mkvirtualenv easy-as-pypi-termio
    (easy-as-pypi-termio) $ pip install release-ghub-pypi

To develop on the project, link to the source files instead::

    (easy-as-pypi-termio) $ deactivate
    $ rmvirtualenv easy-as-pypi-termio
    $ git clone git@github.com:tallybark/easy-as-pypi-termio.git
    $ cd easy-as-pypi-termio
    $ mkvirtualenv -a $(pwd) --python=/usr/bin/python3.8 easy-as-pypi-termio
    (easy-as-pypi-termio) $ make develop

After creating the virtual environment,
to start developing from a fresh terminal, run |workon|_::

    $ workon easy-as-pypi-termio
    (easy-as-pypi-termio) $ ...

