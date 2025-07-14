

- WatchKit
- Storyboard support
-  Building watchOS app Interfaces Using the Storyboard 

# Building watchOS app Interfaces Using the Storyboard

Create the user interface for your watchOS app by nesting stacks.

## Overview

watchOS apps use a simplified, stack-based layout model for their user interfaces. Xcode automatically groups elements into horizontal and vertical stacks, and you can fine-tune the layout by modifying the element’s attributes. Additionally, you can ensure that your interface works as expected on all Apple Watch sizes by using resizable elements and size-specific customizations.

As you add items to the storyboard, Xcode stacks them vertically, with each item on its own line (Figure 1).

Use Groups to create horizontal or vertical stacks (Figure 2). Groups don’t have a default visual representation, but you can configure a background color or image as needed. Nest Groups, as necessary, to create more complex layouts.

### Customize the Layout Using Attributes

You can fine-tune an interface element’s size and layout using the Attributes inspector. All interface elements have the following attributes:

Horizontal  
Configures the horizontal position of the item within the space provided by its container.

Vertical  
Configures the vertical position of the item within the space provided by its container.

Width  
Determines how the system calculate’s the object’s width. This attribute has three possible values: Size to Fit Content, Relative to Container, and Fixed. Size to Fit Content sets the width based on the object’s content. Relative to Container sets the width to a percentage of the container’s width. Fixed sets the width to the specified size in points.

Height  
Determines how the system calculate’s the object’s height. This attribute has three possible values: Size to Fit Content, Relative to Container, and Fixed. Size to Fit Content sets the height based on the object’s content. Relative to Container sets the height to a percentage of the container’s height. Fixed sets the height to the specified size in points.

Groups provide additional options to manage their content:

Layout  
Specifies the layout direction for items in the group. You can stack items horizontally or vertically, or have them overlap.

Insets  
Sets the amount of space (in points) between the edges of the group and its child elements. Use Custom to specify different values for the top, bottom, left, and right edges.

Spacing  
Sets the spacing (in points) between child elements in the group. The default spacing is 2 points.

## Topics

### Controls

Connecting Your User Interface to Your Code

Connect the interface objects in your storyboard to outlets and action methods in your WatchKit extension.

### Navigation

Navigating Between Scenes

Help users navigate between interface controllers.

## See Also

### User interface basics

class WKInterfaceObject

An object that provides information that is common to all interface objects in your watchOS app.

class WKInterfaceController

A class that provides the infrastructure for managing the interface in a watchOS app.

class WKAlertAction

An object that encapsulates information about a button displayed in an alert or action sheet.

class WKAccessibilityImageRegion

An object that defines a portion of an image that you want to call out separately to an assistive app.

func WKAccessibilityIsVoiceOverRunning() -> Bool

Returns a Boolean value indicating whether VoiceOver is running.

func WKAccessibilityIsReduceMotionEnabled() -> Bool

Returns a Boolean value indicating whether reduced motion is enabled.

