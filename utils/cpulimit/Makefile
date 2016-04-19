include $(TOPDIR)/rules.mk

PKG_NAME:=cpulimit
PKG_VERSION:=2015-06-17
PKG_RELEASE:=1
PKG_REV:=f4d2682804931e7aea02a869137344bb5452a3cd

PKG_SOURCE_PROTO:=git
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.bz2
PKG_SOURCE_SUBDIR:=$(PKG_NAME)-$(PKG_VERSION)
PKG_SOURCE_URL:=https://github.com/opsengine/cpulimit.git
PKG_SOURCE_VERSION:=$(PKG_REV)

include $(INCLUDE_DIR)/package.mk

define Package/cpulimit
  CATEGORY:=Utilities
  TITLE:=cpulimit
  URL:=https://github.com/opsengine/cpulimit.git
endef

define Package/cpulimit/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/src/cpulimit $(1)/usr/bin
endef


$(eval $(call BuildPackage,cpulimit))
