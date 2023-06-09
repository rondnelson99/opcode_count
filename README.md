# opcode_count
Used to get statistics of which instructions your Game Boy code uses.
Instructions:
 - In Emulicious, open the Trace Logger from the debugger
 - Set Write Trace Log to File on
 - Uncheck all the boxes at the bottom, but put in `@PC` as the "Additional Expression"
 - Profile your game with the Start Tracing and Stop Tracing button
 - Run the script and pass your logged file as an output
 - Profit?

Sameple Output:
```
LD A,(HL+): 8.33% (217101 occurences)
LD L,A: 5.23% (136392 occurences)
RET: 5.11% (133225 occurences)
CALL a16: 3.27% (85258 occurences)
JR NZ,r8: 3.18% (83033 occurences)
ADD A,d8: 2.7% (70357 occurences)
PUSH HL: 2.57% (67099 occurences)
POP HL: 2.57% (67098 occurences)
LD B,A: 2.49% (64833 occurences)
ADC A,D: 2.45% (63877 occurences)
LD H,A: 2.38% (61994 occurences)
POP DE: 2.25% (58743 occurences)
LD H,(HL): 2.17% (56648 occurences)
ADD A,E: 2.07% (54087 occurences)
ADC A,d8: 2.03% (52821 occurences)
SUB L: 1.99% (51917 occurences)
JR r8: 1.97% (51290 occurences)
PUSH DE: 1.93% (50328 occurences)
PUSH BC: 1.91% (49864 occurences)
ADD HL,HL: 1.88% (49003 occurences)
LD B,H: 1.85% (48361 occurences)
LD C,L: 1.85% (48361 occurences)
LD C,A: 1.75% (45657 occurences)
LDH A,(a8): 1.75% (45525 occurences)
LD (DE),A: 1.7% (44318 occurences)
SUB C: 1.43% (37232 occurences)
LD A,(DE): 1.38% (36077 occurences)
INC DE: 1.36% (35351 occurences)
LD E,A: 1.26% (32889 occurences)
LD D,A: 1.26% (32877 occurences)
AND d8: 1.25% (32471 occurences)
DEC A: 1.18% (30734 occurences)
LDH (a8),A: 1.09% (28500 occurences)
SUB E: 1.01% (26426 occurences)
LD A,H: 0.97% (25414 occurences)
LD A,B: 0.96% (25011 occurences)
LD A,(BC): 0.82% (21393 occurences)
LD H,d8: 0.76% (19859 occurences)
DEC DE: 0.76% (19838 occurences)
AND A: 0.7% (18317 occurences)
LD (BC),A: 0.68% (17856 occurences)
JR Z,r8: 0.68% (17808 occurences)
LD (a16),A: 0.66% (17199 occurences)
LD A,d8: 0.65% (17056 occurences)
ADD HL,DE: 0.64% (16695 occurences)
PREFIX CB: 0.63% (16411 occurences)
LD (HL+),A: 0.61% (15883 occurences)
LD B,(HL): 0.6% (15581 occurences)
RRA: 0.59% (15258 occurences)
RET Z: 0.55% (14225 occurences)
INC L: 0.54% (13961 occurences)
LD A,L: 0.5% (13080 occurences)
LD A,E: 0.49% (12828 occurences)
RST 20H: 0.46% (12064 occurences)
LD HL,d16: 0.45% (11679 occurences)
POP AF: 0.45% (11605 occurences)
LD L,d8: 0.44% (11518 occurences)
PUSH AF: 0.44% (11517 occurences)
OR L: 0.36% (9504 occurences)
CP d8: 0.34% (8812 occurences)
DEC C: 0.32% (8358 occurences)
LD A,(a16): 0.32% (8227 occurences)
LD A,C: 0.28% (7420 occurences)
CP B: 0.27% (7140 occurences)
LD A,(HL): 0.27% (7095 occurences)
OR (HL): 0.27% (7063 occurences)
INC E: 0.24% (6276 occurences)
SUB B: 0.23% (6035 occurences)
LD A,(HL-): 0.2% (5298 occurences)
LD C,d8: 0.19% (5008 occurences)
LD (HL),A: 0.17% (4498 occurences)
SUB (HL): 0.17% (4484 occurences)
INC H: 0.15% (4013 occurences)
XOR A: 0.14% (3636 occurences)
JP (HL): 0.13% (3506 occurences)
JR NC,r8: 0.12% (3114 occurences)
ADD A,A: 0.1% (2732 occurences)
LD A,D: 0.1% (2637 occurences)
DEC B: 0.1% (2634 occurences)
SUB d8: 0.1% (2549 occurences)
JP a16: 0.1% (2483 occurences)
ADD A,B: 0.09% (2253 occurences)
LD (HL-),A: 0.08% (2156 occurences)
ADD A,C: 0.08% (2018 occurences)
RETI: 0.08% (2004 occurences)
INC HL: 0.07% (1880 occurences)
LD E,L: 0.07% (1859 occurences)
LD D,H: 0.07% (1859 occurences)
LD DE,d16: 0.07% (1803 occurences)
ADD A,(HL): 0.07% (1735 occurences)
RST 08H: 0.06% (1502 occurences)
POP BC: 0.06% (1502 occurences)
INC C: 0.06% (1455 occurences)
INC A: 0.04% (1104 occurences)
OR d8: 0.04% (1064 occurences)
DEC (HL): 0.04% (1027 occurences)
JR C,r8: 0.04% (1007 occurences)
DI: 0.04% (1002 occurences)
XOR B: 0.04% (1000 occurences)
CP (HL): 0.04% (1000 occurences)
HALT: 0.04% (993 occurences)
ADC A,H: 0.03% (900 occurences)
AND B: 0.03% (876 occurences)
LD (HL),d8: 0.03% (825 occurences)
JP Z,a16: 0.03% (741 occurences)
ADD HL,BC: 0.02% (645 occurences)
LD D,d8: 0.02% (607 occurences)
CPL: 0.02% (551 occurences)
LD BC,d16: 0.02% (540 occurences)
CALL NZ,a16: 0.02% (537 occurences)
CALL C,a16: 0.02% (524 occurences)
EI: 0.02% (501 occurences)
AND (HL): 0.02% (501 occurences)
JP NZ,a16: 0.02% (501 occurences)
LD (C),A: 0.02% (476 occurences)
RET NZ: 0.02% (431 occurences)
RST 28H: 0.01% (376 occurences)
ADC A,E: 0.01% (376 occurences)
LD E,C: 0.01% (252 occurences)
SCF: 0.01% (235 occurences)
ADD A,D: 0.01% (180 occurences)
LD L,E: 0.01% (153 occurences)
LD E,d8: 0.01% (144 occurences)
DEC HL: 0.01% (135 occurences)
LD B,d8: 0.01% (134 occurences)
INC (HL): 0.0% (126 occurences)
SUB H: 0.0% (120 occurences)
CP L: 0.0% (116 occurences)
CALL Z,a16: 0.0% (116 occurences)
LD C,(HL): 0.0% (116 occurences)
LD H,D: 0.0% (107 occurences)
AND E: 0.0% (88 occurences)
OR E: 0.0% (88 occurences)
OR H: 0.0% (85 occurences)
ADC A,(HL): 0.0% (64 occurences)
XOR D: 0.0% (63 occurences)
ADD A,H: 0.0% (63 occurences)
CP C: 0.0% (63 occurences)
XOR (HL): 0.0% (59 occurences)
SBC A,C: 0.0% (58 occurences)
RET C: 0.0% (41 occurences)
LD (HL),L: 0.0% (38 occurences)
LD (HL),H: 0.0% (38 occurences)
XOR d8: 0.0% (36 occurences)
ADD A,L: 0.0% (36 occurences)
AND C: 0.0% (33 occurences)
DEC E: 0.0% (27 occurences)
RLCA: 0.0% (23 occurences)
SBC A,A: 0.0% (23 occurences)
CP E: 0.0% (23 occurences)
OR B: 0.0% (18 occurences)
LD A,(C): 0.0% (18 occurences)
LD L,(HL): 0.0% (18 occurences)
ADC A,B: 0.0% (9 occurences)
CALL NC,a16: 0.0% (9 occurences)
LD (HL),E: 0.0% (9 occurences)
XOR H: 0.0% (4 occurences)
Total number of lines in the file: 2607424```
