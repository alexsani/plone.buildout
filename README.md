Plone buildout
--------------
A simple plone buildout for development and production purpose


Requirements (Debian)
---------------------

    $ apt-get install git libjpeg8-dev poppler-utils python-dev python-virtualenv wv libxml2-dev libxslt1-dev libxslt1.1 libpq-dev libldap2-dev libsasl2-dev libssl-dev libaio-dev ncurses-dev libpcre3-dev

Requirements (Mac)
---------------------
 - Git (https://help.github.com/articles/set-up-git)
 - XCode from App Store (from XCode preference also install "Command line tools")
 - VirtualEnv                         
                          
        $ sudo easy_install virtualenv


Install (Debian)
----------------
Clone git repo locally

    $ git clone https://github.com/alexsani/plone.buildout.git plone-test

Create a isolated Python environments with virtualenv (optionally you can add parameter "-p /usr/bin/python2.6" to use a specific python version):

    $ sudo virtualenv --no-site-packages -p /usr/bin/python2.6 plone-test

and, important, activate it:

    $ cd plone-test
    $ . bin/activate

(ONLY for Mac install PIL in the virtualenv

    $ sudo bin/easy_install pillow
    
)

    $ sudo bin/python boostrap.py

Edit onfiguration file to fit your buildout



