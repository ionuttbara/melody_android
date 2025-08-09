Melody Script for Android
Optimizes The Android Phone.
<h1 align="center">
  <br>
  <img src="https://raw.githubusercontent.com/jbara2002/melody12/master/logo.png" alt="Melody logo"></a>
</h1>

# Requiments
Android Phone with OS Version 7.1.1 or newer.
For Samsung Phones with OS Version 9 or newer (OneUI only).
ADB Installed with Drivers (the ADB Installer will be put in release and source code management).
# Commands

__YOU CAN CREATE A BAT FILE FROM THAT COMMANDS.__
The list of commands for
> # IMPROVING SYSTEM PERFORMANCE
>*Disables Window Blur Effects and animations*
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
> Improve Network Speeds by fixing signal quality (not for all devices)
>>```
>>adb shell settings put global preferred_network_mode 9,9
>>```
> # IMPROVING POWER MANAGEMENT ON PHONES
>*Improving the way the phone is sleeping by disable adaptive sleep algorithms.*
>*If you get delayed notifications of messaging applications, go to Settings, App, go to messaging app, battery and set to __Unrestricted__.*
>*Don't use 3rd Party or OEM Applications for doing that. I don't recommend doing that with them because the effect will be not desired as seen.*
>*Recommendation: Removing all 3rd Cleaning or Device Care Application for the algorithm to work correctly.*
>>```
>>adb shell settings put global sem_enhanced_cpu_responsiveness 0
>>```
>>```
>>adb shell settings put global enhanced_processing 0
>>```
>>```
>>adb shell settings put global app_standby_enabled 0
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
>>```
>>adb shell settings put global automatic_power_save_mode 0
>>```
>> # Disable Android Power Saver Mode, if you want to re-enable go to Setting or set *low_power* to 1 in command.
>>```
>>adb shell settings put global low_power 0
>>```
>>```
>>adb shell settings put global dynamic_power_savings_enabled 0
>>```
>>```
>>adb shell settings put global dynamic_power_savings_disable_threshold 20
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
># Disabling Swipe to Call/Messsage from Samsung Contacts App
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
>>```
>>adb shell settings put system sound_effects_enabled 0
>>```

>Enable Sync Vibration with Ringtone
>>```
>>adb shell settings put system sync_vibration_with_ringtone 1
>>```
>>```
>>adb shell setting put system sync_vibration_with_ringtone_2 1
>>```
>Enable Sync Vibration with Notification
>>```
>>adb shell settings put system sync_vibration_with_notification 1
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
>> ```
>> adb shell settings put secure adaptive_charging_enabled 0
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
>> ```
>> adb shell settings put secure adaptive_connectivity_enabled 0
>> ```
>> ```
>> adb shell settings put secure systemui.google.opa_enabled 0
>> ```
># Disable Android's Motion Engine Sensor (can save some battery) also disables some adaptive sleep bad features
>> ```
>> adb shell settings put system master_motion 0
>> ```
>> ```
>> adb shell settings put system motion_engine 0
>> ```
>> ```
>> adb shell settings put system air_motion_engine 0
>> ```
>> ```
>> adb shell settings put system air_motion_wake_up 0
>> ```
>> ```
>> adb shell settings put system intelligent_sleep_mode 0
>> ```
>> ```
>> adb shell settings put secure adaptive_sleep 0
>> ```
># Disabling Online Manual URL and Remote Support (Samsung ONE UI, All version with/o Tips Installed)
>>```
>>adb shell settings put global online_manual_url 0
>>```
>>```
>>adb shell settings put system remote_control 0
>>```
># Improve app launch times for Samsung Phones (and telemetry in Vanilla Android)
>>```
>>adb shell settings put global activity_starts_logging_enabled 0
>>```
>>```
>>adb shell settings put secure send_action_app_error 0
>>```
>>```
>>adb shell settings put global bixby_pregranted_permissions 0
>>```
>>```
>>adb shell settings put system send_security_reports 0
>>```
>>```
>>adb shell settings put system rakuten_denwa 0
>>```
># Audio Quality Improving in phones
>>```
>>adb shell settings put system tube_amp_effect 1
>>```
>>```
>>adb shell settings put system k2hd_effect 1
>>```
># Enable Multimedia Packet Scheduler (Also you can do by going in Developer Options from Settings)
>>```
>>adb shell settings put system multicore_packet_scheduler 1
>>```
># Killing Game Optimizing Service (GOS in Samsung) 👆GOS
>>```
>>adb shell settings put secure game_auto_temperature_control 0
>>```
>>```
>>adb shell pm clear --user 0 com.samsung.android.game.gos
>>```
>>```
>>adb shell settings put secure gamesdk_version 0
>>```
>>```
>>adb shell settings put secure game_home_enable 0
>>```
>>```
>>adb shell settings put secure game_bixby_block 1
>>```
># Block Galaxy System Updates (Policy and/or Device Update) (not interference with Galaxy Store Update or with F/OTA Updates)
>>```
>>adb shell settings put global galaxy_system_update_block 1
>>```
># OLED Screen Tweak
>>```
>>adb shell settings put global burn_in_protection 1
>>```
># Improve Touchscreen Responsiness and Latency on Android Phones
>>```
>>adb shell settings put secure tap_duration_threshold 0.0
>>```
>>```
>>adb shell settings put secure touch_blocking_period 0.0
>>```
># Disable Background Scanning for Devices (Bluetooth, Nearby Devices)
>>```
>>adb shell settings put system nearby_scanning_permission_allowed 0
>>```
>>```
>>adb shell settings put system nearby_scanning_enabled 0
>>```
>>```
>>adb shell settings put global ble_scan_always_enabled 0
>>```
># Disable hotword detection (OK Google, or Hey Google) in-background detection (improves baterry)
>>```
>>adb shell settings put global hotword_detection_enabled 0
>>```
># Another Samsung Phone Settings
>## Samsung Cross-Device Sync
>>```
>>adb shell settings put system mcf_continuity 0
>>adb shell settings put system mcf_continuity_permission_denied 1
>>adb shell settings put system mcf_permission_denied 1
>>```
>## Disable RAM Plus 
>>```
>>adb shell settings put global ram_expand_size_list 0
>>```
>>```
>>adb shell settings put global zram_enabled 0
>>```
># Refresh phone commands (these helps to refresh phone apps by a bit of boost)
>>```
>>adb shell cmd package compile -m speed-profile -a
>>adb shell cmd package bg-dexopt-job
>>adb shell pm trim-caches 999999999999999999
>>```
># Developer Options
>>```
>>adb shell settings put global development_settings_enabled 1
>>```
># Wifi Tweaks
>>```
>>adb shell settings put global wifi_poor_connection_warning 0
>>adb shell 
