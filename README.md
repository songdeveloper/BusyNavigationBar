# BusyNavigationBar
[![Version](https://img.shields.io/cocoapods/v/BusyNavigationBar.svg?style=flat)](http://cocoapods.org/pods/BusyNavigationBar)
[![License](https://img.shields.io/cocoapods/l/BusyNavigationBar.svg?style=flat)](http://cocoapods.org/pods/BusyNavigationBar)
[![Platform](https://img.shields.io/cocoapods/p/BusyNavigationBar.svg?style=flat)](http://cocoapods.org/pods/BusyNavigationBar)

A navigation bar extension to show loading effects above navigation bar's background.

## Screenshot



## Usage

BusyNavigationBar is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following lines to your Podfile:

```ruby
use_frameworks!
pod "BusyNavigationBar"
```
	
## Setup
```swift
var options = BusyNavigationBarOptions()

/// Color of the shapes. Defaults to gray.
options.color = UIColor.grayColor()

/// Alpha of the animation layer. Remember that there is also an additional (constant) gradient mask over the animation layer. Defaults to 0.5.
options.alpha = 0.5

/**
    Animation type

    - Stripes: Sliding stripes as seen in Periscope app.
    - Bars: Bars going up and down like a wave.
    - CustomLayer(() -> CALayer): Your layer to be inserted in navigation bar. In this case, properties other than `transparentMaskEnabled` and `alpha` will not be used. 
*/
options.animationType = .Stripes

/// Width of the bar. Defaults to 20.
options.barWidth = 20

/// Gap between bars. Defaults to 30.
options.gapWidth = 30

/// Speed of the animation. 1 corresponds to 0.5 sec. Defaults to 1.
options.speed = 1

/// Flag for enabling the transparent masking layer over the animation layer.
options.transparentMaskEnabled = true


```

## Properties
Soon

## Author

Günay Mert Karadoğan, mertkaradogan@gmail.com

## License

BusyNavigationBar is available under the MIT license. See the LICENSE file for more info.


