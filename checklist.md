## 8bytes iOS / Android Checklist


|  |  |
|:-------------------------------------|-------------------------------------:|
| App name                             |      *insert content*                |
| Version                              |      *insert content*                |
| Date of submission                   |      *insert content*           |


This is to ensure we cover ourselves for any easily avoidable issues. 

--

### View Controller life cycles

All View controllers should have up to date information and refresh with the server for:
- Initial Load
- On app foreground
- On Reachability Reconnect
- Other

### Devices

Run the application through navigations using different devices with different iOS versions and display formats.

- iPhone 4s
- iPhone 5
- iPhone 6
- iPhone 6s+

- iPad
- iPad Split Screen

--

### Audio
If app plays audio, perform the following checks.

- Headphones/speaker routing
- Dock connector audio out routing
- Mute switch functionality (officially it mutes non-user-requested sounds)
- Audio pause on received phone call
- Background audio (if supported): playback and multitasking bar controls
- Start playing audio when another app is already playing
- Headphone remote for audio control
- Multitasking screen audio control

--

### Video

- User cancels video before playback begins
- User cancels video during playback 
- Video plays to the end
- Video return from full screen
- Dock connector video out
- Video transition between inline and full screen

--

### Location

- Gracefully asked for location permission
- Deals with no permissions
- Deals with change of permissions
- Deals with no location returned


### Logging

Android:
- Turn off Logging

--

### User Interface
Test each major view in the app.

- Double height status bar (eg in call)
- Orientation change
- Upside-down orientation
- Orientation lock 

--

### Installation

- Fresh install 
- Upgrade from previous live version
- Upgrade from older live version


--

### Third Party Services
All third party services should use production API key and the new app version should be registered in the respective dashboards

- Turn off netfox
- Upload dSYM to Crashlytics
- Turn on Answers  
- Turn off Enviorment Switcher
- Production App ID for social services (Twitter, Facebook, Instagram, etc)
- Production App ID for Stripe

Android Only:
- Turn off Leaky Canary
- Turn off Stethoscope


--

Sign-off: __________________________________________  
