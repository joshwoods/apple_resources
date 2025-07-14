

- Application Services
- Carbon Accessibility
-  Parameterized Attributes 

API Collection

# Parameterized Attributes

Define the parameterized attributes an accessibility object can have.

## Overview

Parameterized attributes allow you to pass in additional values to get more specific information about the text associated with an accessibility object.

## Topics

### Constants

var kAXLineForIndexParameterizedAttribute: String

Given an indexed character, the line number of the text associated with this accessibility object that contains the character.

var kAXRangeForLineParameterizedAttribute: String

Given a line number, the range of characters of the text associated with this accessibility object that contains the line number.

var kAXStringForRangeParameterizedAttribute: String

A substring of the text associated with this accessibility object that is specified by the given character range.

var kAXRangeForPositionParameterizedAttribute: String

var kAXRangeForIndexParameterizedAttribute: String

var kAXBoundsForRangeParameterizedAttribute: String

The bounding rectangle of the text associated with this accessibility object that is specified by the given range. This is the bounding rectangle a sighted user would see on the display screen, in pixels.

var kAXRTFForRangeParameterizedAttribute: String

The RTF representation of the text associated with this accessibility object that is specified by the given range.

var kAXAttributedStringForRangeParameterizedAttribute: String

The CFAttributedStringType representation of the text associated with this accessibility object that is specified by the given range.

var kAXStyleRangeForIndexParameterizedAttribute: String

Given a character index, the range of text associated with this accessibility object over which the style in effect at that character index applies.

## See Also

### Accessibility Object Constants

Roles

Define the values an accessibility object’s role attribute can have.

Subroles

Define the values for an accessibility object’s subrole attribute.

Attributes

Define the attributes available for accessibility objects.

Actions

Define the actions an accessibility object can perform.

Notifications

Define the notifications that can be broadcast by an accessibility object.

Orientations and Sort Directions

Define the values for the orientation and sort-direction attributes of some accessibility objects.

