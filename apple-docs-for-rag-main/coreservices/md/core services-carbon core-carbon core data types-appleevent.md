

- Core Services
- Carbon Core
- Carbon Core Data Types
-  AppleEvent 

Type Alias

# AppleEvent

A descriptor whose data is a list of descriptors containing both attributes and parameters that make up an Apple event.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AppleEvent = AERecord
```

## Discussion

The Apple event data type describes a full-fledged Apple event. Like the data for an Apple event record (data type AERecord), the data for an Apple event consists of a list of keyword-specified descriptors. Unlike an Apple event record, the data for an Apple event is conceptually divided into two parts, one for attributes and one for parameters. This division within the Apple event allows the Apple Event Manager to distinguish between an event’s attributes and its parameters.

Many functions work with Apple events, including the functions described in Apple Event Manager, Apple Event Manager, Creating an Apple Event, and Sending an Apple Event.

