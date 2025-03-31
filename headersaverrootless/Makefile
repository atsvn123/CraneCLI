TARGET := iphone:clang:latest:15.0
ARCHS = arm64e  # Explicitly target arm64e
export SYSROOT = $(THEOS)/sdks/iPhoneOS16.5.sdk

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = headersaverrootless

headersaverrootless_FILES = Tweak.xm
headersaverrootless_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/tweak.mk
