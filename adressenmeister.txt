10 REM * A D R E S S E N M E I S T E R * 
20 REM * ( C ) BY MICHAEL CLEMENS  '92 * 
100 PRINT"{clr}" 
101 PRINT "{down}{down}{down}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{red}A{purple}D{yellow}R{cyan}E{green}S{lblue}S{orange}E{brown}N-" 
102 PRINT"{down}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{lgreen}M{lblue}E{brown}I{grey3}S{grey2}T{lblue}E{lred}R" 
103 PRINT"{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{yellow}( C ) B Y   M I C H A E L  C L E M E N S{white}" 
110 POKE53280,0:POKE53281,0 
120 V=53248 
130 POKEV+21,4 
140 POKE2042,13 
150 FORN=0TO62:READQ:POKE832+N,Q:NEXT 
160 POKE V+23,4:POKE V+29,4 
165 FOR MICHI=1 TO 2 
170 FORX=0TO250 
180 POKEV+4,X 
190 POKEV+5,X 
192 FOR T=1 TO 15:NEXT 
194 NEXTX 
195 NEXT MICHI 
196 GOTO10100 
200 DATA35,59,48,82,170,64,138,179,54,251,170,16 
210 DATA139,43,96,0,0,0,109,40,180,137,173,164 
220 DATA109,106,181,41,40,164,205,40,180,0,0,0 
230 DATA110,220,0,132,148,0,100,216,0,36,148,0,196,212,0 
240 DATA0,0,0,68,65,128,134,194,0,69,81,160 
900 GOTO 5000 
1000 PRINT"{clr}" 
1010 POKE53280,14:POKE53281,6 
1100 PRINT"{right}{right}{right}{right}**** COMMODORE 64 BASIC V2 ****" 
1200 PRINT"{down}{right}NOTIZBLOCK V1.2 BY MICHAEL CLEMENS '92" 
1300 PRINT"{down}READY." 
1400 POKE 19,1 
1500 OPEN 4,4 
1600 INPUT A$ 
1700 PRINT 
1900 IF A$="@M"THEN CLOSE 4:POKE19,0:GOTO 5000 
2000 PRINT#4,A$ 
2100 CLOSE 4 
2200 GOTO 1400 
2300 CLOSE 4 
2400 PRINT"{clr}" 
2450 INPUT"{rvson}{right}{right}{right}{right}{right}{right}{right}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}SIND SIE SICH SICHER{rvsoff}";A$ 
2451 IF A$="J"THEN 2500 
2452 IF A$<>"J"THEN 5000 
2500 PRINT"{clr}{rvson}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}AUF WIEDERSEHEN!{rvsoff}" 
2700 WAIT 198,1 
2800 SYS 64738 
2900 PRINT"{clr}" 
3000 PRINT"    **** COMMODORE 64 BASIC V2 ****" 
3100 PRINT"{down} ADRESSENDRUCKER BY MICHAEL CLEMENS '92" 
3300 OPEN 4,4 
3400 INPUT"{down}{down}{down}{down}{down}{down}{right}{right}{right}N A M E :";A$:IF A$="@M"THENGOTO5000 
3600 INPUT"{down}{right}{right}{right}S T R A S S E :";B$:IF B$="@M" THEN GOTO5000 
3800 INPUT"{down}{right}{right}{right}P L Z / O R T :";C$:IF C$="@M" THEN GOTO5000 
3900 INPUT"{down}{right}{right}{right}T E L.:";D$:IF D$="@M" THEN GOTO 5000 
3945 PRINT#4,A$:PRINT#4,B$:PRINT#4,C$:PRINT#4,D$ 
3950 CLOSE4 
4000 INPUT"{down}{down}{right}{right}NOCH EINE ADRESSE (J/N)";A$ 
4100 IF A$="J"THEN GOTO 2900 
4200 IF A$<>"J"THEN GOTO 5000 
5000 CLOSE 4:PRINT"{clr}":POKEV+21,0:POKE53281,6:POKE53280,14 
5100 PRINT"    **** COMMODORE 64 BASIC V2 ****" 
5200 PRINT"{down} ** M E N U E ** BY MICHAEL CLEMENS '92" 
5300 PRINT"{down}{down}{down}{down}{right}-P R O G R A M M" 
5400 PRINT"{down}{right}{right}{rvson}A{rvsoff}DRESSENDRUCKER" 
5500 PRINT"{down}{right}{right}{rvson}N{rvsoff}OTIZBLOCK" 
5600 PRINT"{down}{down}{down}{right}-S O N S T I G E S" 
5700 PRINT"{down}{right}{right}{rvson}E{rvsoff}RSTE HILFE" 
5850 PRINT"{down}{right}{right}{rvson}R{rvsoff}AUS HIER" 
5900 PRINT"{up}{up}{up}{up}{up}{up}{up}{up}{up}{up}{up}{up}{up}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}-D R U C K E R" 
6000 PRINT"{down}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{rvson}B{rvsoff}REITDRUCK" 
6100 PRINT"{down}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{rvson}K{rvsoff}URSIVDRUCK" 
6200 PRINT"{down}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{rvson}U{rvsoff}NTERSTREICHUNG"
6300 PRINT"{down}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{rvson}S{rvsoff}CHATTENDRUCK" 
6350 PRINT"{down}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{rvson}F{rvsoff}ETTDRUCK" 
6360 PRINT"{down}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{right}{rvson}NLQ{rvsoff}-DRUCK" 
6400 INPUT"{down}{down}{down}{right}{right}{right}{right}{right}WAS MOECHTEN SIE";M$ 
6500 IF M$="E"THEN GOTO 26000 
6700 IF M$="A"THEN GOTO 2900 
6800 IF M$="N"THEN GOTO 1000 
6900 IF M$="B" THEN GOTO 26990 
7000 IF M$="K" THEN GOTO 27100 
7100 IF M$="U" THEN GOTO 27200 
7200 IF M$="S" THEN GOTO 27300 
7201 IF M$="R" THEN GOTO 2400 
7202 IF M$="NLQ" THEN GOTO 30000 
10100 POKE53280,0:POKE53281,0 
10200 V=53248 
10300 POKEV+21,4 
10400 POKE2042,13 
10500 FORN=0TO62:READQ:POKE832+N,Q:NEXT 
10600 POKE V+23,4:POKE V+29,4 
10700 FOR MICHI=1 TO 2 
10800 FORX=0TO250 
10900 POKEV+4,255 
11000 POKEV+5,X 
11100 FOR T=1 TO 15:NEXT 
11200 NEXTX 
11300 NEXT MICHI 
11350 GOTO 12000 
11400 DATA,,,,,,,,,1,255,,2,170,128,4,,64,8,,32,8,198,32,8,214,32,8,16 
11500 DATA 32 ,10,16,160,9,1,32,8,130,32,4,124,64,2,,128,1,131,,,68,,,68,0,0,0 
11600 DATA0,0,0,0,0,0,0 
12000 POKE53280,0:POKE53281,0 
12100 V=53248 
12200 POKEV+21,4 
12300 POKE2042,13 
12400 FORN=0TO62:READQ:POKE832+N,Q:NEXT 
12500 POKE V+23,4:POKE V+29,4 
12600 FOR MICHI=1 TO 1 
12700 FORX=0TO250 
12800 POKEV+4,X 
12900 POKEV+5,150 
13000 FOR T=1 TO 15:NEXT 
13100 NEXTX 
13200 NEXT MICHI 
13250 POKEV+21,0 
13300 GOTO5000 
13400 DATA35,59,48,82,170,64,138,179,54,251,170,16 
13500 DATA139,43,96,0,0,0,109,40,180,137,173,164 
13600 DATA109,106,181,41,40,164,205,40,180,0,0,0 
13700 DATA110,220,0,132,148,0,100,216,0,36,148,0,196,212,0 
13800 DATA0,0,0,68,65,128,134,194,0,69,81,160 
13900 GOTO 5000 
26000 PRINT"{clr}" 
26010 PRINT"    **** COMMODORE 64 BASIC V2 ****" 
26020 PRINT"{down} ERSTE-HILFE V.1 BY MICHAEL CLEMENS '92" 
26030 PRINT"{down}{down}{down}{down}{down}{right}{right}{right}WAS IST LOS?" 
26040 PRINT"{down}{right}{right}{right}{rvson}D{rvsoff}RUCKT DER DRUCKER NICHT ODER " 
26045 INPUT"{right}{right}{right}{rvson}B{rvsoff}LEIBEN DIE NADELN HAENGEN";A$ 
26050 IF A$="D"THEN GOTO 26070 
26060 IF A$="B"THEN GOTO 26150 
26070 OPEN4,4 
26080 PRINT#4,CHR$(7) 
26090 CLOSE4 
26100 INPUT"{down}{right}{right}{right}HOEREN SIE DEN PIEPSER (J/N)";A$ 
26110 IF A$="J"THEN GOTO 26115 
26111 IF A$="N" THEN GOTO 26135 
26115 PRINT"{down}{right}{right}{right}DANN MUESSTE EIGENTLICH ALLES" 
26120 PRINT"{right}{right}{right}FUNKTIONIEREN":WAIT 198,1:GOTO 5000 
26135 PRINT"{down}{right}{right}{right}VIELLEICHT LIEGT ES AN DER" 
26140 PRINT"{right}{right}{right}DRUCKERADRESSE (MOMENTAN NR.4)":WAIT 198,1:GOTO 5000 
26150 PRINT"{down}{right}{right}{right}VIELLEICHT IST DER DRUCKKOPF " 
26160 PRINT"{right}{right}{right}ZU NAH AM PAPIER":WAIT 198,1:GOTO 5000 
26990 PRINT"{clr}":INPUT"{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{right}{right}{right}{right}{right}{rvson}E{rvsoff}IN- ODER {rvson}A{rvsoff}US- SCHALTEN";F$ 
26991 IF F$="E" THEN GOTO 27000 
26992 IF F$<>"E" THEN GOTO 27030 
27000 OPEN4,4 
27010 PRINT#4,CHR$(14) 
27020 CLOSE 4 
27025 GOTO 5000 
27030 OPEN4,4 
27040 PRINT#4,CHR$(15) 
27050 CLOSE 4 
27060 GOTO5000 
27100 PRINT"{clr}":INPUT"{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{right}{right}{right}{right}{right}{rvson}E{rvsoff}IN- ODER {rvson}A{rvsoff}US- SCHALTEN";F$ 
27105 PRINT"{down}{down}{right}{right}{rvson}ACHTUNG: NLQ WIRD MIT EINGESCHALTET":WAIT 198,1 
27110 IF F$="E" THEN GOTO 27141 
27120 IF F$<>"E" THEN GOTO 27160 
27130 IF B$="N"THEN PRINT"{down}{right}{right}{right}VIELLEICHT STIMMT DIE DRUCKERADRESSE" 
27140 PRINT"{right}{right}{right}NICHT":WAIT 198,1:GOTO 5000 
27141 OPEN4,4 
27142 PRINT#4, CHR$(27);CHR$(120);CHR$(49) 
27143 CLOSE4 
27144 OPEN4,4 
27145 PRINT#4, CHR$(27);CHR$(52) 
27150 CLOSE 4 
27155 GOTO 5000 
27160 OPEN4,4 
27165 PRINT#4,CHR$(27);CHR$(53) 
27166 CLOSE4 
27167 OPEN4,4 
27169 PRINT#4, CHR$(27);CHR$(120);CHR$(48) 
27170 CLOSE 4 
27175 GOTO5000 
27200 PRINT"{clr}":INPUT"{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{right}{right}{right}{right}{right}{rvson}E{rvsoff}IN- ODER {rvson}A{rvsoff}US- SCHALTEN";F$ 
27210 IF F$="E" THEN GOTO 27230 
27220 IF F$<>"E" THEN GOTO 27260 
27230 OPEN4,4 
27240 PRINT#4,CHR$(27);CHR$(45);CHR$(49) 
27250 CLOSE 4 
27255 GOTO 5000 
27257 PRINT#4, CHR$(27);CHR$(120);CHR$(49) 
27260 OPEN4,4 
27265 PRINT#4,CHR$(27);CHR$(45);CHR$(48) 
27270 CLOSE 4 
27275 GOTO5000 
27300 PRINT"{clr}":INPUT"{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{right}{right}{right}{right}{right}{rvson}E{rvsoff}IN- ODER {rvson}A{rvsoff}US- SCHALTEN";F$ 
27310 IF F$="E" THEN GOTO 27330 
27320 IF F$<>"E" THEN GOTO 27360 
27330 OPEN4,4 
27340 PRINT#4,CHR$(27);CHR$(69) 
27350 CLOSE 4 
27355 GOTO 5000 
27360 OPEN4,4 
27365 PRINT#4,CHR$(27);CHR$(69) 
27370 CLOSE 4 
27375 GOTO5000 
30000 PRINT"{clr}":INPUT"{down}{down}{down}{down}{down}{down}{down}{down}{down}{down}{right}{right}{right}{right}{right}{rvson}E{rvsoff}IN- ODER {rvson}A{rvsoff}US- SCHALTEN";F$ 
30001 IF F$="E" THEN GOTO 30003 
30002 IF F$<>"E" THEN GOTO 30008 
30003 OPEN4,4 
30004 PRINT#4,CHR$(27);CHR$(120);CHR$(49) 
30005 CLOSE 4 
30006 GOTO 5000 
30008 OPEN4,4 
30009 PRINT#4,CHR$(27);CHR$(120);CHR$(48) 
30010 CLOSE 4 
30011 GOTO5000