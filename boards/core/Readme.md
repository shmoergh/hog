## Core board

Circuit for all core modules of HOG:

- 2x VCO
- 2x Waveshapers
- VCA
- ADSR
- 2x LFO
- Sub source
- Noise source
- Output

### Versions

**Experimental** — Some parts of the circuit contains multiple solutions, options that can be selected to build. In this version there are multiple ways to build thermal compensation for the VCOs depending on component availability (NTC based, PTS100 based); it contains a precision +/-5V circuit with output connectors that can be used on the UI board if necessary; and misc. options.

**Stable** — This is the opinionated, tested and recommended version of the core board. Compared to the experimental board:

- This board uses PTS100 for thermal compensation
- It is designed for SMD manufacturing. Note that some parts are not available at JLCPCB. We kept these THT whereever it's possible for easy build.
- +/-5V precision output is removed. Instead +/-12V resistor divider is used where needed, as approximate values were fine on the Core board.
-