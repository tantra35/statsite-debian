statsite-debian
===============

Debian packaging for statsite

How-to

```bash
    $ git clone https://github.com/armon/statsite.git statsite # Get upstream app
    $ rm -rf statsite/.git # Remove VCS files
    $ tar zcf statsite_0.8.0.orig.tar.gz statsite/ # Create source archive
    $ git clone https://github.com/tantra35/statsite-debian.git statsite/debian
    $ cd statsite 
    $ debuild -us -uc # Build it. A couple of build dependencies must be installed via apt or something
    $ sudo dpkg -i ../statsite_0.8.0_amd64.deb # Enjoy!
```
