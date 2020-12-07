include $(TOPDIR)/rules.mk

PKG_NAME:=python3-temper-py
PKG_VERSION:=0.0.2
PKG_RELEASE:=1

PYPI_NAME:=temper-py
PKG_HASH:=cd1f6d15978661f1326d2fea9150e9b72aee852523bc3a8c74226bfc4ac3ec82

PKG_MAINTAINER:=Timothee Floure <timothee.floure@ungleich.ch>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-temper-py
  SECTION:=lang
  CATEGORY:=Languages
  SUBMENU:=Python
  TITLE:=Reads temperature data from misc. 'TEMPer' devices
  URL:=https://github.com/ccwienk/temper
  DEPENDS:=+python3-light +python3-pyserial +kmod-usb-hid
endef

define Package/python-temper-py/description
  Reads temperature data from misc. 'TEMPer' devices, using minimal dependencies
endef

$(eval $(call Py3Package,python3-temper-py))
$(eval $(call BuildPackage,python3-temper-py))
$(eval $(call BuildPackage,python3-temper-py-src))
