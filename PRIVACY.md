# VRC (Video Recording Control) - Telemetry & Privacy Policy

VRC is a free, passion-driven project built for the broadcast community. To understand if this tool is actually useful and whether I should continue investing my personal time into developing new features, VRC includes a basic, anonymous telemetry system. 

This system is **enabled by default**, but you can completely disable it at any time in the App Settings.

## What data is collected?
We only collect non-identifiable usage metrics to understand the scale of VRC deployments. When you use VRC, the app sends a simple "heartbeat" containing:
* **App Version:** (e.g., 1.0.74-beta) to see if users are updating.
* **Session Duration:** How long the app was running.
* **Device Counts:** The maximum number of devices connected during the session (e.g., 2 vMix instances, 4 HyperDecks).
* **Anonymous ID:** A randomly generated GUID created upon installation. This cannot be traced back to you or your machine.

## What is strictly NOT collected?
We respect your production environment. VRC does **NOT** collect:
* IP Addresses or MAC Addresses.
* Computer names or Usernames.
* Content of your streams, recording file names, or input names.
* Network configurations.

## How to Opt-Out
If you are working in a strictly air-gapped environment or simply prefer not to send any data, you can disable telemetry immediately:
1. Open VRC.
2. Go to **Settings** (Gear icon).
3. Toggle off **"Anonymous usage statistics"**.
No data will be sent from that point forward.

Thank you for using VRC and supporting the project!
