# M472A Stereo Equalizer Module · Filters

Ward-Beck Systems M472A, 1986|19. Wiki page: [M472A on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M472A.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 32 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 7 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 5 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 19 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 8 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 28 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

**On the WBSps forum (2006|39 - 2014|47):** [1 topic](FORUM.md): what owners and technicians said about it.

## Specifications

From the technical data sheet: [1986 - M472A - P002 - 1-1.jpg](MANUALS/1986%20-%20M472A%20-%20P002%20-%201-1.jpg) page 1 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Gain** | Unity +/-0.25 dB |
| **Frequency response** | +/-0.5 dB from 20 Hz to 20 kHz with the equalizer inserted and cut/boost controls in the detent pos ton |
| **Noise** | -90 dBm absolute (20 Hz to 20 kHz) equalizer cut/boost controls in the detent position |
| **Harmonic distortion** | Less than 0.1% from 20 Hz to 20 kHz at +20 dBm output Level or Less Less than 0.01% at kHz at +20 dBm output Level. |
| **Source impedance** | Less than 10 ohms unbalanced |
| **Input impedance** | Greater than 4k ohms unbalanced |
| **Input level** | ~6dBm nominal +20 dBm maximum. |
| **Output impedance** | Less than 50 ohms unbalanced |
| **Load impedance** | Sk ohms or greater |
| **Output level** | -6 dBm nominal +22 dBm maximum. |
| **Channel separation** | Greater than 60 dB |
| **Phasing** | Input and output are in phase with the equalizing controls in the 0 detent position. |
| **Equalization tracking** | Within 0.5 dB |
| **Power requirements** | +/-25 volts dc 65 mA. |
| **Ambient temperature** | Dimensions to 60 degrees Celsius. 1.60&quot; wide 7.00&quot; high 6.50&quot; deep (41 Mm 178 Mm 165 mm). |
| **Weight** | M472A oz (0,565 kg) net. |

## Circuit description

From [1986 - M472A - P006 - 4-1.jpg](MANUALS/1986%20-%20M472A%20-%20P006%20-%204-1.jpg) page 1 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

The left channel of the M472A Stereo Equalizer wili be described. Input The unbalanced audio input appears at pin of the module connector It is routed directly to the normally closed contact of Equalizer Insert switch SWZA and to buffer amplifier U1B. Mid-Frequensy Equalizer The output from the input buffer amplifier 418 feeds summing amplifier UIA and the Mid-Frequency cut/boost control R4: R4 bridges between the input and output of summing amplifier UIA. The arm of Rb connects the signal to the state variable filter U3A, U3B, and U4A. C6 through C9 along with R15 and R18 determine the resonant frequency of the filter_ R8 adjusts the overall filter gain and therefore its 0 High 0 is nominally four and Low is nominally two. The filter output is fed back into summing amplifier UIA via C5_ This feedback signa/ adds or subtracts from the main signal in proportion to its magnitude and Phase relationship. Lew_Frequency Equalizer The output from UIA feeds the audio signal to the low frequency summing amplifier U2B, Low Frequency cutlboost control R23 bridges across 42B, with the arm of this control coupling the audio signal through C11 to Low-pass filter u4B. The frequency determining components of this filter are the LF shelf control Rz7, Rz9, C12 and C13. The filter output is fed back to summing amplifier 028 through R30. Dependent upon the setting of cut/boost control R23 the signal, is added or subtracted from the main signa/ path thus affecting the frequency response characteristics of the Low Frequency portion of the audio spectrum.

</details>

<!-- /module data -->

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYUdlN2s1THAxckU/view?resourcekey=0-WsMRo9jMwQiuQjjYXduCvg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYUdlN2s1THAxckU&resourcekey=0-WsMRo9jMwQiuQjjYXduCvg" width="240" alt="19xx - M472A - DOC - STEREO L SERIES - P009 - B77012-04-011 L.jpg"></a><br><sub>19xx - M472A - DOC - STEREO L SERIES - P009 - B77012-04-011 L · <a href="MECHANICAL/19xx%20-%20M472A%20-%20DOC%20-%20STEREO%20L%20SERIES%20-%20P009%20-%20B77012-04-011%20L%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## 3-D model

[`MECHANICAL/M472A.stl`](MECHANICAL/M472A.stl) (GitHub turns it in 3-D) · [view, change and generate it on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/2026/stl.html?m=M472A)

- **Size:** 41 × 178 mm panel, 165 mm deep, 3.2 mm plate (assumed: 1.6" x 7" x 6.5", the common module)
- **From the drawing:** 0 holes and cut-outs, 0 knobs (front panel: `MECHANICAL/M472A - front panel.svg`)
- no drawing of the front panel: the panel is blank
- Made by `tools/module_models.py` (→ `MECHANICAL/M472A.model.json`) and `tools/stl/make_stl.mjs` in [WBSps.ca](https://github.com/WardBeckSystems/WBSps.ca); the site makes the same STL from the same JSON.

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUkwzeWJRdkRqb28/view?resourcekey=0-uDRBodxCJz2NCtTh8_jjtg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUkwzeWJRdkRqb28&resourcekey=0-uDRBodxCJz2NCtTh8_jjtg" width="240" alt="1986 - M472A - 472-01-002 - EQUALIZER MODULE FUNCTIONAL.jpg"></a><br><sub>1986|19 · 472-01-002 - EQUALIZER MODULE FUNCTIONAL · <a href="SCHEMATICS/1986%20-%20M472A%20-%20472-01-002%20-%20EQUALIZER%20MODULE%20FUNCTIONAL%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWUdfb1Z4b2dLQk0/view?resourcekey=0-LkDgaH-IZP73hpsTPAeCTw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWUdfb1Z4b2dLQk0&resourcekey=0-LkDgaH-IZP73hpsTPAeCTw" width="240" alt="1986 - M472A - 472-01-002.jpg"></a><br><sub>1986|19 · 472-01-002 · <a href="SCHEMATICS/1986%20-%20M472A%20-%20472-01-002%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWERWZXM2RDhsTXc/view?resourcekey=0--zwtr2wF9XJbpQyBKJuhGw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWERWZXM2RDhsTXc&resourcekey=0--zwtr2wF9XJbpQyBKJuhGw" width="240" alt="1986 - M472A - 472-02-002 - CHASS VIOO AZO.jpg"></a><br><sub>1986|19 · 472-02-002 - CHASS VIOO AZO · <a href="SCHEMATICS/1986%20-%20M472A%20-%20472-02-002%20-%20CHASS%20VIOO%20AZO%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUUxwZzJ2U0I4b3M/view?resourcekey=0-qP6G4AdqQ9ceZSLAf8MZDA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUUxwZzJ2U0I4b3M&resourcekey=0-qP6G4AdqQ9ceZSLAf8MZDA" width="240" alt="1986 - M472A - 472-02-002 - ICD DIT COWPORRNT DRSICAATIONP COLGAT.jpg"></a><br><sub>1986|19 · 472-02-002 - ICD DIT COWPORRNT DRSICAATIONP COLGAT · <a href="SCHEMATICS/1986%20-%20M472A%20-%20472-02-002%20-%20ICD%20DIT%20COWPORRNT%20DRSICAATIONP%20COLGAT%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNS0xRXdYd09VMGM/view?resourcekey=0-F9nU5d403yHspSyWOthnCg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNS0xRXdYd09VMGM&resourcekey=0-F9nU5d403yHspSyWOthnCg" width="240" alt="1986 - M472A - 472-02-002 - UZA AJR- RJO LMUM.jpg"></a><br><sub>1986|19 · 472-02-002 - UZA AJR- RJO LMUM · <a href="SCHEMATICS/1986%20-%20M472A%20-%20472-02-002%20-%20UZA%20AJR-%20RJO%20LMUM%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWWo1YTdWUEtMRHc/view?resourcekey=0-gGUHBQIaVkjLrawFR82iEw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWWo1YTdWUEtMRHc&resourcekey=0-gGUHBQIaVkjLrawFR82iEw" width="240" alt="1986 - M472A - 472-06-002 - EQUALIZER MODULE COMPONENT LAYOUT.jpg"></a><br><sub>1986|19 · 472-06-002 - EQUALIZER MODULE COMPONENT LAYOUT · <a href="SCHEMATICS/1986%20-%20M472A%20-%20472-06-002%20-%20EQUALIZER%20MODULE%20COMPONENT%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYXhFNGtlRnVkYjQ/view?resourcekey=0-mx_JrQji49hFib1D15qdLA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYXhFNGtlRnVkYjQ&resourcekey=0-mx_JrQji49hFib1D15qdLA" width="240" alt="1986 - M472A - P018 - B 472-047-004 L.jpg"></a><br><sub>1986|19 · P018 - B 472-047-004 L · <a href="SCHEMATICS/1986%20-%20M472A%20-%20P018%20-%20B%20472-047-004%20L%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKS1VibTdJU0U1cXc/view?resourcekey=0-tx2RaDZoqVCupXtzGl7Kag" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKS1VibTdJU0U1cXc&resourcekey=0-tx2RaDZoqVCupXtzGl7Kag" width="240" alt="1986 - M472A - P019 - B 472-047-004 R.jpg"></a><br><sub>1986|19 · P019 - B 472-047-004 R · <a href="SCHEMATICS/1986%20-%20M472A%20-%20P019%20-%20B%20472-047-004%20R%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

## RTO-144 pinout

11 contacts. Every contact, with where it was read: [`RTO.json`](RTO.json).

| Pin | Signal | Kind | Pair | Confidence |
|---|---|---|---|---|
| 4 | EQ(UNBALANCED) IN LEFT | in | A1 + | high |
| 6 | EQ(UNBALANCED) OUT LEFT | out | A2 + | high |
| 9 | EQ(UNBALANCED) IN RIGHT | in | A3 + | high |
| 11 | EQ(UNBALANCED) OUT RIGHT | out | A4 + | high |

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYUVqcUh3aWM5d0E/view?resourcekey=0-ZU9S_Xs1lQGNnndbT9oMow" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYUVqcUh3aWM5d0E&resourcekey=0-ZU9S_Xs1lQGNnndbT9oMow" width="240" alt="1986 - M472A - P001 - Title Page.jpg"></a><br><sub>1986|19 · P001 - Title Page</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYndDZXNUWGwzYzA/view?resourcekey=0-OUoeSa3bqg9-JpPAbWBN9A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYndDZXNUWGwzYzA&resourcekey=0-OUoeSa3bqg9-JpPAbWBN9A" width="240" alt="1986 - M472A - P002 - 1-1.jpg"></a><br><sub>1986|19 · P002 - 1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKX3NmNC1yVEkxZm8/view?resourcekey=0-vruY4dsEYHeVVSdRgdJ6Zw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKX3NmNC1yVEkxZm8&resourcekey=0-vruY4dsEYHeVVSdRgdJ6Zw" width="240" alt="1986 - M472A - P003 - 2-1.jpg"></a><br><sub>1986|19 · P003 - 2-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdC1wcTcwQms3dHc/view?resourcekey=0-FaiYci1Aa70u-xL1pSLiqA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdC1wcTcwQms3dHc&resourcekey=0-FaiYci1Aa70u-xL1pSLiqA" width="240" alt="1986 - M472A - P004 - 3-1.jpg"></a><br><sub>1986|19 · P004 - 3-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZUN1TWVxRHY1a3M/view?resourcekey=0-QYTKH97XC4wDHtmI9u1Bfg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZUN1TWVxRHY1a3M&resourcekey=0-QYTKH97XC4wDHtmI9u1Bfg" width="240" alt="1986 - M472A - P005 - 3-2.jpg"></a><br><sub>1986|19 · P005 - 3-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSTZwbWFnVlhxdVU/view?resourcekey=0-sndemJRKDVM5hLnS7NQ6xg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSTZwbWFnVlhxdVU&resourcekey=0-sndemJRKDVM5hLnS7NQ6xg" width="240" alt="1986 - M472A - P006 - 4-1.jpg"></a><br><sub>1986|19 · P006 - 4-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWnY0NWJaNzdpVTA/view?resourcekey=0-lMinlLK71mhtZCABjV6iXw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWnY0NWJaNzdpVTA&resourcekey=0-lMinlLK71mhtZCABjV6iXw" width="240" alt="1986 - M472A - P007 - 4-2.jpg"></a><br><sub>1986|19 · P007 - 4-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWlJIeE9Pc1duOGc/view?resourcekey=0-XpwjHFDKIuaScPHYLMpDJQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWlJIeE9Pc1duOGc&resourcekey=0-XpwjHFDKIuaScPHYLMpDJQ" width="240" alt="1986 - M472A - P008 - 5-1.jpg"></a><br><sub>1986|19 · P008 - 5-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKck1rVnNxSjN2VkU/view?resourcekey=0-2rUxuw8NDyyZM27NQSIMeQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKck1rVnNxSjN2VkU&resourcekey=0-2rUxuw8NDyyZM27NQSIMeQ" width="240" alt="1986 - M472A - P009 - 5-2.jpg"></a><br><sub>1986|19 · P009 - 5-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdzBFYTc5Y09zdHM/view?resourcekey=0-w35b4c1pBk20-Nqk1Buq8A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdzBFYTc5Y09zdHM&resourcekey=0-w35b4c1pBk20-Nqk1Buq8A" width="240" alt="1986 - M472A - P010 - 5-3.jpg"></a><br><sub>1986|19 · P010 - 5-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNV8xNFNCNHI2S3c/view?resourcekey=0-k0qa5Cdf-4LMUtDGTXAtGQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNV8xNFNCNHI2S3c&resourcekey=0-k0qa5Cdf-4LMUtDGTXAtGQ" width="240" alt="1986 - M472A - P011 - 6-1.jpg"></a><br><sub>1986|19 · P011 - 6-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKckw2NlFYUXMxWUE/view?resourcekey=0-WcSuzQUd8R82lJsj8_9k0Q" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKckw2NlFYUXMxWUE&resourcekey=0-WcSuzQUd8R82lJsj8_9k0Q" width="240" alt="1986 - M472A - P012 - 6-2.jpg"></a><br><sub>1986|19 · P012 - 6-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcUM2RXZmcHdGOEU/view?resourcekey=0-J6QQNB5RdTk7RSPz79a2KA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcUM2RXZmcHdGOEU&resourcekey=0-J6QQNB5RdTk7RSPz79a2KA" width="240" alt="1986 - M472A - P013 - 6-3.jpg"></a><br><sub>1986|19 · P013 - 6-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbFFFdWhTamhOVDQ/view?resourcekey=0-KIQJUkV_MQaBJ_uho1YtKA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbFFFdWhTamhOVDQ&resourcekey=0-KIQJUkV_MQaBJ_uho1YtKA" width="240" alt="1986 - M472A - P014 - 6-4.jpg"></a><br><sub>1986|19 · P014 - 6-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcDN6bF9abU1RQTg/view?resourcekey=0-hvtqqASWkHNzCHVLJKdlEw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcDN6bF9abU1RQTg&resourcekey=0-hvtqqASWkHNzCHVLJKdlEw" width="240" alt="1986 - M472A - P015 - 6-5.jpg"></a><br><sub>1986|19 · P015 - 6-5</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbmszNk9BTUNER00/view?resourcekey=0-okF1Cw2OEJV32DHdal3PGg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbmszNk9BTUNER00&resourcekey=0-okF1Cw2OEJV32DHdal3PGg" width="240" alt="1986 - M472A - P016 - 6-6.jpg"></a><br><sub>1986|19 · P016 - 6-6</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZUZQcWliZ1ZHRFk/view?resourcekey=0-2ixKRaz8IpXJP5TXXsWNpQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZUZQcWliZ1ZHRFk&resourcekey=0-2ixKRaz8IpXJP5TXXsWNpQ" width="240" alt="1986 - M472A - P017 - 7-1.jpg"></a><br><sub>1986|19 · P017 - 7-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNi1HWHBYRGJxWHM/view?resourcekey=0-d-OxVSOZAbT6PHa_f9sQjA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNi1HWHBYRGJxWHM&resourcekey=0-d-OxVSOZAbT6PHa_f9sQjA" width="240" alt="19xx - M472A - DOC - K2942S - P18 - 3-1.jpg"></a><br><sub>19xx - M472A - DOC - K2942S - P18 - 3-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQTJ6c0JaSklnaEk/view?resourcekey=0-XM7munndTr4kWzum7sbPXg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQTJ6c0JaSklnaEk&resourcekey=0-XM7munndTr4kWzum7sbPXg" width="240" alt="19xx - M472A - DOC - STEREO L SERIES - P007.jpg"></a><br><sub>19xx - M472A - DOC - STEREO L SERIES - P007</sub></td></tr>
</table>

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [1986 - M472A - 472-01-002 - EQUALIZER MODULE FUNCTIONAL.kicad_sch](KICAD/1986%20-%20M472A%20-%20472-01-002%20-%20EQUALIZER%20MODULE%20FUNCTIONAL.kicad_sch)
- [1986 - M472A - 472-01-002.kicad_sch](KICAD/1986%20-%20M472A%20-%20472-01-002.kicad_sch)
- [1986 - M472A - 472-02-002 - CHASS VIOO AZO.kicad_sch](KICAD/1986%20-%20M472A%20-%20472-02-002%20-%20CHASS%20VIOO%20AZO.kicad_sch)
- [1986 - M472A - 472-02-002 - ICD DIT COWPORRNT DRSICAATIONP COLGAT.kicad_sch](KICAD/1986%20-%20M472A%20-%20472-02-002%20-%20ICD%20DIT%20COWPORRNT%20DRSICAATIONP%20COLGAT.kicad_sch)
- [1986 - M472A - 472-02-002 - UZA AJR- RJO LMUM.kicad_sch](KICAD/1986%20-%20M472A%20-%20472-02-002%20-%20UZA%20AJR-%20RJO%20LMUM.kicad_sch)
- [1986 - M472A - P018 - B 472-047-004 L.kicad_sch](KICAD/1986%20-%20M472A%20-%20P018%20-%20B%20472-047-004%20L.kicad_sch)
- [1986 - M472A - P019 - B 472-047-004 R.kicad_sch](KICAD/1986%20-%20M472A%20-%20P019%20-%20B%20472-047-004%20R.kicad_sch)
- [M472A.kicad_sym](KICAD/M472A.kicad_sym)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
