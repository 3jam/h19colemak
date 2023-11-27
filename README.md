Colemak on the Heathkit H19A
============================
Here is a small patch to the keymap ROM of the Heathkit H19A to switch it to
Colemak. I used a 28C16 EEPROM which is a drop in replacement for the 8316 ROM
located at U445.

The bsdiff patch can be applied by running:
```
bspatch <original rom> <new rom> colemak.bsdiff
```

The IPS patch can by applied using any number of IPS patch tools.
ROMhacking.net has a good online tool [here](https://www.romhacking.net/patch/).

The MD5 checksum for the original ROM is: `9e5288035a27f8b539e47a4dde2771e7`  
The MD5 checksum for a successfully patched patched ROM is: `37534bd8bc618021a346de6ecdae6190`

Compatibility with similar machines
-----------------------------------

I'm fairly confident that this patch will also work with the Heathkit H19 and
Zenith Z19, though I do not have access to those terminals to check their ROMs.
If you use this patch on any of those systems, please let me know. Note that
the schematics and PCBs for those machines may be numbered differently. Check
your ROM against the checksum before attempting to swap in a replacement.
