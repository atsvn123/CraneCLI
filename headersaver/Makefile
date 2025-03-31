TARGET := iphone:clang:latest:15.0
ARCHS = arm64e  # Explicitly target arm64e
export SYSROOT = $(THEOS)/sdks/iPhoneOS16.5.sdk

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = headersaver

headersaver_FILES = Tweak.x
headersaver_CFLAGS = -fobjc-arc
headersaver_LIBRARIES = mryipc
headersaver_IPHONEOS_DEPLOYMENT_TARGET = 15.0  # Explicitly enforce iOS 15.0

include $(THEOS_MAKE_PATH)/tweak.mk
