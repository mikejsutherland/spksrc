PKG_NAME = nut
PKG_VERS = 2.7.3
PKG_EXT = tar.gz
PKG_DIST_NAME = $(PKG_NAME)-$(PKG_VERS).$(PKG_EXT)
PKG_DIST_SITE = http://www.networkupstools.org/source/2.7
PKG_DIR = $(PKG_NAME)-$(PKG_VERS)

DEPENDS = cross/net-snmp

HOMEPAGE = http://www.networkupstools.org/
COMMENT  = Network UPS Tools (NUT) project
LICENSE  = LGPLv2
SUPPORTURL = http://www.networkupstools.org/documentation.html

GNU_CONFIGURE = 1
INSTALL_PREFIX = /usr/local/$(PKG_NAME)
CONFIGURE_ARGS = --prefix=$(INSTALL_PREFIX) --with-statepath=$(INSTALL_PREFIX)/var
CONFIGURE_ARGS += --with-snmp=yes --with-snmp-libs="-L$(STAGING_INSTALL_PREFIX)/lib -lnetsnmp"

include ../../mk/spksrc.cross-cc.mk

