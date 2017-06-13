# The AndiX project - Linux piggyback for Android
# Copyright (C) 2017 Andrey Zabolotnyi

include $(TOPDIR)/rules.mk

BOARD:=andix
BOARDNAME=AndiX piggyback Unix for Android
FEATURES+=targz
SUBTARGETS:=arm32 arm64
MAINTAINER:=Andrey Zabolotnyi <zapparello@ya.ru>

DEVICE_TYPE:=andix
KERNEL_PATCHVER:=4.4

include $(INCLUDE_DIR)/target.mk

$(eval $(call BuildTarget))
