ExpireClipboard is a small security utility to expire the system Clipboard contents after a configurable timeout.

The goal is to automatically remove the potentially sensitive information from the Clipboard, where it is often left forgotten due to invisibility.

The utility stays in memory and periodically (once every minute) checks if the Clipboard contents have been changed. If the contents remain static for some configurable length of time (one hour by default) it gets emptied. This means that it would not interrupt the normal use, but if you leave your computer on after working with some sensitive data, the Clipboard will eventually be cleared without user interaction.

The utility does not keep a copy of the Clipboard contents for comparison, but instead holds a SHA-256 hash. This is to both avoid unneessary duplication of the potentially sensitive information, and to minimize the memory footprint of the utility.

Copyright (c) Alexander Ilin, 2014.
