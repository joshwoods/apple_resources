

- Matter
-  MTRStorage 

Protocol

# MTRStorage

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
protocol MTRStorage : NSObjectProtocol
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Instance Methods

func removeStorageData(forKey: String) -> Bool

**Required**

func setStorageData(Data, forKey: String) -> Bool

**Required**

func storageData(forKey: String) -> Data?

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MTRPersistentStorageDelegate

