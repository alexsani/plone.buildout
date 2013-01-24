Plone buildout
--------------
A simple plone buildout for development and production purpose


Requirements (Debian)
---------------------

    $ apt-get install git libjpeg8-dev poppler-utils python-dev python-virtualenv wv libxml2-dev libxslt1-dev libxslt1.1 libpq-dev libldap2-dev libsasl2-dev libssl-dev libaio-dev ncurses-dev libpcre3-dev

Requirements (Mac)
---------------------
 - Git (https://help.github.com/articles/set-up-git)
 - XCode from App Store
 - VirtualEnv                         
                          
        $ sudo easy_install virtualenv

Install (Debian)
----------------
Clone git repo locally

    $ git clone https://github.com/alexsani/plone.buildout.git plone-test

Create a isolated Python environments with virtualenv (optionally you can add parameter "-p /usr/bin/python2.6" to use a specific python version):

    $ virtualenv --no-site-packages -p /usr/bin/python2.6 plone-test

and, important, activate it:

    $ . plone-test/bin/activate


Install PIL downloading it from http://www.pythonware.com/products/pil/ ed extract it;
install it using python in the virtual-env:

    $ cd /path/to/Imaging-1.1.7
    $ /Users/myuser/plone-python/bin/python setup.py install
	
Clone the git repository in a local folder where you have write access:
    
    $ cd /Users/myuser/
    $ git clone https://github.com/alexsani/plone.buildout.git ./plone
	
and start to install

    $ cd plone
    $ /Users/myuser/plone-python/bin/python boostrap.py --distribute
    $ bin/buildout


