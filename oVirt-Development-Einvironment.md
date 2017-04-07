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
