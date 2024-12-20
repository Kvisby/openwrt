include $(TOPDIR)/rules.mk

PKG_NAME:=student-db

PKG_VERSION:=1.0
PKG_RELEASE:=1
PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/Kvisby/student-db.git
PKG_SOURCE_VERSION:=main

PKG_MIRROR_HASH:=skip

PKG_MAINTAINER:=Kristaps Bukss <kristaps.bukshs@gmail.com>

include $(INCLUDE_DIR)/package.mk

define Package/student-db
	SECTION:=custom
	CATEGORY:=RTU
	TITLE:=student-db
	DEPENDS:=+libc
endef

define Package/student-db/description
	student-db
endef

define Package/student-db/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/student_db $(1)/usr/bin/
endef

$(eval $(call BuildPackage,student-db))

