=== Windows Firewall Notifier Lite ===
Website: https://github.com/AtlasHackert/WFNLite
Current version: Alpha


=== Description ===
Windows Firewall Notifier Lite (WFN Lite) is based on Windows Firewall Notifier (WFN), which can be found at https://github.com/wokhansoft/WFN

WFN started as an "extension" to the embedded Windows firewall, and WFN Lite is a stripped-down version containing only the notification functionality.

Please read the documentation about the features and limitation of WFN Lite. Especially note that WFN Lite is **not** a firewall itself; it is only an extension of the Windows Firewall!


=== Behavior ===
This application only uses existing Windows features, enabling some of them when first launched:
- Enables the Windows embedded firewall
- Sets the firewall to block both inbound and outbound connections for which no rule exists
- Enables the default Windows firewall inbound connection notification
- Enables the Windows firewall outbound connections logging (disabled by default)
- Creates a scheduled task linked to the Windows firewall event log entries, allowing WFN Lite to be launched when needed only


=== Installation ===
WFN Lite is tested on an up-to-date Windows 10 64-bit machine with the latest .NET framework installed. It may run on older set-ups too, but this is not guaranteed.

The application can be unzipped in the folder of your choice (usually C:\Program Files\WFNLite). Run the "EnableWFNLite.cmd" program in order to set-up WFN Lite.

Uninstall: Run the "DisableWFNLite.cmd" program in WFN Lite's program folder. Afterwards, you can safely delete the WFNLite files.


=== How-to ===
WFN Lite will show a notification balloon when an application attempts an outgoing connection while not being allowed to do so. From this notification, several actions can be taken, such as:
- create a rule for the application, so that it will always be able to connect;
- always block the application (no notification will therefore be displayed afterwards);
- create a fine-tuned rule to allow or block only specific types of connection from the application.

To remove created firewall rules, a button to open the Windows Firewall configuration applet can be used.


=== Release history ===
Alpha
