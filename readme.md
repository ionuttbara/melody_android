Melody Script for Android
Optimizes The Android Phone.
<h1 align="center">
  <br>
  <img src="https://raw.githubusercontent.com/jbara2002/melody12/master/logo.png" alt="Melody logo"></a>
</h1>

# Requiments
Android Phone with OS Version 7.1.1 or newer.  
ADB Installed with Drivers (the ADB Installer will be put in release and source code management).  


# Commands

__YOU CAN CREATE A BAT FILE FROM THAT COMMANDS.__
The list of commands for
> # IMPROVING SYSTEM PERFORMANCE
>*Disables Z-RAM ,Window Blur Effects and animations*
>>adb shell settings put global zram_enabled 0  
>>adb shell settings put global disable_window_blurs 1 
>> adb shell settings put system screen_auto_brightness_adj 1.0  
>> adb shell settings put system peak_refresh_rate 48.0  (__THIS SET THE SCREEN TO 48Hz Refresh rate, if don't want that, don't put in the bat list.__)  
>> adb shell settings put system min_refresh_rate 1.0  
>> adb shell settings put global window_animation_scale 0.0  
>> adb shell settings put global transition_animation_scale 0.0  
>> adb shell settings put global animator_duration_scale 0.0  
>
> # IMPROVING MOBILE NETWORKING PERFORMANCE
>*Improved network data transfer (3G/4G/5G)*  
>*Disabling some throttling , enabling mobile data by default when boot and enable assisted GPS*
>>adb shell settings put global network_recommendations_enabled 0  
>>adb shell settings put global network_scoring_ui_enabled 0  
>>adb shell settings put global tether_offload_disabled 0  
>>adb shell settings put global wifi_power_save 0  
>>adb shell settings put global enable_cellular_on_boot 1  
>>adb shell settings put global mobile_data_always_on 0  
>>adb shell settings put global ble_scan_always_enabled 0  
> # IMPROVING POWER MANAGEMENT ON PHONES
>*Improving the way the phone is sleeping by disable adaptive sleep algorithms.*  
>*If you get delayed notifications of messaging applications, go to Settings, App, go to messaging app, battery and set to __Unrestricted__.*  
>*Don't use 3rd Party or OEM Applications for doing that. I don't recommend doing that with them because the effect will be not desired as seen.*  
>*Recommendation: Removing all 3rd Cleaning or Device Care Application for the algorithm to work correctly.*  
>>adb shell settings put global cached_apps_freezer enabled  
>>adb shell settings put global app_standby_enabled 1  
>>adb shell settings put global adaptive_battery_management_enabled 0  
>>adb shell settings put secure long_press_timeout 250  
>>adb shell settings put secure multi_press_timeout 250  
>>adb shell settings put global app_restriction_enabled true  
>>adb shell settings put system intelligent_sleep_mode 0  
>>adb shell settings put secure adaptive_sleep 0  
># DISABLING ANDROID SCREEN SAVER TO GET BETTER BATTERY LIFE  
>>adb shell settings put secure screensaver_enabled 0   
>>adb shell settings put secure screensaver_activate_on_sleep 0  
>>adb shell settings put secure screensaver_activate_on_dock 0  
