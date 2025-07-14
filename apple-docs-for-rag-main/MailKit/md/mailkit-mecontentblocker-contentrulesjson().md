

- MailKit
- MEContentBlocker
-  contentRulesJSON() 

Instance Method

# contentRulesJSON()

The rules, as JSON data, that the system applies when it displays a message.

macOS 12.0+

``` source
func contentRulesJSON() -> Data
```

**Required**

## Return Value

A data object that contains valid JSON content.

## Discussion

MailKit relies on WebKit to block content. Therefore, the JSON structure is the same that a content blocker extension for Safari uses. For details about the structure of the JSON to specify the content-blocking rules, see Introduction to WebKit Content Blockers.

The following code shows an example of a content blocker that uses a rule to hide all links from a specific domain:

```
func contentRulesJSON() -> Data {
    // A single rule that visually hides all links to example.com.
    let rules = [
        [
            "action": [
                "type": "css-display-none",
                "selector": "a[href*='example.com']"
            ],
            "trigger": [ "url-filter": ".*" ]
        ]
    ]

    // Serialize the array of rules to JSON.
    let data = try? JSONSerialization.data(withJSONObject: rules, options: [])

    // Return the encoded rules, or an empty data if encoding failed.
    return data ?? Data()
}
```

