#!/bin/sh

# Unload LaunchDaemons
launchctl unload /System/Library/LaunchDaemons/com.apple.gw_controld.plist
launchctl unload /System/Library/LaunchDaemons/com.apple.gw_datad.plist
launchctl unload /System/Library/LaunchDaemons/com.apple.gw_logd.plist

# Remove Keychain Items
rm /System/Library/Keychains/AppleServiceToolkit.keychain

# Remove Launch Daemons
rm /System/Library/LaunchDaemons/com.apple.gw_controld.plist
rm /System/Library/LaunchDaemons/com.apple.gw_datad.plist
rm /System/Library/LaunchDaemons/com.apple.gw_logd.plist

# Remove Preferences
rm /Library/Preferences/com.apple.gateway.plist
rm ~/Library/Preferences/com.apple.GatewayManager.plist

# Remove command line utilities
rm /usr/bin/gw_controld
rm /usr/bin/gw_datad
rm /usr/bin/gw_logd

# Remove Diagnostics Gateway & support files
rm -rf /Applications/Gateway\ Manager.app
rm -rf /private/var/adg

# Remove Netboot Sets
rm -rf /Library/NetBoot/NetBootSP0/AppleServiceToolkit.nbi
rm -rf /Library/NetBoot/NetBootSP0/AppleDiagnosticOSs
rm -rf /Library/NetBoot/NetBootSP0/AppleDiagnosticOS
rm -rf /Library/NetBoot/NetBootSP0/AST64bit.nbi
rm -rf /Library/NetBoot/NetBootSP0/ASTLegacy.nbi
rm -rf /Library/NetBoot/NetBootSP0/Diagnostics.nbi
rm -rf /Library/NetBoot/NetBootSP0/i386
rm -rf /Library/NetBoot/NetBootSP0/TAOS_*

# Remove receipts
rm /Library/Receipts/apple.com.astos*

# Remove log files
rm -rf /private/var/log/adg

exit 0