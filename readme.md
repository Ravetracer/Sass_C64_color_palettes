C64 color palettes for Sass/Compass
=

Since Sass supports the "map" type and recently Compass 1.0 introduces the support also, I've decided to collect all Commodore C64 color palettes I found around in emulators and on the internet.

These colors can be easily imported in your Sass .scss files like any other one:

	@import "<where-every-you-put-your-add-on-files>/c64colors"
	
Then use it in the following way like this small example:

	$pal = $c64_<palette_name>;
	
	p.white {
		color: map_get($pal, c64-white);
	}
	
	div.c64-border {
		background-color: map_get($pal, c64-light-blue);
	}
	
	div.c64-background {
		background-color: map_get($pal, c64-blue);
	}
	
> I've created the reference **$pal** so it's possible to switch to another palette without modifying **map_get()** commands

Palette names:
-
**Prefix the following names with $c64_**

* ccs64 *(taken from emulator)*
* light
* old
* old2
* pepto *(my preferred one)*
* deekay
* frodo *(taken from emulator)*
* gryf_elysium
* jpz
* moog_agony
* vice *(taken from emulator)*
* wanja
* wanja_inverse

Color names:
-
**Use them in the map_get($pal, < color-name >) function**
* c64-black
* c64-white
* c64-red
* c64-cyan
* c64-purple
* c64-green
* c64-blue
* c64-yellow
* c64-orange
* c64-brown
* c64-light-red
* c64-dark-grey
* c64-grey
* c64-light-green
* c64-light-blue
* c64-light-grey

**Have fun!**