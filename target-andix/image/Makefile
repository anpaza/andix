# The AndiX project - Linux piggyback for Android
# Copyright (C) 2017 Andrey Zabolotnyi

include $(TOPDIR)/rules.mk
include $(INCLUDE_DIR)/image.mk

define Image/Prepare
	$(CP) $(LINUX_DIR)/arch/$(LINUX_KARCH)/boot/Image $(KDIR)/Image
endef

define Image/Build
	$(call Image/Build/$(1))
	$(CP) $(KDIR)/Image $(BIN_DIR)/$(IMG_PREFIX)-qemu-virt.Image
	$(CP) $(KDIR)/root.$(1) $(BIN_DIR)/$(IMG_PREFIX)-root.$(1)
endef

$(eval $(call BuildImage))
