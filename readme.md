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
>> ```
>>adb shell settings put global zram_enabled 0  
>>```
>>```
>>adb shell settings put global accessibility_reduce_transparency 1
>>```
>>```
>>adb shell settings put global disable_window_blurs 1 
>>```
>> ```
>> adb shell settings put global window_animation_scale 0.0  
>> ```
>> ```
>> adb shell settings put global transition_animation_scale 0.0  
>> ```
>> ```
>> adb shell settings put global animator_duration_scale 0.0  
>> ```
>>```
>>adb shell settings put system screen_auto_brightness_adj 1.0  
>>```
>>
>> (__THIS SET THE SCREEN TO 48Hz Refresh rate, if don't want that, don't put in the bat list.__)  
>> ``` 
>>adb shell settings put system peak_refresh_rate 48.0
>>```
>>```
>> adb shell settings put system min_refresh_rate 1.0  
>> ```
>
> # IMPROVING MOBILE NETWORKING PERFORMANCE
>*Improved network data transfer (3G/4G/5G)*  
> *Also it will block 90-95% of ads and porn websites without root.*
>*Disabling some throttling , enabling mobile data by default when boot and enable assisted GPS*
>> ```
>>adb shell settings put global network_recommendations_enabled 0 
>>```
>>``` 
>>adb shell settings put global network_scoring_ui_enabled 0  
>>```
>>```
>>adb shell settings put global tether_offload_disabled 0  
>>```
>>```
>>adb shell settings put global wifi_power_save 0  
>>```
>>```
>>adb shell settings put global enable_cellular_on_boot 1  
>>```
>>```
>>adb shell settings put global mobile_data_always_on 0  
>>```
>>```
>>adb shell settings put global ble_scan_always_enabled 0
>>```  
>>```
>>adb shell settings put global private_dns_specifier family.adguard-dns.com
>>```
> # IMPROVING POWER MANAGEMENT ON PHONES
>*Improving the way the phone is sleeping by disable adaptive sleep algorithms.*  
>*If you get delayed notifications of messaging applications, go to Settings, App, go to messaging app, battery and set to __Unrestricted__.*  
>*Don't use 3rd Party or OEM Applications for doing that. I don't recommend doing that with them because the effect will be not desired as seen.*  
>*Recommendation: Removing all 3rd Cleaning or Device Care Application for the algorithm to work correctly.*  
>>```
>>adb shell settings put global cached_apps_freezer enabled  
>>```
>>```
>>adb shell settings put global sem_enhanced_cpu_responsiveness 0
>>```
>>```
>>adb shell settings put global enhanced_processing 0
>>```
>>```
>>adb shell settings put global app_standby_enabled 1  
>>```
>>```
>>adb shell settings put global adaptive_battery_management_enabled 0 
>>```
>>``` 
>>adb shell settings put global app_restriction_enabled true  
>>```
>>```
>>adb shell settings put system intelligent_sleep_mode 0  
>>```
>>```
>>adb shell settings put secure adaptive_sleep 0 
>>``` 
># DISABLING ANDROID SCREEN SAVER TO GET BETTER BATTERY LIFE  
>>```
>>adb shell settings put secure screensaver_enabled 0  
>>```
>>``` 
>>adb shell settings put secure screensaver_activate_on_sleep 0  
>>```
>>```
>>adb shell settings put secure screensaver_activate_on_dock 0
>>```  
># Speed up Long Press Delay
>> ```
>> adb shell settings put secure long_press_timeout 250
>> ```
>> ```
>> adb shell settings put secure multi_press_timeout 250
>> ```
>> 
># Remove User Manual from Settings (Samsung OneUI)
>> ```
>> adb shell settings put global online_manual_url 0
>> ```
># Call Features. Enabling extra in-call volume and Noice Reduction
># Add Volume in Call
>> ```
>> adb shell settings put system call_extra_volume 1
>> ```
># Add Noice Reduction on Calls
>> ```
>> adb shell settings put system call_noise_reduction 1
>> ```
># Disabling In-Answer Call Vibration
>> ```
>> adb shell settings put system call_answer_vib 0
>> ```
># Disabling End Call Vibration
>> ```
>> adb shell settings put system call_end_vib 0
>> ```
>> ```
>> adb shell settings put global swipe_to_call_message 0
>> ```
># Changing phone name
>> ```
>> adb shell settings put secure bluetooth_name "device name"
>> ```
>> ```
>> adb shell settings put global device_name "device name"
>> ```
>> ```
>> adb shell settings put global synced_account_name "device name"
>> ```
># System Sounds and Vibrations
>*Disables some System Control Sounds and Vibrations such as:*
>Navigation
>> ```
>> adb shell settings put system navigation_gestures_vibrate 0
>> ```
>Lock Screen
>> ```
>> adb shell settings put system lockscreen_sounds_enabled 0
>> ```
>Camera
>>```
>>adb shell settings put system camera_feedback_vibrate 0
>>```
>Vibration in general
>>```
>>adb shell settings put system haptic_feedback_enabled 0
>>```
>>```
>>adb shell settings put system SEM_VIBRATION_FORCE_TOUCH_INTENSITY 0
>>```
>>```
>>adb shell settings put system SEM_VIBRATION_NOTIFICATION_INTENSITY 0
>>```
>>```
>>adb shell settings put system SEM_VIBRATION_RING_INTENSITY 5
>>```
>>```
>>adb shell settings put system vibrate_when_ringing 0
>>```
>>```
>>adb shell settings put system vibration_sound_enabled 0
>>```
>>```
>>adb shell settings put system VIB_FEEDBACK_MAGNITUDE 0
>>```
>>```
>>adb shell settings put system VIB_RECVCALL_MAGNITUDE 0
>>```
># Power Sounds
>>```
>>adb shell settings put global power_sounds_enabled 0
>>```
># Charging
>> ```
>> adb shell settings put secure charging_vibration_enabled 0
>> ```
>> ```
>> adb shell settings put secure charging_sounds_enabled 0
>> ```
># Bluetooth Audio Codecs
>> ```
>> adb shell settings put secure bluetooth_a2dp_bt_uhq_state 1
>> ```
>> ```
>> adb shell settings put secure bluetooh_a2dp_uhqa_support 1

># Google
>*Disabling Google Features, if you want to enable change 0 to 1*
>
> Android Auto
>> ```
>> adb shell settings put system gearhead:driving_mode_settings_enabled 0
>> ```
> GSM Tweak
>> ```
>> adb shell settings put secure assistant 0
>> ```
>> ```
>> adb shell settings put secure smartspace 0
>> ```
>> ```
>> adb shell settings put global google_core_control 0
>> ```
