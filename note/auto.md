autoscan
mv configure.scan configure.ac 
autoheader
修改 configure.ac 增加AM_INIT_AUTOMAKE
```
AC_INIT([FULL-PACKAGE-NAME], [VERSION], [BUG-REPORT-ADDRESS])
AM_INIT_AUTOMAKE # here
```
touch NEWS README AUTHORS ChangeLog COPYING
copy INSTALL,install-sh,compile,depcomp,missing file to there
automake

修改 aclocal.m4 或是 編寫 acinclude.m4 他們都是m4宏 autogen.sh
aclocal
autoconf
#mv Makefile Makefile.in

./configure


更多資訊找 configure.ac automake aclocal 等..編寫方式