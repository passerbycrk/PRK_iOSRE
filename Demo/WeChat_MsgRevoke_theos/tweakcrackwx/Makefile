THEOS_DEVICE_IP = localhost
THEOS_DEVICE_PORT = 2333
ARCHS = arm64
TRAGET = iphone:latest:9.0

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = TweakcrackWX
TweakcrackWX_FILES = Tweak.xm

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	install.exec "killall -9 SpringBoard"
