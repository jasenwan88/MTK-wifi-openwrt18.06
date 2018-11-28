#
# Copyright (C) 2018 Willy All rights reserved
#
# Written by Willy(jasenwan@163.com)
# Created Time: Wed 28 Nov 2018 11:58:30 AM CST
#

include $(TOPDIR)/rules.mk

PKG_NAME:=luci-mtk-wifi
PKG_VERSION:=0.1
PKG_RELEASE:=

PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)-$(PKG_VERSION)

include $(INCLUDE_DIR)/package.mk

define Package/luci-mtk-wifi
  SECTION:=MTK Properties
  CATEGORY:=MTK Properties
  TITLE:=LuCI patch for MTK WiFi drivers
  SUBMENU:=Applications
  DEPENDS:=+luci-mod-admin-full
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Compile/Default

endef
Build/Compile = $(Build/Compile/Default)

define Package/luci-mtk-wifi/install
	$(INSTALL_DIR) $(1)/usr/lib/lua/luci/model/cbi/admin_network
	$(INSTALL_BIN) files/wifi.lua $(1)/usr/lib/lua/luci/model/cbi/admin_network/
endef

$(eval $(call BuildPackage,luci-mtk-wifi))
