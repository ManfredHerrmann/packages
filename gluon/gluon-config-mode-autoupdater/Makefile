include $(TOPDIR)/rules.mk

PKG_NAME:=gluon-config-mode-autoupdater
PKG_VERSION:=1

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(GLUONDIR)/include/package.mk

define Package/gluon-config-mode-autoupdater
  SECTION:=gluon
  CATEGORY:=Gluon
  TITLE:=Let the user know whether the autoupdater is enabled or not.
  DEPENDS:=+gluon-config-mode-core +gluon-autoupdater
endef

define Package/gluon-config-mode-autoupdater/description
	Luci based config mode
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef

define Package/gluon-config-mode-autoupdater/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,gluon-config-mode-autoupdater))
