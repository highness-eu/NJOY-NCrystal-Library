# NJOY+NCrystal Library

This repository contains a library of thermal scattering files generated with a special version of [NJOY2016](https://github.com/njoy/NJOY2016), modified to compute coherent scattering with [NCrystal](https://github.com/mctools/ncrystal). This tool, called NJOY+NCrystal, is available [here](https://github.com/highness-eu/NJOY2016).

For each material, TSL files in the [ENDF-6](https://www.nndc.bnl.gov/csewg/docs/endf-manual.pdf) and [ACE](https://github.com/NuclearData/ACEFormat/blob/master/ACEFormat.pdf) formats are included. Two versions are provided: the standard format that can either contain coherent or incoherent elastic, and one in the improved format recently [proposed](https://indico.bnl.gov/event/7233/contributions/43822/), called "mixed elastic", which contains both. This new format is not yet supported in MCNP, but a modified version of [OpenMC](https://docs.openmc.org/) that supports it is provided in a [separate repository](https://github.com/highness-eu/openmc).

All temperatures are provided in ENDF-6 format, but only the first one is provided in ACE format because of space requirements. Nevertheless, pdf plots created with ACER are provided for all the temperatures.

Evaluations in this release were generated with [NJOY2016 2016.61_njoyncrystal](https://github.com/highness-eu/NJOY2016/tree/2016.61_njoyncrystal) and [NCrystal v2.6.1_njoyncrystal](https://github.com/highness-eu/ncrystal/tree/v2.6.1_njoyncrystal).

More details can be found in the following papers:

* K. Ramic, J.I. Marquez Damian, T. Kittelmann, D.D DiJulio, D. Campi, M. Bernasconi and V. Santoro. "NJOY+NCrystal: an open-source tool for creating thermal neutron scattering libraries"  Nuclear Instruments and Methods in Physics Research Section A: Accelerators, Spectrometers, Detectors and Associated Equipment 1027 (2022) 166227, https://doi.org/10.1016/j.nima.2021.166227
* X.-X. Cai and T. Kittelmann, NCrystal: A library for thermal neutron transport, Computer Physics Communications 246 (2020) 106851, https://doi.org/10.1016/j.cpc.2019.07.015

This work was funded by HighNESS project at European Spallation Source ERIC under HORIZON 2020 grant agreement ID: 951782.

## List of materials:
112 new and updated materials are provided in the library:

| Material | Name           | Compound Number | Temperatures |
|----------|----------------|-----------------|--------------|
| AgBr | Silver Bromide | 1 | 293.6 20 77 100 200 300 400 500 600 700 K |
| Ag | Silver | 2 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 K |
| Al2O3 | Corundum | 3 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 2200 K |
| Al4C3 | Aluminium Carbide | 4 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 2000 2400 K |
| AlN | Aluminum Nitride | 5 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2500 2700 K |
| Al | Aluminum | 6 | 293.6 20 77 100 200 300 400 500 600 800 900 K |
| Au | Gold | 7 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 K |
| BaF2 | Barium Fluoride | 8 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 K |
| BaO | Barium Oxide | 9 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 K |
| Ba | Barium | 10 | 293.6 20 77 100 200 300 400 500 600 800 1000 K |
| Be3N2 | Beryllium Nitride | 12 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 2000 2400 K |
| Bi2O3-beta | Bismuth Trioxide | 18 | 600 650 700 750 800 850 900 K |
| Bi | Bismuth | 22 | 293.6 20 77 100 200 300 400 500 K |
| C-diamond | Diamond | 23 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 2500 3000 3500 4000 K |
| CF4-alpha | Carbon Tetrafluoride | 25 | 20 25 30 35 40 45 50 55 60 65 70 K |
| CaCO3 | Aragonite | 26 | 293.6 20 77 100 200 300 400 500 600 800 1000 K |
| CaF2 | Calcium Flouride | 27 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 K |
| CaH2 | Calcium Hydride | 28 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 K |
| CaOH2 | Calcium Hydroxide | 29 | 293.6 20 77 100 200 300 400 500 600 700 800 K |
| CaO | Calcium Oxide | 30 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 2000 2500 K |
| CaZrO3 | Calcium Zirconate | 31 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 2000 2500 K |
| Ca | Calcium | 32 | 293.6 20 77 100 200 300 400 500 600 700 K |
| CeO2 | Cerium Oxide | 33 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2500 K |
| Cr | Chromium | 34 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 1800 2000 K |
| Cu2O | Cuprite | 35 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 K |
| Cu | Copper | 36 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 K |
| Dy2O3 | Dysprosium Oxide | 37 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2400 K |
| Fe-alpha | Alpha Iron | 38 | 293.6 20 77 100 200 300 400 500 600 800 1000 1100 K |
| Fe-gamma | Gamma Iron | 39 | 1200 1300 1400 1500 1600 1700 1800 K |
| GaN | Gallium Nitride | 40 | 293.6 20 77 100 200 300 400 600 800 1000 1500 1900 K |
| GaSe | Gallium Selenide | 42 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 K |
| Ge3Bi4O12 | Bismuth Germanate | 43 | 293.6 20 77 100 200 300 400 500 600 800 1000 1300 K |
| GeTe | Germanium Telluride | 44 | 293.6 20 77 100 200 300 400 500 600 K |
| Ge | Germanium | 45 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 K |
| Ho2O3 | Holmium Oxide | 47 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2400 K |
| KBr | Potassium Bromide | 48 | 293.6 20 77 100 200 300 400 500 600 800 1000 K |
| KF | Potassium Flouride | 49 | 293.6 20 77 100 200 300 400 600 800 1000 1100 K |
| KOH | Potassium Hydroxide | 50 | 293.6 20 77 100 200 300 400 500 K |
| K | Potassium | 51 | 293.6 20 77 100 150 200 250 300 K |
| La2O3 | Lanthanum Oxide | 52 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2500 K |
| LaBr3 | Lanthanum Bromide | 53 | 293.6 20 77 100 200 300 400 500 600 800 1000 K |
| Li2O | Lithium Oxide | 54 | 293.6 20 77 100 200 300 400 600 800 1000 1500 1700 K |
| Li3N | Lithium Nitride | 55 | 293.6 20 77 100 200 300 400 600 800 1000 K |
| LiF | Lithium Flouride | 56 | 293.6 20 77 100 200 300 400 600 800 1000 1100 K |
| LiH | Lithium Hydride | 57 | 293.6 20 77 100 200 300 400 500 600 700 800 900 K |
| Lu2O3 | Lutetium Oxide | 58 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2400 K |
| Mg2SiO4 | Magnesium Silicate | 59 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2100 K |
| MgAl2O4 | Magnesium Aluminate Spinel | 60 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 2400 K |
| MgCO3 | Magnesium Carbonate | 61 | 293.6 20 77 100 150 200 250 300 350 400 500 600 K |
| MgD2 | Magnesium Deuteride | 62 | 293.6 20 77 100 200 300 400 500 600 K |
| MgH2 | Magnesium Hydride | 64 | 293.6 20 77 100 200 300 400 500 600 K |
| MgOH2 | Magnesium Hydroxide | 65 | 293.6 20 77 100 200 300 400 500 600 K |
| Mg | Magnesium | 67 | 293.6 20 77 100 200 300 400 500 600 800 900 K |
| Mo | Molybdenum | 68 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 2500 K |
| Na4Si3Al3O12Cl | Sodalite | 69 | 293.6 20 77 100 200 300 400 500 600 800 1000 1300 K |
| NaBr | Sodium Bromide | 72 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2100 K |
| NaCl | Sodium Chloride | 73 | 293.6 20 77 100 200 300 400 500 600 700 800 900 1000 K |
| NaF | Sodium Flouride | 74 | 293.6 20 77 100 200 300 400 600 800 1000 1200 K |
| NaI | Sodium Iodide | 75 | 293.6 20 77 100 200 300 400 500 600 800 900 K |
| NaMgH3 | Sodium Magnesium Hydride | 76 | 293.6 20 77 100 200 300 400 500 600 K |
| NaOH | Sodium Hydroxide | 77 | 293.6 20 77 100 200 300 400 500 590 K |
| Na | Sodium | 78 | 293.6 20 77 100 150 200 250 300 350 K |
| Nb | Niobium | 79 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 2500 K |
| Nd2O3 | Neodymium Oxide | 80 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2400 K |
| Ni | Nickel | 81 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 K |
| P2O5 | Phosphorus Pentoxide | 82 | 293.6 20 77 100 200 300 400 500 600 K |
| Pb3O4 | Lead Oxide | 83 | 293.6 170 100 200 300 400 500 600 800 K |
| PbCO3 | Lead Carbonate | 84 | 293.6 20 77 100 200 300 400 500 580 K |
| PbF2 | Lead Flouride | 85 | 293.6 20 77 100 200 300 400 500 600 700 800 900 1000 K |
| PbO-alpha | Alpha Lead Monoxide | 87 | 293.6 20 77 100 200 300 400 500 600 800 1000 1100 K |
| PbO-beta | Beta Lead Monoxide | 88 | 293.6 20 77 100 200 300 400 500 600 800 1000 1100 K |
| PbS | Lead Sulfide | 89 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1300 K |
| Pb | Lead | 90 | 293.6 20 77 100 200 300 400 500 600 K |
| Pd | Palladium | 91 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 1800 K |
| Pt | Platinum | 93 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 K |
| Rb | Rubidium | 94 | 293.6 20 77 100 150 200 250 300 K |
| Sc | Scandium | 96 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 1800 K |
| SiC-alpha | Alpha Silicon Carbide | 98 | 1973 2000 2100 2200 2400 2600 2800 3000 3100 K |
| SiC-beta | Beta Silicon Carbide | 99 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 1900 K |
| SiLu2O5 | Silicon Lutetium Oxide | 100 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 2000 2400 K |
| SiO2-alpha | Alpha Quartz | 101 | 293.6 20 77 100 200 300 400 500 600 800 K |
| SiO2-beta | Beta Quartz | 102 | 846.15 900 1000 1100 1200 1300 1400 1500 1600 1700 1800 1900 K |
| SiY2O5 | Silicon Yttrium Oxide | 103 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 2000 2300 K |
| Si | Silicon | 104 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 K |
| Sn | Tin | 107 | 293.6 300 350 400 450 500 K |
| SrF2 | Strontium Fluoride | 108 | 293.6 20 77 100 200 300 400 500 600 800 1000 1400 K |
| SrH2 | Strontium Hydride | 109 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1300 K |
| Sr | Strontium | 111 | 293.6 20 77 100 200 300 400 500 600 700 800 1000 K |
| Th3N4 | Thorium Nitride | 112 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2500 3000 K |
| ThO2 | Thorium Dioxide | 113 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2500 3000 3500 K |
| ThSiO4 | Huttonite | 114 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 K |
| TiO2-anatase | Anatase | 115 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 2000 K |
| TiO2-rutile | Rutile | 116 | 873 1000 1200 1400 1600 1800 2000 K |
| Ti | Titanium | 117 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 1800 K |
| TlBr | Thalium Bromide | 118 | 293.6 20 77 100 200 300 400 600 700 K |
| Tm2O3 | Thulium Oxide | 119 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2400 K |
| UF6 | Uranium Hexaflouride | 120 | 293.6 20 77 100 200 300 320 K |
| V | Vanadium | 122 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 1800 2000 K |
| W | Tungsten | 123 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 2500 3500 K |
| Y2O3 | Yttrium Oxide | 124 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 2500 K |
| Y3Al5O12 | Yttrium Aluminium Garnet | 125 | 293.6 20 77 100 200 300 400 600 800 1000 1500 2000 2500 2900 K |
| YAlO3 | Yttrium Orthoaluminate | 126 | 293.6 20 77 100 200 300 400 500 600 800 1000 1500 2000 K |
| Y | Yttrium | 127 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 K |
| ZnF2 | Zinc Flouride | 128 | 293.6 20 77 100 200 300 400 600 800 1000 K |
| ZnO | Zinc Oxide | 129 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 2200 K |
| ZnS-sphalerite | Zinc Sulfide | 130 | 293.6 20 77 100 200 300 400 500 600 800 1000 1300 K |
| Zn | Zinc | 131 | 293.6 20 77 100 200 300 400 500 600 K |
| ZrF4-beta | Beta Zirconium Tetrafluoride | 132 | 773 800 850 900 950 1000 1050 1100 1150 K |
| ZrO2-tet | Tetragonal Zirconium Dioxide | 133 | 1443.15 1500 1600 1700 1800 1900 2000 2200 2400 2600 K |
| ZrO2 | Zirconium Dioxide | 134 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 K |
| ZrSiO4 | Zirconium Orthosilicate | 135 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1400 1600 1800 K |
| Zr | Zirconium | 136 | 293.6 20 77 100 200 300 400 500 600 800 1000 1200 1500 2000 K |
