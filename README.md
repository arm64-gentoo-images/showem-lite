# showem-lite
Tool to monitor the progress of a parallel **emerge**(1) in Gentoo.

## Description
**showem-lite** is a very simple utility script, which allows you to monitor the progress of a parallel **emerge**(1).

When invoked, it shows a split screen display, which updates once a second. The top part shows the tail of the current **Portage**(5) download log, and the lower part shows the tail of the most recent **Portage**(5) build log.

The download log display is cleared after 1 minute's inactivity; however, the build log is retained (even if stale) - this allows you to quickly see where a build has failed.

The path of the build log is displayed in the title bar of the window. If the window is resized, the display is adapted automatically to fit; however, a minimum size of 80 columns and 24 rows is required.

Exit **showem-lite** using Ctrl-c, when done.

## Installation

**showem-lite** is best installed (on Gentoo) via its ebuild, available as part of the **sakaki-tools-lite** [overlay](https://github.com/sakaki-/sakaki-tools-lite).

