# Toshiba TCX-1007 Replacement - Experimental V2 (Prototype)

⚠️ **WARNING: THIS DESIGN IS COMPLETELY UNTESTED AND UNVERIFIED.** ⚠️

This folder contains the design files for the **V2 Variant** of the Toshiba TCX-1007 ULA replacement. Unlike the proven V1 design, this version has **never been manufactured, assembled, or hardware-tested**. Use these files entirely at your own risk.

## Key Differences from V1
* **Reduced Footprint:** Designed to create a smaller overall PCB module to help with tight motherboard clearance.
* **Component Changes:** Swapped standard logic families for **74HCT series** chips.
* **New PPI Package:** Utilizing the **Renesas CMQ82C55AZ** (44-pin MQFP package) instead of a traditional DIP or PLCC chip.

## Crucial Caveats & Known Risks
1. **Unverified Footprints:** The component footprints—especially for the Renesas MQFP package and the 74HCT logic ICs—**have not been physically checked** against real components for correct pad sizing or pitch alignment.
2. **Untested Logic/Timing:** While the underlying logic circuit matches the functional V1 board, the electrical characteristics and signal timings using the 74HCT family and the Renesas chip have not been validated on real hardware.
3. **Physical Fit:** It is unknown if this layout resolves the tight layout restrictions found in regional variants like the Japanese HX-10DP.

## Component Sourcing Notes
* **Logic:** Ensure you use **74HCT series** components as designated in the schematic. 
* **PPI:** The layout specifies a **Renesas CMQ82C55AZ** (MQFP). Double-check the manufacturer's datasheet dimensions against the PCB layout before ordering any boards.

## Community Call for Beta Testing
If you choose to manufacture this board, please proceed with caution. We highly recommend:
1. Printing the PCB layout on paper at a 1:1 scale to manually verify component footprints before ordering fabrication.
2. Sharing your findings, fixes, or success stories via the GitHub Issues page to help graduate this design out of its experimental state.
