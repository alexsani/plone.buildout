Plone buildout
--------------
A simple plone buildout for development and production purpose


Install
--------------
Use virtualenv to create a isolated Python environments (e.g. in your home):

    $ cd /Users/myuser/
    $ virtualenv --no-site-packages plone-python
	
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


