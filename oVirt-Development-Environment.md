# oVirt Engine Development Environment for Debian-Based Systems

Install the following third-party packages:
(For Debian, the equivalent of libxml2-python is python-lxml, which provides the required libraries. See [here](https://packages.debian.org/stretch/python-lxml))

    $ sudo apt-get install git openjdk-8-jdk maven openssl postgresql python-m2crypto python-psycopg2 python-cheetah python-daemon unzip python-dateutil python-jinja2 python-lxml

# Note
jboss has been superseded by WildFly. Installing WildFly is as follows: 
    
    $ cd /opt 
    $ wget http://download.jboss.org/wildfly/11.0.0.Alpha1/wildfly-11.0.0.Alpha1.zip 
    $ unzip wildfly-11.0.0.Alpha1.zip 
    $ ln -s /opt/wildfly-10.1.0.Final /opt/wildfly

# Installing Required Packages
Download the packages referenced in the RPM-based systems guide from https://gerrit.ovirt.org/ using Git. To install, follow the instructions in the INSTALL file. 
    
    $  git clone https://gerrit.ovirt.org/ovirt-host-deploy
    $  git clone git://gerrit.ovirt.org/ovirt-js-dependencies
    $  git clone git://gerrit.ovirt.org/ovirt-setup-lib

 ovirt-host-deploy depends on otopi and otopi-dev-tools. These can also be gotten from https://gerrit.ovirt.org/ or the mirror on Github.
    
    
    $  git clone https://gerrit.ovirt.org/otopi
    
Follow the instructions in the INSTALL file. When running the command `make install`, use elevated privileges since the program will want to use the directory /usr/local/share. 
