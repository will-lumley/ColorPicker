![ColorPicker: Elegant Color Picking](https://raw.githubusercontent.com/will-lumley/macColorPicker/main/ColorPicker.png)

# macColorPicker

<p align="center">
  <img src="https://github.com/will-lumley/macColorPicker/actions/workflows/BuildTests.yml/badge.svg?branch=main" alt="macOS - CI Status">
</p>
<p align="center">
  <a href="https://github.com/apple/swift-package-manager"><img src="https://img.shields.io/badge/SPM-compatible-4BC51D.svg?style=flat" alt="SPM Compatible"></a>
  <img src="https://img.shields.io/badge/Swift-5.5-orange.svg" alt="Swift 5.5">
  <a href="https://bsky.app/profile/will-lumley.bsky.social">
    <img src="https://img.shields.io/badge/Bluesky-0285FF?logo=bluesky&logoColor=fff&label=will-lumley" alt="Bluesky">
  </a>
</p>

macColorPicker is a tiny, pure Swift library designed for macOS applications that allows you to let your users easily choose a color.

macColorPicker allows you to present the user with a preset range of colors to choose from. As the developer, you get to choose how these are formatted, how they look, and what happens when a user makes a selection.
If you want to give the user more control, you can also allow them to select a button that presents the `NSColorPanel`.

## Usage

macColorPicker is a subclass of `NSView` so you can simply add ColorPicker like you would any other view, whether it be to your storyboard, XIB, or just in code. 
Configuring ColorPicker's `delegate` allows you to be notified when the ColorPicker view is about to be presented, when is has been presented, or when a user has selected a color.


https://user-images.githubusercontent.com/14086082/116811221-6fd58480-ab8b-11eb-9e3f-a19fb3f83caa.mov

## Example Project

To run the example project, clone the repo, and open the example Xcode Project in RichEditorExample.

## Requirements

macColorPicker supports macOS 10.12 and above.

## Installation

### Swift Package Manager
macColorPicker is also available through [Swift Package Manager](https://github.com/apple/swift-package-manager). 
To install it, simply add the dependency to your Package.Swift file:

### Cocoapods and Carthage
macColorPicker was previously available through CocoaPods and Carthage, however making the library available to all three Cocoapods, 
Carthage, and SPM (and functional to all three) was becoming troublesome. This, combined with the fact that SPM has seen a serious
up-tick in adoption & functionality, has led me to remove support for CocoaPods and Carthage.

```swift
...
dependencies: [
    .package(url: "https://github.com/will-lumley/macColorPicker.git", from: "1.3.0"),
],
targets: [
    .target( name: "YourTarget", dependencies: ["macColorPicker"]),
]
...
```
## Author

[William Lumley](https://lumley.io/), will@lumley.io

## License

macColorPicker is available under the MIT license. See the LICENSE file for more info.
