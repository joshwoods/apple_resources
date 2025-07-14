

- Core Services
- Launch Services
- 
  - Launch Services
- Deprecated Symbols
- LSLaunchFSRefSpec
-  passThruParams Deprecated

Instance Property

# passThruParams

A pointer to an Apple event descriptor that ispassed untouched as an optional parameter, with keyword `keyAEPropData` (`'prdt'`),in the Apple event sent to each application launched or activated(whether individual preferred applications or the application designatedby `appRef`). See the *AppleEvent Manager Reference* in the Carbon Interapplication CommunicationDocumentation for a description of the `AEDesc` datatype. The value of this field can be `NULL`.

macOS 10.0–10.10Deprecated

``` source
var passThruParams: UnsafePointer!
```

