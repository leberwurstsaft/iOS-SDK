### Changelog

## VERSION 6.8.1
* SKOverlay Support: Using Apple's new SKOverlay to improve user's ad experience with a seamless presentation of the app store for app recommendation.
* vungleAdViewedForPlacement - new callback introduced to more accurately track ad impressions
* Stability Improvements

## VERSION 6.8.0
* iOS 14 Support, built on Xcode 12 - Connect to all iOS users including those on the latest version, iOS 14. Xcode 12 required.
* SkAdNetwork Support - Access all data sources to better understand your audience
* AppTrackingTransparency Support - Prepare for upcoming privacy changes and ensure users have more controls on their data usage.
* Updated StoreKit to be available for all formats - Create a seamless ad experience within your app in all formats.
* Removed Flex Feed and Flex View formats
* Stability improvements - Backend performance improvements to continually optimize your monetization efforts

## VERSION 6.7.1
* Removal of Moat framework
* Fixed issue with FMDB duplicate symbol
* Various bug fixes

## VERSION 6.7.0
* CCPA Support – Compliance with new government regulations while assuring your users their personal data is being used the way they want
* Multiple banner ad support – Display multiple banners on the screen txo leverage more ways to monetize your inventory and attract Premium Buyers
* Stability enhancements to continually ensure high performance
* Improved real-time ad play callbacks for click and rewarded events for a better end-user experience
* Improvements to orientation handling to improve end-user experience
* Backend performance improvements to continually optimize your monetization efforts
* Various bug fixes

## VERSION 6.5.3
* Bugs and issues resolved.

## VERSION 6.5.1
* Optimized caching logic to reduce data usage
* Added additional support for new banner sizes (320x50, 300x50, 728x90)
* Improved user experience and fixed issues related to Apple's StoreKit on iOS 13
* Improved how our SDK handles orientation settings and changes
* Eliminated main thread checker warnings
* Updated device information provider
* Made background webview of banner transparent
* Ad reporting improvements
* Removed VunglePlayAdOptionKeyBannerViewSize from pladAdOption
* Updated Moat version to 3.7.5
* Various bugs squashed and stability improvements

## VERSION 6.5.0
* Introduction of Banner Format
* Continuous improvements to ad caching
* Updated Moat framework
* Squashed many other bugs 

## VERSION 6.4.6
* Bug Fixes

## VERSION 6.4.5
* Updated Moat
* Bug Fixes

## VERSION 6.4.3
* iOS 13 Support and Enhancements
* Cache Optimization — Automatically optimizes ad caching to ensure ads are available faster. No additional work from developer needed.
* Introduced new MREC Video placement type to serve higher performing banners.
* Privacy by Design — Removed latitude and longitude collection to protect users.
* Updated Moat to no longer collect location data.
* Reduced App Store loading delay to reduce blank loading screens.
* Removed UIWebView references due to Apple no longer accepting submissions of apps that use UIWebView APIs.
* Publisher controls to override minimum disk requirements, helping to ensure good user experiences.

## VERSION 6.3.2
* Support for iOS 12
* StoreKit support for fullscreen MRAID ads
* Improved Moat viewability tracking
* Publishers can now track custom GDPR consent message versions
* MRAID ads now mute according to SDK option

## VERSION 6.3.1
* iOS 12 Compatibility
* Improved ad display on iPhone X
* Improved ad handling for placements
* Bug Fixes

## VERSION 6.3.0
* StoreKit support for MRAID ads
* Extend additional Moat support for our exchange
* Stability improvements

## VERSION 6.2.0
* GDPR compliance
* License updated
* Removed the requirement to have an auto-cached placement
* Removed the requirement to initialize Vungle SDK with all placements
* Bug fixes

## VERSION 5.4.0
* Fixed crashes on iOS 7
* Fixed crashes around Flex View layout logic
* Improved Flex View and Flex Feed stability
* Resolved duplicate symbol error on zipOpen4

## VERSION 5.3.2
* Sleep code to be enforced at placement level
* Ordinal data reporting
* iOS 11 API for safeAreaLayoutGuide for iPhone X
* Ability to close Flex-View ads through API or timer
* Bug fixes and performance improvements

## VERSION 5.3.0
* Allow cached ad to play when other placements are downloading
* Allow cached ad to play when there is no reception
* Fixed Flex View (ad unit) scaling issue
* Removed background dim in an interactive ad unit

## VERSION 5.2.0
* Fixed a regression of clickedThrough in internal reporting. Advertiser will see accurate clicks in dashboard
* Fixed user agent format for internal reporting
* Fixed an issue with application lifecycle that can result in black screens

## VERSION 5.1.1
* Made cache improvements
* Updated MOAT framework
* Added code to prevent SDK from initializing in iOS 7

## VERSION 5.1.0
* Launched new Placements feature.
* Added Native Flex View ad unit.
* Added Moat Viewability technology.
* Added GZIP for faster network transfers.
* Migrate MRAID to WKWebView on iOS 9 and 10 to address memory leak in UIWebView.
* Disabled iOS 7 support.

## VERSION 4.1.0
* Fix for occurrence of a black screen at the end of video.
* Cache improvements.
* Migrate to WKWebView for end cards on iOS 9 and 10 to address memory leak in UIWebView.
* Set user-agent in HTTP header to platform user agent for all external requests.
* StoreKit support for MRAID ads.

## VERSION 4.0.9
* Fix wrong behavior for the willCloseAdWithViewInfo: delegate method
* Improved SDK initialization
* Minor fixes and performance improvements
* Fix user-agent field on requests

## VERSION 4.0.8
* Refresh the IDFA when app comes to foreground
* Minor fixes

## VERSION 4.0.6
* Add cache early check to initial operation chain
* Prefix 3rd party zip/unzip lib functions
* Track and use the didDownload state for legacy ads

## VERSION 4.0.5
* Bug fixes
* Performance improvement

## VERSION 4.0.4
* iOS 10 OS performance optimizations
* CloudUX functionality support
* Vungle unique id implementation to maintain publisher frequency capping
* Fix click area around CTA button
* Resume video when app comes to foreground
* Add logging when the publisher uses a wrong appId


## VERSION 3.2.2
* Fix presenting modal view controller exception

## VERSION 3.2.1
* Bitcode support!
* Initialization prevention for devices under iOS 7.0
* Multiple initialization crash fix

## VERSION 3.2.0
* This SDK supports iOS 7+ devices only
* Enabled SSL as default for all internal network requests
* Improved caching performance
* Resolved race-condition crash around fetchConfig request
* Unified adPlayable behavior across flags & events
* Fix for playAd return code inconsistency during streaming ad plays
* Fix for progress bar location on smaller screens
* Fix for AppStore failing to load on some occasions
* Fix for issues resulting in inaccessible postroll

## VERSION 3.1.2
* Bug fixes

## VERSION 3.1.0
* API changed in Vungle delegate protocol: `vungleSDKhasCachedAdAvailable` changed to `vungleSDKAdPlayableChanged:`
* API changed in Vungle singleton: `isCachedAdAvailable` deprecated in favor of `isAdPlayable`
* New UI while playing video
* Bug fixes (background related bug, networking improvements)

## VERSION 3.0.13
* Minor Bug Fixes

## VERSION 3.0.12
* Fixes crash that happened on rare occasions when sending the app to the background
* Improves re-queuing of network requests. It should improve the ability to re-send requests even after they failed.
* Move saved /reportAds from cache directory to app support directory
* Option to modify incentivized alert text (title, body, close button, and continue button)

## VERSION 3.0.11
* Deprecated VunglePlayAdOptionKeyShowClose
* Deprecated VungleSDK#playAd: & VungleSDK#playAd:withOptions:
* Fixed some minor memory leaks
* Fixed orientations issues on iOS 8
* Fixed some random crashes on very limited edge cases
* Moved internal database from Documents to App Support

## VERSION 3.0.10
* Fixed crash that killed the app when sent to the background (in rare conditions)
* Fixed postroll and corrupted video bugs
* Improved support for iOS 8

## VERSION 3.0.9

* improved iOS 5 support
* fixed TPAT bugs

## VERSION 3.0.8

* added global playAd options
* added placements for each play, as well as dev-defined extra keys
* Fix a few mem leaks
* Send post params instead of query params for /sessionEnd
* miniz symbols no longer exposed
* Delegate methods are optional now