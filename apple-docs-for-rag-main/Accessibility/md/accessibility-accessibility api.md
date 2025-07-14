

- Accessibility
-  Accessibility API 

API Collection

# Accessibility API

Browse API in the Accessibility framework.

## Overview

While many Apple frameworks provide built-in accessibility support, the Accessibility framework defines API for supporting additional accessibility features across multiple platforms. The Accessibility framework includes API that enable you to:

- Respond to changes in Accessibility system settings

- Post accessibility notifications

- Define an accessible representation of your chart to support audio graphs

- Interact with hardware such as braille displays and hearing devices

- Generate a localized description of a color

## Topics

### System settings

struct AccessibilitySettings

A structure for working with accessibility system settings.

### Notifications

enum AccessibilityNotification

Types of accessibility notifications that an app can post.

### Assistive technologies

struct AccessibilityTechnology

static let automation: AccessibilityTechnology

static let fullKeyboardAccess: AccessibilityTechnology

static let hoverText: AccessibilityTechnology

static let speakScreen: AccessibilityTechnology

static let switchControl: AccessibilityTechnology

static let voiceControl: AccessibilityTechnology

static let voiceOver: AccessibilityTechnology

static let zoom: AccessibilityTechnology

class AccessibilityRequest

### Features

Customized accessibility content

Customize your apps to deliver accessibility information to your users in measured portions as they need it.

Audio graphs

Define an accessible representation of your chart for VoiceOver to generate an audio graph.

Braille displays

Display a graphical representation of images, icons, data, and more on a two-dimensional braille display.

Hearing device support

Access information about paired hearing aid devices and streaming status.

func AXNameFromColor(CGColor) -> String

Returns a localized description of the color to use in accessibility attributes.

### Deprecated

func AXAnimatedImagesEnabled() -> Bool

Returns a Boolean value that indicates whether the system setting for Animated Images is on.

Deprecated

func AXPrefersHeadAnchorAlternative() -> Bool

Returns a Boolean value that indicates the person’s preference for content that follows their head position.

Deprecated

func AXPrefersHorizontalTextLayout() -> Bool

Returns a Boolean value that indicates whether the system setting for Prefer Horizontal Text is on.

Deprecated

