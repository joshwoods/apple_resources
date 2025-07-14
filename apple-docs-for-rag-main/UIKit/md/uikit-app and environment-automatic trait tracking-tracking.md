

- UIKit
- App and environment
-  Automatic trait tracking 

API Collection

# Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

## Overview

In iOS 18 and later, automatic trait tracking is a UIKit feature that eliminates the need to manually register for trait changes when you use traits in a supported method or closure. This feature reduces the amount of code you need to write and maintain, improves performance, and encourages the best practice of using traits within the scope of the supported APIs.

A complete list of APIs that support automatic trait tracking appears below.

## Topics

### Views

Views support automatic trait tracking when using traits from the trait collection of the view inside any of the following methods.

func layoutSubviews()

Lays out subviews.

func updateConstraints()

Updates constraints for the view.

func draw(CGRect)

Draws the view’s image within the passed-in rectangle.

### View controllers

View controllers support automatic trait tracking for both the trait collection of the view controller and the trait collection of its view inside any of the following methods.

func viewWillLayoutSubviews()

Notifies the view controller that its view is about to lay out its subviews.

func viewDidLayoutSubviews()

Notifies the view controller when its view finishes laying out its subviews.

func updateViewConstraints()

Notifies the view controller when its view needs to update its constraints.

func updateContentUnavailableConfiguration(using: UIContentUnavailableConfigurationState)

Updates the content-unavailable configuration for the provided state.

### Presentation controllers

Presentation controllers support automatic trait tracking for both the trait collection of the presentation controller and the trait collection of its container view inside any of the following methods.

func containerViewWillLayoutSubviews()

Notifies the presentation controller that layout is about to begin on the views of the container view.

func containerViewDidLayoutSubviews()

Notifies the presentation controller when layout ends on the views of the container view.

### Buttons

func updateConfiguration()

Updates the button configuration in response to a button state change.

var configurationUpdateHandler: UIButton.ConfigurationUpdateHandler?

A closure that executes when the button state changes.

### Collection view cells

func updateConfiguration(using: UICellConfigurationState)

Updates the cell’s configuration using the current state.

var configurationUpdateHandler: UICollectionViewCell.ConfigurationUpdateHandler?

A block for handling updates to the cell’s configuration using the current state.

### Table view cells

func updateConfiguration(using: UICellConfigurationState)

Updates the cell’s configuration using the current state.

var configurationUpdateHandler: UITableViewCell.ConfigurationUpdateHandler?

A block for handling updates to the cell’s configuration using the current state.

### Table view headers and footers

func updateConfiguration(using: UIViewConfigurationState)

Updates the view’s configuration using the current state.

var configurationUpdateHandler: UITableViewHeaderFooterView.ConfigurationUpdateHandler?

A block for handling updates to the view’s configuration using the current state.

### Collection view compositional layouts

The compositional layout section provider supports automatic trait tracking when using traits from the trait collection of the layout environment in the section provider.

typealias UICollectionViewCompositionalLayoutSectionProvider

A closure that creates and returns each of the layout’s sections.

## See Also

### Adaptivity

Responding to changing display modes on Apple TV

Change images and resources dynamically when the screen gamut on your device changes.

class UITraitCollection

A collection of data that represents the environment for an individual element in your app’s user interface.

protocol UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

protocol UIMutableTraits

A mutable container of traits.

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

protocol UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

