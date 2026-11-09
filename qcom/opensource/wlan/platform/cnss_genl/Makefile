# SPDX-License-Identifier: GPL-2.0-only

WLAN_PLATFORM_PROFILE ?= sun
include $(WLAN_PLATFORM_ROOT)/cnss_genl/$(WLAN_PLATFORM_PROFILE)_gki_defconfig
ccflags-y += -Wmissing-prototypes

ifeq ($(CONFIG_CNSS_OUT_OF_TREE),y)
ccflags-y += -I$(WLAN_PLATFORM_ROOT)/inc
endif

obj-$(CONFIG_CNSS_GENL) := cnss_nl.o
