

- Application Services
-  Carbon Accessibility 

API Collection

# Carbon Accessibility

## Overview

This section describes the functions some Carbon developers may need to use to access-enable their applications.

This section describes the constants that define accessibility events and aspects of accessibility objects. The accessibility event constants are defined in `CarbonEvents.h` in the Carbon framework. The accessibility object constants are defined in header files in the ApplicationServices framework.

### Overview

This document describes the Carbon accessibility API. You use this API to make your Carbon application accessible to assistive applications and technologies, a process called access enabling.

#### Who Should Read This Document?

All Carbon application developers should read this document for information on specific functions and constants they may need to access-enable their applications. If you’re unsure which parts of the Carbon accessibility API you need, or if you’re new to accessibility in macOS, be sure to read the documents listed in See Also.

#### Organization of This Document

This document contains API reference in the following sections:

- Carbon Accessibility documents the functions some Carbon applications use to create and manipulate accessibility objects.

- Carbon Accessibility documents accessibility Carbon events and the constants that define the accessibility event parameters, object attributes, and notifications.

- Result Codes describes some of the error codes returned by the Carbon accessibility implementation.

#### See Also

For more information on accessibility in general and access enabling Carbon applications in particular, you should read the following documents:

- Getting Started With Accessibility

- Accessibility Programming Guide for OS X

- Accessibility Programming Guidelines for Carbon

## Topics

### Accessibility Events

Accessibility Event Class

Defines the event class for accessibility events.

### Accessibility Object Constants

Roles

Define the values an accessibility object’s role attribute can have.

Subroles

Define the values for an accessibility object’s subrole attribute.

Attributes

Define the attributes available for accessibility objects.

Parameterized Attributes

Define the parameterized attributes an accessibility object can have.

Actions

Define the actions an accessibility object can perform.

Notifications

Define the notifications that can be broadcast by an accessibility object.

Orientations and Sort Directions

Define the values for the orientation and sort-direction attributes of some accessibility objects.

### Result Codes

The result codes returned by the Carbon accessibility implementation are listed below. Other result codes defined in `AXError.h` are of use only to assistive applications.

case illegalArgument

The value received in this event is an invalid value for this attribute. This also applies for invalid parameters in parameterized attributes.

case invalidUIElement

The accessibility object received in this event is invalid.

case invalidUIElementObserver

The observer for the accessibility object received in this event is invalid.

case cannotComplete

A fundamental error has occurred, such as a failure to allocate memory during processing.

case attributeUnsupported

The referenced attribute is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case actionUnsupported

The referenced action is not supported. Alternatively, you can return the `eventNotHandledErr` error.

case apiDisabled

Assistive applications are not enabled in System Preferences.

case parameterizedAttributeUnsupported

The parameterized attribute is not supported. Alternatively, you can return the `eventNotHandledErr` error.

