# how-to-use-criann-cluster
A list of questions I asked when using CRIANN cluster and the possible answers to them.

Feel free to ask a question or answer one. You are welcome to add one :triangular_flag_on_post: to a question if you met it before. (Try not to remove flags~) Have fun!

## How to log into the CRIANN cluster? :8ball::triangular_flag_on_post:

## How to install a Python package that doesn't exist on CRIANN server? :triangular_flag_on_post:

There are several ways to do it.

### Ask an administrator of CRIANN to add it for you.

It is simple, however may take a long time and may be refused.

### Use the ``--user`` option of pip/pip3.

For example, if you try to add the NumPy package to your local directory, you can use the command:

``pip3 install --user numpy``

This will install the numpy package to your local directory, no need of the root right.

### Install a package to your local directory from source code.

Take NumPy for example. First download the source from its website:

``wget jaist.dl.sourceforge.net/project/numpy/NumPy/1.11.2/numpy-1.11.2.tar.gz``

Unzip the file:

``tar -xzf jaist.dl.sourceforge.net/project/numpy/NumPy/1.11.2/numpy-1.11.2.tar.gz``

Enter the numpy directory:

``cd numpy-1.11.2``

Configure installation directory and install:

``python setup.py install --prefix $HOME/.local``

This command will install the NumPy package to the $HOME/.local directory.
