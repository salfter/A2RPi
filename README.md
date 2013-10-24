This is a redesign of the Apple II Pi (http://schmenk.is-a-geek.com/wordpress/?cat=10), with
the following goals:

1) Keep the design in files with an open format, editable with
   freely-available design software.
2) Replace through-hole components with surface-mount components to the
   extent that it's possible to do so.
3) Enable future improvements to the design by anybody interested in doing
   so (item 1 helps considerably with this).

Recent discussion in comp.sys.apple2
(https://groups.google.com/forum/#!topic/comp.sys.apple2/ogb335ww8-w) has
already led to one change: provision has been made to clock the 6551 with
either a crystal (and, if needed, an extra capacitor) or the GPIO4 line from
the Raspberry Pi.  Also, I had originally planned on using the WDC W65C51N
in the LQFP-32 package, but (1) the current datasheet indicates that part
might not be widely available and (2) there are some bugs in the W65C51N
that indicate it might be a better idea to use new-old-stock 6551s from
other suppliers.  That is why the 6551 is still using the old DIP-28
footprint.
