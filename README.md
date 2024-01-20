# BombJackLevelTable

; DE38h - level meta data
;
; 64 6-byte records (ABCDEF).
;
; A = platform design number --> see 4C06h
; B = platform colour (0=yel/red, 1=green, 2=yel/red, 3=yellow, 4=blue) --> see 4E38h
; C = which tile/pal use for border -> see 5C34h
; D = bomb design number (always same as A except for levels 5, 10, ...) --> see 54EAh
; E = backdrop number (0=pyramid, 1=acropole, 2=castle, 3=city, 4=lights) --> see 4C15h
; F = music (0, 1, 2)
;
; The fact that there are only 64 entries must be why backdrops
; resync at level 65. I don't know why platform colours desync
; again at level 77, though.

    hex 00 00 02 00 00 00  ; Level 19
    hex 0B 01 00 0B 01 01
    hex 08 02 03 08 02 02
    hex 07 03 04 07 03 00
    hex 04 04 01 04 04 01
    hex 02 00 02 02 00 02
    hex 06 01 00 06 01 00
    hex 03 02 03 03 02 01
    hex 0A 03 04 0A 03 02
    hex 04 04 01 00 04 00
    hex 0C 00 02 0C 00 01
    hex 0E 01 00 0E 01 02
    hex 09 02 03 09 02 00    
    hex 0F 03 04 0F 03 01
    hex 04 04 01 04 04 02
    hex 0D 00 02 0D 00 00
    hex 01 01 00 01 01 01
    hex 05 02 03 05 02 02  ; Level 18
    hex 0B 03 04 0B 03 00  ; Level 19
    hex 04 04 01 0D 04 01  ; Level 20
    hex 0E 00 02 0E 00 02
    hex 06 01 00 06 01 00
    hex 07 02 03 07 02 01
    hex 09 03 04 09 03 02
    hex 04 04 01 0F 04 00  ; Level 25
    hex 05 00 02 05 00 01
    hex 03 01 00 03 01 02
    hex 01 02 03 01 02 00
    hex 0C 03 04 0C 03 01
    hex 04 04 01 00 04 02
    hex 02 00 02 02 00 00
    hex 08 01 00 08 01 01
    hex 0F 02 03 0F 02 02
    hex 0D 03 04 0D 03 00
    hex 04 04 01 06 04 01
    hex 0A 00 02 0A 00 02
    hex 09 01 00 09 01 00
    hex 01 02 03 01 02 01
    hex 02 03 04 02 03 02
    hex 04 04 01 02 04 00
    hex 03 00 02 03 00 01
    hex 05 01 00 05 01 02 
    hex 06 02 03 06 02 00
    hex 07 00 04 07 03 01  ; Level 44 - B returns to 0
    hex 04 01 01 0E 04 02
    hex 08 02 02 08 00 00
    hex 09 03 00 09 01 01
    hex 0A 04 03 0A 02 02
    hex 0B 00 04 0B 03 00
    hex 04 01 01 0A 04 01
    hex 0C 02 02 0C 00 02
    hex 0D 03 00 0D 01 00
    hex 0E 04 03 0E 02 01
    hex 0F 00 04 0F 03 02
    hex 04 01 01 06 04 00
    hex 00 02 02 00 00 01 ; level 56
    hex 01 03 00 01 01 02
    hex 02 04 03 02 02 00
    hex 03 00 04 03 03 01
    hex 04 01 01 08 04 02
    hex 05 02 02 05 00 00
    hex 06 03 00 06 01 01
    hex 07 04 03 07 02 02


Pattern lookup table

00	A
0B	B
08	C
07	D
04	E
02	F
06	G
03	H
0A	I
0C	J
0E	K
09	L
0F	M
0D	N
01	O
05	P

