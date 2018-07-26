# oneupSDK

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements

## Installation

### 1. Add Library with cocoapods
oneupSDK is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'oneupSDK'
```


### 2. Enable Bluetooth Background Mode

To allow the app to run in the background when in range of beacons, we need to enable the Bluetooth Background Mode in our Xcode project.

1. Select the project in the left sidebar, and on the right, go to “Capabilities”.
2. Flip the Background Modes to “ON”.
3. Expand the Background Modes section and check the “Uses Bluetooth LE accessories” option.

![background-mode.png](Documents/background-mode.png)

### 3. Define Location User Permission Description

In the project navigator, find the Info.plist file, right click on it, and select “Open As”, “Source Code”. Then, inside the top-level <dict> section, add:

	<key>NSLocationWhenInUseUsageDescription</key>
	<string>We'll show you cool things near you in the app.</string>
	
	<!-- iOS 10 or earlier -->
	<key>NSLocationAlwaysUsageDescription</key>
	<string>We'll show you cool things near you in the app, and alert you via
	notifications if you don't have the app open.</string>
	
	<!-- iOS 11 -->
	<key>NSLocationAlwaysAndWhenInUseUsageDescription</key>
	<string>We'll show you cool things near you in the app. With the "always" option,
	we can also alert you via notifications if you don't have the app open.</string>


## Author

Solutions Marketing OneUp Inc.

## License

oneupSDK is available under the MIT license. See the LICENSE file for more info.
