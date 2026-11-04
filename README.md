# AquaSense Mini Build

## AI Tool Used
Claude AI was used to assist with developing the tank level dashboard using HTML, CSS, and JavaScript.

## Prompts Used

**Prompt 1:**
"Create a simple tank level dashboard using HTML, CSS, and JavaScript, displaying the current level, today's minimum, and today's maximum from the provided JSON data."

**Prompt 2:**
"Add an alert feature that checks the water level and displays a warning banner at the top of the page whenever it drops below 20%."

## Mobile App Behavior When Wi-Fi Disconnects

If the device loses Wi-Fi connection during an operation, the mobile app should detect the connection loss and display an offline warning to the user. It should not show outdated tank readings as live data. Any pending command should be handled safely. Once the Wi-Fi connection is restored, the app should reconnect to the device and fetch the latest tank status to update the dashboard.
