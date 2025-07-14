

- TabularData
- JSONReadingOptions
-  addDateParseStrategy(\_:) 

Instance Method

# addDateParseStrategy(\_:)

Adds a date parsing strategy.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func addDateParseStrategy(_ strategy: T) where T : ParseStrategy, T.ParseInput == String, T.ParseOutput == Date
```

## Parameters 

`strategy`  

A parsing strategy that has a string input and a date output.

