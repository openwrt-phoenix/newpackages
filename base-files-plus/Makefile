#
# Copyright (C) 2007-2016 OpenWrt.org
# Copyright (C) 2010 Vertical Communications
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#


include $(TOPDIR)/rules.mk

PKG_NAME:=base-files-plus
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/base-files-plus
  SECTION:=base
  CATEGORY:=Base system
  DEPENDS:=+base-files
  TITLE:=Base filesystem for OpenWrt plus
  URL:=http://openwrt.org/
  VERSION:=$(PKG_RELEASE)-$(REVISION)
endef

define Package/base-files-plus/description
  This package contains a base filesystem and system scripts for OpenWrt.
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Compile

endef

define Package/base-files-plus/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,base-files-plus))
