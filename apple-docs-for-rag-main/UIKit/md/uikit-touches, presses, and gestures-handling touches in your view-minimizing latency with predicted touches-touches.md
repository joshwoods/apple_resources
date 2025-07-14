

- UIKit
- Touches, presses, and gestures
- Handling touches in your view
-  Minimizing latency with predicted touches 

# Minimizing latency with predicted touches

Create a smooth and responsive drawing experience using UIKit’s predictions for touch locations.

## Overview

It takes time for UIKit to generate and deliver touch events to your app, and it takes time for your app to process those events and render the results. In fact, it takes enough time that there can be a visible lag between the movements of a person’s finger or Apple Pencil and the rendered results. To minimize the perceived latency between touch input and rendered content, you can incorporate predicted touches into your event handling.

Predicted touches are the system’s best guess of where the next touch events will occur. The following image illustrates the concept in a drawing app. When a drawing sequence begins, UIKit uses previous touch locations from a person’s finger or Apple Pencil to predict where the next touch may occur. UIKit generates additional UITouch objects for these predicted locations and makes them available to your app.

To retrieve predicted touch data, call the predictedTouches(for:) method of the UIEvent object containing the original UITouch object. That method returns an array of touches predicted to occur after the last actual touch. Always treat predicted touches as temporary data in your app and discarded them upon receipt of each new touch event.

## Topics

### Example

Incorporating predicted touches into an app

Learn how to create a simple app that incorporates predicted touches into its drawing code.

## See Also

### Advanced touch handling

Implementing a Multi-Touch app

Learn how to create a simple app that handles multitouch input.

Getting high-fidelity input with coalesced touches

Learn how to support high-precision touches in your app.

