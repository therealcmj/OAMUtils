# OAMUtil
OAM Utilities

A little landing place for any OAM utils that I find myself needing.


JPSCreds:

From OAM 11.1.2.3 release, the OAM wlst command ListCred() is not available. If you need to access the .oamkeystore you will need to [retrieve the .oamkeystore password programatically](http://howtoidm.blogspot.com/2015/07/how-to-retrieve-oamkeystore-oamstore.html).


update build.xml:
  <property name="fmw_home" value="/home/oracle/Oracle/Middleware"/>
  <property name="domain_home" value="${fmw_home}/user_projects/domains/OAMDomain"/>

To compile just run via ant

$ ant
Buildfile: build.xml

clean:

prep:
    [mkdir] Created dir: /home/oracle/OAMutil/build

compile:
    [javac] Compiling 1 source file to /home/oracle/OAMutil/build

build:

BUILD SUCCESSFUL
Total time: 1 second


To run just type ant run:
$ ant run
Buildfile: build.xml

clean:
   [delete] Deleting directory /home/oracle/OAMutil/build

prep:
    [mkdir] Created dir: /home/oracle/OAMutil/build

compile:
    [javac] Compiling 1 source file to /home/oracle/OAMutil/build

build:

run:
     [java] Feb 03, 2016 11:49:52 AM oracle.security.audit.Auditor init
     [java] WARNING: IAU:IAU-6012: Unable to determine the audit log directory. No log directory specified.
     [java] Feb 03, 2016 11:49:52 AM oracle.security.jps.util.JpsUtil disableAudit
     [java] INFO: JpsUtil: isAuditDisabled set to true
     [java] Feb 03, 2016 11:49:52 AM oracle.security.jps.internal.audit.AuditServiceImpl validateLogPossible
     [java] WARNING: No audit log directory is set. Cannot perform audit operations for component JPS.
     [java] tda59eg5h6i6ef8f9gkjqq20dq

BUILD SUCCESSFUL
Total time: 8 seconds