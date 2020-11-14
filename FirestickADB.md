#Install ADB tools onto server machine first.

adb start-server  /  adb kill-server (as required)

UP
adb shell input keyevent 19
DOWN
adb shell input keyevent 20
LEFT
adb shell input keyevent 21
RIGHT
adb shell input keyevent 22
ENTER
adb shell input keyevent 66
BACK
adb shell input keyevent 4
HOME
adb shell input keyevent 3
MENU
adb shell input keyevent 1
MEDIA PLAY/PAUSE
adb shell input keyevent 85
MEDIA PREVIOUS
adb shell input keyevent 88
MEDIA NEXT
adb shell input keyevent 87

# Power (Currently not working)
adb shell input keyevent KEYCODE_POWER

# Start Kodi (Live TV)
adb shell am start -n org.xbmc.kodi/.Splash

# Launch Browser and Webpage
adb shell am start -a android.intent.action.VIEW -d https://www.cssscript.com/demo/rss-feed-scroller-marquee/
