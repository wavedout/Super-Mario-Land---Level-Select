SUPER MARIO LAND - LEVEL SELECT
Version 1.0
Release date: September 21, 2026
Platform: Nintendo Game Boy

OVERVIEW
========
This small quality-of-life hack permanently enables Super Mario Land's
built-in level select from the title screen.

In the original game, level select is unlocked only after completing the
game twice: once normally and once in Expert Mode. This patch makes the
level select available immediately, with no prior completion and no save
file required.

The hack keeps the normal game difficulty. It does not force Expert Mode.

HOW TO USE
==========
At the title screen:

  A      Cycle through the 12 stages.
  START  Begin the currently selected stage.

PATCHING
========
Two patch formats are included:

  Super Mario Land - Level Select.bps
  Super Mario Land - Level Select.ips

BPS is recommended because the format validates the source ROM.
IPS is included for compatibility with older patching utilities.

Apply ONE patch to a clean, unmodified copy of:

  Super Mario Land (World)

Do not apply both patches. Do not apply the patch to Super Mario Land DX,
Rev A, or another already-modified ROM.

SOURCE ROM INFORMATION
======================
Name:    Super Mario Land (World)
Size:    65536 bytes
CRC32:   90776841
MD5:     B48161623F12F86FEC88320166A21FCE
SHA-1:   3A4DDB39B234A67FFB361EE7ABC3D23E0A8B1C89
SHA-256: 470D6C45C9BCF7F0397D00C1AE6DE727C63DD471049C8EEDBEFDC540CEEA80B4

PATCHED ROM INFORMATION
=======================
Size:    65536 bytes
CRC32:   A02CBC4E
MD5:     A480CB8CFFF19483EAA2BB1E81006879
SHA-1:   D4DD74FF565B2045DD1FF592C6ED5D191602D22C
SHA-256: 8921D584F1D5DDF3C20338D73B1133C03CD7BFD84817F6F1A47DEAAF07CE8C8B

TECHNICAL NOTES
===============
This is intentionally a minimal hack. It changes the two checks that gate
the built-in level-select state, allowing the original level-select routine
to be used immediately. The Game Boy global checksum is then corrected.

Three bytes differ from the clean ROM in total:

  ROM offset $04A9: $02 -> $00
  ROM offset $04D1: $02 -> $00
  ROM offset $014F: $6B -> $67  (global checksum)

No graphics, levels, music, physics, or normal-difficulty enemy layouts are
changed.

PATCH FILE CHECKSUMS
====================
BPS:
  Size:    38 bytes
  CRC32:   2144DF1C
  MD5:     E570BE6D84F13560E5F571C1A3D08E39
  SHA-1:   B128B703195485D0342024A8DDD395D2B4DD03B8
  SHA-256: 1A9810CDDEE4314BBAD340386FF4F00C4EF504A9DDEF5EF39EFE92DC9F3C74BF

IPS:
  Size:    26 bytes
  CRC32:   A18DABBC
  MD5:     DB37C15337F1D5673818E65D0B7522A5
  SHA-1:   AFB11B372FC0E092198596327438DFE74A1ADEDB
  SHA-256: CC533A023B5A6D167BBF805B8780295E874D09FD51205A376A25FF1894204B5A

CREDITS
=======
Hack / release: [YOUR NAME OR ROMHACKING.NET USERNAME]

Super Mario Land was developed and published by Nintendo.
This patch contains no original game ROM.

CHANGELOG
=========
v1.0 - September 21, 2026
- Initial release.
- Level select is available immediately on the title screen.
- Normal difficulty is retained.
- BPS and IPS patch formats included.
