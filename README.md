# WpfContextMenuBug
Minimal reproduction of what seems to be a XAML compiler bug

This project contains the minimal setup to reproduce the XAML ContextMenu click handler bug.

TL;DR: When you add a ContextMenu to ListBoxItems via ItemContainerStyle, the generated items do not receive their Click event handlers properly. 

Compile, run, right-click any ListBoxItem and make a wild guess as to why you don't see the MessageBox...
