### Testing Script for the Glibc GHOST Vulnerability # CVE-2015-0235

A little script I found to test the Glibc GHOST Vulnerability # CVE-2015-0235.
The usage is quite simple. Just clone or download the script to your server/desktop and
start it like this:

#### Debian/Ubuntu

    gcc ghosttest.c -o ghosttest

or:

    ./ghosttest.c

#### CentOS/RHEL/Suse

    ./ghosttest.sh

If your server/desktop is vulnerable you should perform an updata **ASAP**.

The pathced Version should be **glibc-2.12-1.149.el6_6.5.x86_64** or **glibc-2.12-1.149.el6_6.5.i686**.

On CentOS/RHEL/Suse you can find the version like this:

    rpm -q glibc

On Debian/Ubuntu you can use this command:

    aptitude show libc6 | grep Version

To fix the vulnerability just run an update, patches have been released.
