# WpfContextMenuBug
Minimal reproduction of what seems to be a XAML compiler bug

This project contains the minimal setup to reproduce the XAML ContextMenu click handler bug.

TL;DR: When you add a ContextMenu to ListBoxItems via ItemContainerStyle, the generated items do not receive their Click event handlers properly. 

The compiler chooses the target for the event handler wrongly, as illustrated by this demo.

Compile, run and right-click any ListBox item, and see what happens...

Next, replace the atrocity that is a MenuItem placed directly in a Grid,
with any sane control (one already lies there, commented), compile and run... or at least, try to...
