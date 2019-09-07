# VoiceOver Assisted iOS App
> I just added VoiceOver to the label and two buttons that this app originally used.

## Code
```SWIFT
// MARK: VoiceOver Code for Portal Dev Team
    // Resource: https://medium.com/@ericamillado/how-to-make-a-uilabel-accessible-swift-3-336b0839760d
    /// Setting up VoiceOver for label and buttons
    func setUpVoiceOver() {
        motorText.isAccessibilityElement = true
        forwardButton.isAccessibilityElement = true
        backwardButton.isAccessibilityElement = true

        motorText.accessibilityTraits = UIAccessibilityTraits.staticText
        forwardButton.accessibilityTraits = UIAccessibilityTraits.button
        backwardButton.accessibilityTraits = UIAccessibilityTraits.button

        // Motor Text
        motorText.accessibilityLabel = "fuck yeah"
        motorText.accessibilityValue = "this shit"
        motorText.accessibilityHint = "works"

        // Forward Button
        forwardButton.accessibilityLabel = "Foward Button"
        forwardButton.accessibilityValue = "Does nothing at the moment."
        forwardButton.accessibilityHint = "You can stop tapping it."

        // Backwards Button
        backwardButton.accessibilityLabel = "Backward Button"
        backwardButton.accessibilityValue = "Does nothing at the moment."
        backwardButton.accessibilityHint = "You can stop tapping it."
    }
```
## Resources
https://medium.com/@ericamillado/how-to-make-a-uilabel-accessible-swift-3-336b0839760d
