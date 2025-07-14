

- Accessibility
- Accessibility Inspector
-  Testing system accessibility features in your app 

Article

# Testing system accessibility features in your app

Confirm that your app provides a good experience for everyone by testing system accessibility settings in Accessibility Inspector.

## Overview

In Accessibility Inspector, the *Settings pane* provides quick access to common accessibility settings for easier testing. Use this pane to toggle these system-wide settings so you can test how your app behaves for a person who uses one or more of these accessibility features. Turning these settings on or off updates the corresponding setting in the Accessibility section of the target device’s system settings.

### Provide sufficient color contrast

People rely on accessibility features that increase contrast to improve the legibility of content. Ensure that your app provides sufficient color contrast and continues to provide a good experience when people turn on system settings that affect color. Listed below are the platform-specific accessibility settings that affect color contrast.

Tip

Accessibility Inspector provides a color contrast calculator to help you test the contrast for certain color combinations. To open this tool, choose Window \> Show Color Contrast Calculator (⌥⌘C).

#### All platforms

**Invert colors**. This option toggles the Invert Colors setting, which reverses the colors of the display with some behavior differences depending on the platform.

Default colors

Inverted colors

**Increase contrast**. This option toggles the Increase Contrast setting, which raises color contrast between app foreground and background colors.

Default contrast

Increased contrast

**Reduce transparency**. This option toggles the Reduce Transparency setting, which improves contrast and legibility by reducing transparency and blur effects on certain backgrounds.

Default transparency

Reduced transparency

#### iOS, watchOS, and tvOS

**Grayscale**. This option toggles the Grayscale setting, which removes color by rendering the UI as grayscale.

### Adjust animations to reduce onscreen motion

People with motion sensitivity can opt to decrease the amount of movement in screen elements, which can affect animations like parallax, animated images, and screen transitions. Ensure that your app doesn’t present any issues when a person chooses to reduce motion on their device. Listed below is the accessibility setting that affects motion in the UI.

#### All platforms

**Reduce motion**. This option toggles the Reduce Motion setting, which decreases motion in the UI like parallax and animations.

 Video with custom controls. 

 Content description: Example of content that uses significant motion in the UI when scrolling the content. 

Play 

Default motion

 Video with custom controls. 

 Content description: Example of content that uses minimal motion in the UI when scrolling the content with the reduce motion option. 

Play 

Reduced motion

### Support keyboard interaction

People can use an external hardware keyboard to control their devices, including iPhone. Ensure that your app works well with keyboard input, and test that your people can navigate and perform actions in your app using an external keyboard. Listed below is the accessibility setting that affects keyboard interaction.

#### All platforms

**Full Keyboard Access**. This option toggles the Full Keyboard Access setting, which allows a person to use an external keyboard to control the device.

### Communicate information without relying solely on color

People who are colorblind can find it difficult to distinguish between certain colors. Ensure that your app doesn’t rely solely on color to differentiate between objects or communicate important information, and test your app with these system settings. Listed below are the platform-specific accessibility settings that affect color.

#### All platforms

**Differentiate without color**. This option toggles the Differentiate Without Color setting, which replaces UI elements that rely solely on color to convey information.

#### iOS, watchOS, and tvOS

**Button shapes**. This option toggles the Button Shapes setting, which draws a more prominent UI for buttons to help differentiate them from noninteractive elements.

**On/Off labels**. This option toggles the On/Off Labels setting, which adds a label to each side of a switch to help reinforce which state it’s in.

### Ensure text is legible at any size

People can adjust the font weight and size on their devices to improve text legibility. Ensure that your app doesn’t make assumptions about font size, and your UI scales appropriately for different font weights and sizes. Listed below are the platform-specific accessibility settings that affect text legibility.

#### iOS, watchOS, and tvOS

**Bold fonts**. This option toggles the Bold Text setting, which increases the font weight for text throughout the system.

- Default fonts
- Bold fonts

**Dynamic type**. This option adjusts the system font size using Dynamic Type.

For more information about designing an accessible app, read Accessibility in Human Interface Guidelines.

