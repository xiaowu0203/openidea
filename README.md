# Evidence for OpenIDEA #3713

Source branch: fix/3713-rectangular-mouse-selection
Source commit: a671b122705ac9c5f6e22e1477236318446a28a0

before-middle.png was captured from the unmodified baseline. after-middle.png was
captured from the fix before the upstream sync; both use SelectionDemo.java, at
different window widths. Browser recordings were captured after merging upstream main.
The merged Windows desktop build is blocked by upstream E0432 in clipboard.rs
(unresolved crate::commands::doc::blocking); that file is unchanged by this fix.

The recordings exercise rectangular selection/editing and mouse shortcut recording,
saving and reopening. Native desktop smoke tests use the application's MCP bridge;
Windows physical mouse/keyboard checks were separately confirmed by the contributor.
Linux and macOS native applications were not tested.

This branch contains review evidence only. It is not part of the repair branch or PR diff.