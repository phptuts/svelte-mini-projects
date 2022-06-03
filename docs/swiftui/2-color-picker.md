# Color Picker

Create a color picker with 3 Slider that shows the hex value of the color, percentages of red, green and blue and the actual color in a SwiftUI Rectangle.

<iframe width="560" height="315" src="https://www.youtube.com/embed/2P_B2Ux0e_0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## [Code](https://github.com/phptuts/ios-mini-projects/blob/main/ColorPicker/ColorPicker/ContentView.swift)



## Code To Copy

```swift
extension Color {
    func hexString() -> String {
        let components = self.cgColor?.components
        let r: CGFloat = components?[0] ?? 0.0
        let g: CGFloat = components?[1] ?? 0.0
        let b: CGFloat = components?[2] ?? 0.0

        let hexString = String.init(format: "#%02lX%02lX%02lX", lroundf(Float(r * 255)), lroundf(Float(g * 255)), lroundf(Float(b * 255)))
        return hexString
    }
}

extension Double {
    func toPercent() -> String {
        String(format:"%6.2f%%",self * 100)
    }
}
```


## Resources

- [Discord](https://discord.gg/Jwv7xaPRMS)
- [SwiftUI Slider](https://www.hackingwithswift.com/quick-start/swiftui/how-to-create-a-slider-and-read-values-from-it)
- [SwiftUI Rectangle](https://www.hackingwithswift.com/quick-start/swiftui/how-to-display-solid-shapes)
- [State](https://www.hackingwithswift.com/quick-start/swiftui/what-is-the-state-property-wrapper)
