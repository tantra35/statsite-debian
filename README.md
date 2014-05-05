statsite-debian
===============

Debian packaging for statsite

How-to
--------

    $ git clone https://github.com/armon/statsite.git statsite # Get upstream app
    $ rm -rf statsite/.git # Remove VCS files
    $ tar cvjf statsite_0.6.5.orig.tar.bz2 statsite/ # Create source archive
    $ git clone https://github.com/melkor217/statsite-debian.git statsite/debian
    $ cd statsite 
    $ debuild -us -uc # Build it. A couple of build dependencies must be installed via apt or something
    $ sudo dpkg -i ../statsite_0.6.5-1_amd64.deb # Enjoy!
