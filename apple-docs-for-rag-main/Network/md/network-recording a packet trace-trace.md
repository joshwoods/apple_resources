

- Network
-  Recording a Packet Trace 

# Recording a Packet Trace

Learn how to record a low-level trace of network traffic.

## Overview

A packet trace is a record of traffic traveling across the network. It’s useful for investigating complex network problems related to both correctness and performance.

Once you start a packet trace on a network interface, it records all traffic passing through that interface until you stop the trace. Packet traces are usually quite short — perhaps recording the traffic associated with one specific connection — but there are situations where you might want to run the trace for hours or even days.

Both macOS and iOS have built-in support for packet traces. This article explains how to record a packet trace on both platforms. Even if your primary focus is iOS, you should start by running some tests on macOS to familiarize yourself with the tools before you attempt to debug your actual problem.

Note

Packet traces are a low-level feature and, if you’re just getting started, you may be better off using one of the higher-level tools referenced in Choosing a Network Debugging Tool. Additionally, while the focus of this article is the built-in packet trace tools, there are a variety of third-party packet trace tools that you might want to investigate; see Taking Advantage of Third-Party Network Debugging Tools for details.

### Choose the Correct Interface

The first step in recording a packet trace on the Mac is to choose the correct interface. If you choose the wrong interface, you may end up recording an empty packet trace. For example, if you use the `en0` interface on a Mac that has built-in Ethernet but is connected to the Internet over Wi-Fi, your packet trace will include all the traffic over the built-in Ethernet, that is, nothing.

Determine the correct interface name by running the `networksetup` command-line tool with the `-listallhardwareports` argument. This prints a list of network interfaces, including both the user-visible name and the short interface name needed by packet trace tools. For example:

```
```

In this example, the built-in Ethernet is `en0` and the built-in Wi-Fi is `en1`, but this will change from machine to machine. Look through this list for the user-visible name of the interface you want to trace (these match the names shown in Network preferences), then use the associated short interface name.

### Record and Analyze a Packet Trace on a Mac

Working with packet traces usually involves recording a packet trace to a file and analyzing that file. It’s possible to do both steps at once, and it’s a good idea to do that when you’re just getting started. The following Terminal command starts a packet trace and prints information about each packet as it’s transferred.

```
```

In this example:

- `tcpdump` is the name of macOS’s built-in packet trace tool.

- The `sudo` command causes `tcpdump` to run with privileges, which is necessary in order to record packets.

- The `-i en0` option tells `tcpdump` to record packets on the default Ethernet-like interface. Replace `en0` with the short interface name you determined in Choose the Correct Interface.

- The `-n` option tells tcpdump not to attempt to use reverse DNS to map IP addresses to names; such mapping is rarely useful on the modern Internet and it radically slows things down.

When you run `tcpdump` in this way, you see something like this:

```
```

There’s a line of output for each packet seen on the network. On each line there’s a timestamp and a lot of information about that packet. This specific example shows the start of a connection from an SSH client at 192.168.1.187 to an SSH server listening on port 22 of 192.168.1.39.

Packet traces can be quite overwhelming. Rather than trying to interpret the packet trace in real time, use the `-w` option to write the trace to a file and then do your analysis later on.

```
```

This example records a packet trace and writes the results to a file call `trace.pcap`. You can save that file to analyze later on using `tcpdump` itself, or one of the tools listed in Taking Advantage of Third-Party Network Debugging Tools. You can also submit it to Apple for analysis (see Submitting a Packet Trace to Apple).

Important

Even if your ultimate goal is to save a packet trace file, it’s often a good idea to start out by looking at real-time results from `tcpdump`, just to make sure that you’re capturing the right thing.

If you’re having problems recording a packet trace, see Troubleshooting Packet Traces.

### Set Up iOS Packet Tracing

iOS doesn’t let you record a packet trace directly. However, you can use your Mac to record a packet trace on an attached iOS device using the Remote Virtual Interface (RVI) mechanism. To get started, first connect your iOS device to your Mac via USB. Next run the `rvictl` command in Terminal.

```
```

In this example:

- `rvictl` is the name of the command that manipulates RVIs.

- `-s` tells `rvictl` to set up a new RVI.

- `b0e8fe73db17d4993bd549418bfbdba70a4af2b1` is the UDID of the iOS device to target. This UDID is just an example; you can find your device’s UDID in the Devices and Simulators window in Xcode.

This command prints the following output.

```
```

This output includes the interface name of the newly-created RVI, `rvi0` in this example. Supply this interface name to your favorite packet trace tool to record a trace of the traffic on your iOS device. For example, use the following command to record a packet trace on `rvi0` and write it to `trace.pcap`.

```
```

If you’re having problems working with RVIs, see Troubleshooting Packet Traces for some troubleshooting tips.

### Display and Filter iOS Interface Information

An RVI represents the entire networking stack of the iOS device; you cannot target a specific interface on the device as you would on the Mac. However, information about the interface is recorded in the packet metadata. You can use your packet trace tool to display the interface for each packet and filter the trace based on that interface. For the `tcpdump` tool, use the -k option to display packet metadata and tcpdump -Q to filter on it. The `tcpdump` man page has the details; see Reading UNIX Manual Pages.

## Topics

### Working with Packet Traces

Troubleshooting Packet Traces

Take action to address packet tracing problems.

Recording a Wi-Fi Packet Trace

Record traces of Wi-Fi traffic and traffic management.

Submitting a Packet Trace to Apple

Learn the best way to record a packet trace when communicating with Apple.

## See Also

### Related Documentation

Reading UNIX Manual Pages

Use the Terminal app to read the documentation for low-level UNIX tools and APIs.

### Network Debugging

Choosing a Network Debugging Tool

Decide which tool works best for your network debugging problem.

Debugging HTTP Server-Side Errors

Understand HTTP server-side errors and how to debug them.

Debugging HTTPS Problems with CFNetwork Diagnostic Logging

Use CFNetwork diagnostic logging to investigate HTTP and HTTPS problems.

Taking Advantage of Third-Party Network Debugging Tools

Learn about the available third-party network debugging tools.

Testing and Debugging L4S in Your App

Learn how to verify your app on an L4S-capable host and network to improve your app’s responsiveness.

