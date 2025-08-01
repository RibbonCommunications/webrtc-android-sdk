# Change Log

Ribbon WebRTC Android SDK change log.

- This project adheres to [Semantic Versioning](http://semver.org/).
- This change log follows [keepachangelog.com](http://keepachangelog.com/) recommendations.

## 6.36.0 - 2025-31-07
### Added
- Custom SIP Headers input for Demo Apps. `KAE-1593`

## 6.35.0 - 2025-27-06
### Changed
- User Guide documentation updated. `KAE-1592`

## 6.34.0 - 2025-04-30

## 6.33.0 - 2025-03-12

## 6.32.0 - 2024-11-29

## 6.31.0 - 2024-11-01

## 6.30.0 - 2024-09-23

### Changed
- Call Service migrated to Kotlin `KAE-1580`

## 6.29.0 - 2024-08-20

### Changed
- WebRTC migrated to Kotlin `KAE-1578`

## 6.28.0 - 2024-07-23

## 6.27.0 - 2024-06-24

### Changed
- Rest Manager migrated to Kotlin `KAE-1570`

## 6.26.0 - 2024-05-24

### Changed
- Notification Engine migrated to Kotlin `KAE-1567`

## 6.25.0 - 2024-04-29

## 6.24.0 - 2024-03-29

## 6.23.0 - 2024-02-26

## 6.22.2 - 2024-02-20

### Changed
- ScaleType xml resource name changed

## 6.22.1 - 2024-02-06

### Changed
- Maven Artifactory server is changed

### Fixed
- Maven Artifactory server is now reachable
- Javadoc paths is reconfigured with requirements of Gradle 8.5-rc-1

## 6.22.0 - 2023-01-30

## 6.21.0 - 2023-12-29

## 6.20.0 - 2023-12-07

### Added 
- Upgrading WebRTC to M118. `KAE-1544`

## 6.19.0 - 2023-11-14

### Added 
- Build Gradle version updated to 8.5-rc-1 `KAE-1542`

## 6.18.0 - 2023-10-04

## 6.17.0 - 2023-09-04

### Added 
- Build Gradle version updated to 6.5 `KAE-1533`

### Changed
- Sending GET request for Call State to initiate Incoming Call `KAE-1535`

## 6.16.0 - 2023-08-03

## 6.15.0 - 2023-07-04

## 6.14.0 - 2023-05-30

 ### Added
 - KAE-1503 Added External Audio Source 
 ### Fixed
 - KAE-1505 Unit Test Fixes

## 6.13.0 - 2023-02-05

## 6.12.0 - 2023-27-03

### Added 
- Upgrading WebRTC to M110. `KAE-1483`

## 6.11.0 - 2023-28-02

## 6.10.0 - 2023-24-01

## 6.9.0 - 2022-26-12

## 6.8.0 - 2022-31-10

### Added
- Registration Service and Notification Manager refactored. `KAE-1352`

## 6.7.0 - 2022-3-10

## 6.6.0 - 2022-31-08

### Added 
- Video mute/unMute API. `KAE-1338`

## 6.5.0 - 2022-02-08

## 6.4.0 - 2022-28-06

### Changed
- Ringing feedback types are refactored. `KAE-1267`
- The SDK no longer will not operate the re-register operation when it receive gone notification. `KAE-1180`

### Fixed
- Remote video view freeze issue is fixed. `KAE-1300`
- Creating offer SDP with wrong payload numbers issue fixed. `KAE-1306`

## 6.3.0 - 2022-27-05

## 6.2.0 - 2022-25-04

## 6.1.0 - 2022-28-03

## 6.0.0 - 2022-28-02

### Added 
- Upgrading WebRTC to M97. `KAE-1153`
    - With the M97 upgrade, WebRTC backward compatibility is broken, so there might be problem with Cisco and Transfer calls.
### Fixed
- Fixed an issue where WebRTC could not parse SDP due to space on the codec list. `KAE-1222`

## 5.24.0 - 2022-03-01

### Added 
- Public Request API. `KAE-1165`

## 5.23.0 - 2021-11-03

### Removed
- `setRingingFeedbackEnabled(boolean ringingFeedbackEnabled)` was removed.
- `isRingingFeedbackEnabled()` was removed.
- `getLoginType()` was removed.
- `setLoginType(Constants.LoginType loginType)` was removed.

## 5.22.0 - 2021-09-27

## 5.21.1 - 2021-08-25

### Fixed
- Call initializing issue after consecutive call fixed.

## 5.21.0 - 2021-08-16

### Added
- JavaWebSocket version updated to 1.5.1.

## 5.20.0 - 2021-06-29

### Added
- Remote video scaling type change support added.

## 5.19.0 - 2021-06-01

### Added
- Authentication with hmac token support added.

## 5.18.0 - 2021-04-26

## 5.17.0 - 2021-03-26

### Added
- `List<Map> getAvailableCodecs(CodecType codecType)` added to Call class in order to get available codec attributes.

## 5.16.0 - 2021-02-26

### Removed
- `registerToServer(final Constants.SubscribeServices[] serviceTypes, final int expirationTime, final OnCompletionListener listener)` was removed.

## 5.15.0 - 2021-02-04

### Deprecated
- `isRingingFeedbackEnabled` and `setRingingFeedbackEnabled` added to Configuration class methods are deprecated and will be removed in future releases. Instead `ringingFeedbackOptions` and `setRingingFeedbackOptions` should be used. 

## 5.14.0 - 2020-12-30

### Deprecated
- `registerToServer(final Constants.SubscribeServices[] serviceTypes, final int expirationTime, final OnCompletionListener listener)` API in the RegistrationService will be deprecated in the version 5.16.0. But a new `registerToServer(final int expirationTime, final OnCompletionListener listener)` is introduced. Therefore developers should take the necessary action. `KAE-806`

- `DTLS`, `securedWSProtocol`, `requestProtocolHttp`, `kandyVersion`, `kandyToken`, `deviceId`, `deviceNativeId`, `sendKandyTokenInRestHeader`, `connectionType`, `auditEnable`, `supportedCallFeautes`, `notificationType` parameters removed from Configuration class. `KAE-869`

### Added
- `isRingingFeedbackEnabled` and `setRingingFeedbackEnabled` added to Configuration class in order to set and/or check ringing feedback feature.
- `registerToServer(final int expirationTime, final OnCompletionListener listener)` API added to RegistrationService. `KAE-806`

### Renamed
- `replaceCodecSet` parameter renamed as `codecPayloadTypeSet` in Configuration class. `KAE-869`

## 5.13.0 - 2020-12-02

### Fixed
- Crash when the application native dial pad is used is fixed. `KAE-865`

## 5.12.0 - 2020-11-04

## 5.11.0 - 2020-10-05

### Changed
- Return type of `CallInterface.getRTPStatistics` was changed as `NSString`

## 5.10.0 - 2020-08-28

## 5.9.0 - 2020-07-22

## 5.8.0 - 2020-07-03

## 5.7.0 - 2020-06-12

## 5.6.0 - 2020-05-04

### Fixed
- After Session Complete notification the end call DELETE request must be sent. `KAE-669`

## 5.5.0 - 2020-03-30

## 5.4.0 - 2020-03-02

### Added
- Adding configuration property for control TCP keep alive `KAE-571`

## 5.3.0 - 2020-01-09

### Added
- Call forward feature `KAE-80`


## 5.2.0 - 2019-12-02

### Added
- WebRTC stack upgraded to version M78 `KAE-507`
- Custom Kandy Agent HTTP Header is implemented `KAE-524`

### Deprecated
- `CallService.createOutgoingCall(String, CallApplicationListener, OutgoingCallCreateInterface)`, `CallService.createOutgoingCall(String, String, CallApplicationListener, OutgoingCallCreateInterface)`, `CallService.createOutgoingCall(String, String, String, CallApplicationListener, OutgoingCallCreateInterface)` and `CallService.createThreeWayCall(String, String, CallApplicationListener, OutgoingCallCreateInterface)` methods are deprecated and will be removed in future releases, since `CallApplicationListener` can already be set to CallService via a setter method. Instead `CallService.createOutgoingCall(String, OutgoingCallCreationCallback)`, `CallService.createOutgoingCall(String, String, OutgoingCallCreationCallback)`, `CallService.createOutgoingCall(String, String, String, OutgoingCallCreateInterface)` and `CallService.createThreeWayCall(String, String, OutgoingCallCreateInterface)` should be used.


## 5.1.0 - 2019-11-04

### Fixed
- Default value for codec preferrence is set to reflect WebRTC default codec behavior `KAE-538`


## 5.0.0 - 2019-10-03

### Added
- Unified Plan Support `KAE-200`
- Mobile SDK Distribution on Maven `KAE-425`
- Support Custom SIP headers in Incoming Call `KAE-447`
- Callee Name api added to CallInterface `KAE-475`


## 4.6.2 - 2019-09-02

### Fixed
- Media problem when switching between two calls on Music-on-Hold is fixed `KAE-410`


## 4.6.1.1 - 2019-08-05


## 4.6.1 - 2019-07-05

### Added
- Bandwidth limitation feature implemented `KAE-63`

### Fixed
- A fix provided for race condition case during WebRTC audio module creation when a second call session is being initiated. `KAE-435`
- A fix provided for 3-way call fail when early notification is received. `KAE-455`


## 4.6.0 - 2019-06-01

### Added
- PushService for CPaaS push notifications support. `KAE-350`

### Changed
- EventService is renamed as PushService. Its method `receiveNotification` which passes push notifications to Mobile SDK is replaced with `injectPushMessage`. `KAE-350`

### Fixed
- HTTP 4xx and 5xx responses are coded with a new error code and reported with MobileError. `KAE-288`


## 4.5.9.1 - 2019-05-06

### Fixed
- Hardware support of "Acoustic Echo Canceler" and "Noise Suppressor" configuration is fixed `KAE-369`


## 4.5.9 - 2019-05-02

### Changed
- Package name for VideoView is changed to "com.genband.mobile.core.webrtc.view". `KAE-368`
