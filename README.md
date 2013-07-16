Bin packages for gentoo linux on rpi-armv6j-hardfloat.
More infomation see file "Packages".
Create:
Licensc:GNU GPLv2

### Features are as following:

# These settings were set by the catalyst build script that automatically
# built this stage.
# Please consult /usr/share/portage/config/make.conf.example for a more
# detailed example.
CFLAGS="-O2 -pipe -march=armv6j -mfpu=vfp -mfloat-abi=hard -fomit-frame-pointer"
CXXFLAGS="${CFLAGS}"
# WARNING: Changing your CHOST is not something that should be done lightly.
# Please consult http://www.gentoo.org/doc/en/change-chost.xml before changing.
CHOST="armv6j-hardfloat-linux-gnueabi"
ARCH=arm
E_MACHINE=EM_ARM
ACCEPT_KEYWORDS="arm"

USE="   arm zlib bindist make-symlinks -minimal \
        X apache2 bash-completion berkdb cjk cxx dbus fortran gif \
	ipv6 jpeg jpeg2k mudflap multislot mysql nls nptl nptlonly \
	openmp php png python threads tiff truetype unicode usb \
	userland_GNU \
        -bindist -debug -doc -handbook \
	"

LINGUAS="en en_US zh_CN zh"

APACHE2_MODULES=" \
	actions alias auth_basic authn_alias authn_anon authn_dbm \
	authn_default authn_file authz_dbm authz_default authz_groupfile \
	authz_host authz_owner authz_user autoindex cache cgi cgid dav dav_fs \
	dav_lock deflate dir disk_cache env expires ext_filter file_cache \
	filter headers include info log_config logio mem_cache mime mime_magic \
	negotiation rewrite setenvif speling status unique_id userdir \
	usertrack vhost_alias \
	"
APACHE2_MPMS=worker

PHP_INI_VERSION=production 
PHP_TARGETS=php5-4

### python version
USE_PYTHON="2.6 2.7 3.1"

### Kernel Version ###
Linux pi-gentoo 3.9.5-cutdown+ #7 PREEMPT Sun Jun 23 14:23:59 CST 2013 armv6l BCM2708 GNU/Linux

### GCC version ###
Using built-in specs.
COLLECT_GCC=/usr/armv6j-hardfloat-linux-gnueabi/gcc-bin/4.6.3/gcc
COLLECT_LTO_WRAPPER=/usr/libexec/gcc/armv6j-hardfloat-linux-gnueabi/4.6.3/lto-wrapper
Target: armv6j-hardfloat-linux-gnueabi
Configured with: /usr/portage/tmp/portage/sys-devel/gcc-4.6.3/work/gcc-4.6.3/configure \
--prefix=/usr --bindir=/usr/armv6j-hardfloat-linux-gnueabi/gcc-bin/4.6.3 \
--includedir=/usr/lib/gcc/armv6j-hardfloat-linux-gnueabi/4.6.3/include \
--datadir=/usr/share/gcc-data/armv6j-hardfloat-linux-gnueabi/4.6.3 \
--mandir=/usr/share/gcc-data/armv6j-hardfloat-linux-gnueabi/4.6.3/man \
--infodir=/usr/share/gcc-data/armv6j-hardfloat-linux-gnueabi/4.6.3/info \
--with-gxx-include-dir=/usr/lib/gcc/armv6j-hardfloat-linux-gnueabi/4.6.3/include/g++-v4 \
--host=armv6j-hardfloat-linux-gnueabi --build=armv6j-hardfloat-linux-gnueabi \
--disable-altivec --disable-fixed-point --without-cloog --without-ppl --disable-lto \
--with-float=hard --enable-nls --without-included-gettext --with-system-zlib \
--enable-obsolete --disable-werror --enable-secureplt --disable-multilib --enable-libmudflap \
--disable-libssp --enable-libgomp \
--with-python-dir=/share/gcc-data/armv6j-hardfloat-linux-gnueabi/4.6.3/python \
--enable-checking=release --disable-libgcj --enable-libstdcxx-time --with-arch=armv6j \
--with-float=hard --with-fpu=vfp --enable-languages=c,c++,fortran --enable-shared \
--enable-threads=posix --enable-__cxa_atexit --enable-clocale=gnu \
--with-bugurl=http://bugs.gentoo.org/ --with-pkgversion='Gentoo 4.6.3 p1.13, pie-0.5.2'
Thread model: posix
gcc version 4.6.3 (Gentoo 4.6.3 p1.13, pie-0.5.2) 
