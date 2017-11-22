```sh
autoscan
mv configure.scan configure.ac 
autoheader
```
修改 `configure.ac` 增加``AM_INIT_AUTOMAKE`` 
修改完應長得像 `configure.like`
```txt
# configure.ac file
AC_INIT([FULL-PACKAGE-NAME], [VERSION], [BUG-REPORT-ADDRESS])
AM_INIT_AUTOMAKE # here
```
```sh
touch NEWS README AUTHORS ChangeLog COPYING
```
copy `INSTALL,install-sh,compile,depcomp,missing` file to there
```sh
cp -r copyFile/ ./
```
```sh
aclocal
```
必要時修改 `aclocal.m4` 或是 編寫 `acinclude.m4` 他們都是`m4宏` 
```sh
automake #失敗的話從 automake 安裝目錄找 INSTALL,install-sh,compile,depcomp,missing
autoconf
./configure
make
make install
```
更多資訊找 `configure.ac automake aclocal autogen.sh` 等..編寫方式