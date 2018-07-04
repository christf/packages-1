include $(TOPDIR)/rules.mk

PKG_NAME:=clientsim
PKG_VERSION:=1.0

PKG_BUILD_DIR := $(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/clientsim
  SECTION:=ffffm
  CATEGORY:=Customization
  TITLE:=run a naive script that simulates client network traffic from rc.local
  DEPENDS:=+gluon-core +busybox +wget
  MAINTAINER:=Freifunk Frankfurt <admin@ffm.freifunk.net>
  URL:=https://github.com/freifunk-gluon/packages
  SOURCE:=https://github.com/freifunk-gluon/packages
endef

define Package/clientsim/description
	This will simulate a client by loading various websites from rc.local using wget
endef

define Build/Prepare
	mkdir -p $(PKG_BUILD_DIR)
endef

define Build/Configure
endef

define Build/Compile
endef


define Package/clientsim/install
	$(CP) ./files/* $(1)/
endef

$(eval $(call BuildPackage,clientsim))
