

- Xcode
- Xcode Cloud
-  Configuring webhooks in Xcode Cloud 

Article

# Configuring webhooks in Xcode Cloud

Configure webhooks that connect Xcode Cloud to other services and tools.

## Overview

You might use custom services and tools in your development process and for project management purposes and need to connect them to Xcode Cloud. For example, you might want to show build information from Xcode Cloud on your team’s dashboard, automate the merge process for pull requests (PRs), automatically open or close issues in your issue tracking tool, and so on.

To connect Xcode Cloud with a custom tool or service, you need to configure an HTTPS endpoint that can receive HTTP requests from Xcode Cloud, referred to as a *webhook*. By configuring a webhook, you enable Xcode Cloud to send a rich JSON payload to another service or tool at certain moments during the build process. The service or tool can then parse the JSON payload and use the received information to provide its functionality.

Note

You can configure up to five webhooks per Xcode Cloud product.

Xcode Cloud sends an HTTP request to each webhook’s configured HTTPS endpoint every time it creates, starts, and finishes a build.

For more information about creating webhooks in Xcode Cloud, see Customize your advanced Xcode Cloud workflows.

### Create an Xcode Cloud webhook

To create a webhook in Xcode Cloud:

1.  In App Store Connect, choose an app and select the Xcode Cloud tab.

2.  In the sidebar, choose Settings \> Webhooks.

3.  Click the Add button (+) to add a new webhook.

4.  Choose a unique, easily recognizable name for the webhook, like “Team Dashboard” or “Issue Tracker”.

5.  Enter the URL of an app or service that’s capable of receiving and handling HTTPS requests.

When your service or tool receives a request from Xcode Cloud, respond with an HTTP status code that indicates success. If you return a retry-able server error or Xcode Cloud doesn’t receive a response within 30 seconds, it resends the webhook request until it receives a successful response.

Note

You need to configure a project or workspace to use Xcode Cloud before you can create a webhook.

### Debug a webhook

When you create a new webhook, plan to spend some time making sure your service or tool can parse the JSON payload that Xcode Cloud sends. To help you debug an integration problem, Xcode Cloud records a delivery report for each webhook request it sends. It includes detailed request and response metadata.

To access a webhook’s delivery report:

1.  In App Store Connect choose your app and select the Xcode Cloud tab.

2.  In the sidebar, choose Settings \> Webhooks.

3.  Choose a webhook and review its delivery reports.

### Review the payload

With each webhook request, Xcode Cloud includes detailed information about the app you configured in App Store Connect, the workflow that started the build, the build itself, your Git repository, and more. Use this information to provide functionality in your custom tool or service. For example, use the payload information to display Xcode Cloud build information on your team’s dashboard.

For more information on webhook payloads, see Xcode Cloud webhook payload reference.

The following code snippet shows the payload Xcode Cloud sends with a request:

```
```

## See Also

### Notifications

Xcode Cloud webhook payload reference

Review details of the webhook payload that Xcode Cloud sends, including the product, workflow, build, actions, results, and SCM metadata associated with it.

Connecting Xcode Cloud to Slack

Connect Xcode Cloud to Slack to keep your team informed about the latest Xcode Cloud builds.

