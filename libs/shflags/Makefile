#
# Copyright (C) 2012 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=shflags
PKG_VERSION:=191
PKG_RELEASE=$(PKG_SOURCE_VERSION)

PKG_SOURCE_PROTO:=svn
PKG_SOURCE_URL:=http://shflags.googlecode.com/svn/trunk/
PKG_SOURCE_SUBDIR:=$(PKG_NAME)-$(PKG_VERSION)
PKG_SOURCE_VERSION:=191
PKG_SOURCE:=$(PKG_NAME)-$(PKG_SOURCE_VERSION).tar.gz

include $(INCLUDE_DIR)/package.mk

define Package/shflags
  SECTION:=libs
  CATEGORY:=Libraries
  TITLE:=shflags
  DEPENDS:=+getopt
  URL:=http://code.google.com/p/shflags/
endef

define Package/shflags/description
 command-line flags module for Unix shell scripts
endef

define Build/Configure
endef

define Build/Compile
endef

define Build/Install
endef

define Package/shflags/install
	$(INSTALL_DIR) $(1)/usr/share/shflags
	$(CP) $(PKG_BUILD_DIR)/source/1.0/src/shflags  $(1)/usr/share/shflags/shflags.sh
endef

$(eval $(call BuildPackage,shflags))
