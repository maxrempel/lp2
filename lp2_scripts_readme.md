# LP2 Major Revision 1 - Script Handover

## Paper Details
- **Submitted Title**: "Coupling of transposable elements near chromatin contacts"
- **Submission Date**: 50911 (September 11, 2025)
- **Journal**: MDPI Genes
- **Manuscript ID**: genes-3806812
- **Status**: Major revision requested

## Analysis Pipeline

### Script 1: Hotspot/Coldfield Detection
**Script**: `R441v6_Hotco_Walnut_Spock_NoSkip`  
**Output Path**: `/home/ubuntu/00HA1py/out/hotco/250908_(R441v6_Hotco_Walnut_Spock_NoSkip)_results/paired_hotcold_all.pkl`  
**Function**: Identifies focal contact hotspots and matched coldfields from Walnut Micro-C data

### Script 2: TE Homotypic Analysis  
**Script**: `R622v5_Walnut_SpecPlot_5Plots_ProperTitles`  
**Input Path**: `/home/ubuntu/00HA1py/out/hotco/250908_(R441v6_Hotco_Walnut_Spock_NoSkip)_results/paired_hotcold_all.pkl`  
**Output Path**: `/home/ubuntu/00HA1py/out/te_analysis/250909_R622v5_Walnut_SpecPlot_5Plots_results/`  
**Function**: Analyzes transposable element homotypic pairing at chromatin contacts

### Script 3: Local Post-Processing  
**Script**: `L910v13_Walnut_Adjusted_Plot_Analysis_From_PKL`  
**Input Path**: `C:\Users\mremp\00HA1py\post\hotco\250910_R622v6_Walnut_SpecPlot_6Plots_results\*.pkl`  
**Output Path**: `C:\Users\mremp\00HA1py\out\walnut_plots_[timestamp]\`  
**Function**: Creates publication-ready 6-panel figure with adjusted formatting, MIRb scaling (×0.65), and improved visualization

## Data Flow
Walnut Micro-C (4DNFI3ULPBI5) → R441v6 → paired_hotcold_all.pkl → R622v5 → L910v13 → Paper Figures 2,3,5

## GitHub Repository
https://github.com/maxrempel/lp2