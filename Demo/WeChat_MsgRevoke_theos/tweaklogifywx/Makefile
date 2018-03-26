THEOS_DEVICE_IP = localhost
THEOS_DEVICE_PORT = 2333
ARCHS = arm64
TRAGET = iphone:latest:9.0

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = TWeakLogifyWX
TWeakLogifyWX_FILES = Tweak.xm
logifyWX_FRAMEWORKS = UIKit Foundation CoreGraphics
logifyWX_CFLAGS = -fobjc-arc

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	install.exec "killall -9 SpringBoard"
