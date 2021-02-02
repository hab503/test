#
# Copyright (C) 2015-2016 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v3.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=k3wifih
PKG_VERSION:=1
PKG_RELEASE:=2

include $(INCLUDE_DIR)/package.mk

define Package/$(PKG_NAME)
	TITLE:=k3wifih
	DEPENDS:=
	URL:=http://www.k3wifih.com/
endef

define Package/$(PKG_NAME)/description
  k3wifih fw
endef

define Build/Prepare
endef

define Build/Configure
endef

define Build/Compile
endef


define Package/$(PKG_NAME)/install
	$(INSTALL_DIR) $(1)/lib
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DIR) $(1)/lib/firmware/brcm
	$(INSTALL_DATA) ./files/lib/firmware/brcm/brcmfmac4366c-pcie.bin.69027 $(1)/lib/firmware/brcm/brcmfmac4366c-pcie.bin1
endef

$(eval $(call BuildPackage,$(PKG_NAME)))
