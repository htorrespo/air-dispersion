# Factores de conversion

<!--
https://www.epa.gov/sites/production/files/2020-11/documents/appa.pdf

Make your own mock API (super simple), 16 min
https://www.youtube.com/watch?v=FLnxgSZ0DG4

Write a Unit Test for JavaScript (super simple!), 13 min
https://www.youtube.com/watch?v=Rumf96j0cR0

Hay que utilizar expresiones regulares en javascript para transformar la API

Construccion de una API para conversion de unidades
-->

TYPICAL PARAMETERS OF VARIOUS FUELS

Fuel | kcal | Btu | % Sulphur | % Ash
-----|------|-----|-----------|-------------
Bituminous Coal | 7.200/kg | 13.000/lb | 0.6-5.4 | 4-20
Anthracite Coal | 6.810/kg | 12.300/lb | 0.5-1.0 | 7.0-16.0
Lignite (@ 35% moisture) | 3.990/kg | 7.200/lb | 0.7 | 6.2
Wood (@ 40% moisture) | 2.880/kg | 5.200/lb | N | 1-3
Bagasse (@ 50% moisture) | 2.220/kg | 4.000/lb | N | 1-2
Bark (@ 50% moisture) | 2.492/kg | 4.500/lb | N | 1-3b
Coke Byproduct | 7.380/kg | 13.300/lb | 0.5-1.0 | 0.5-5.0
Residual Oil | 9.98 x 10^6/m3 | 150.000/gal | 0.5-4.0 | 0.05-0.1
Distillate Oil | 9.30 x 10^6/m3 | 140.000/gal | 0.2-1.0 | N
Diesel | 9.12 x 10^6/m3 | 137.000/gal | 0.4 | N
Gasoline | 8.62 x 10^6/m3 | 130.000/gal | 0.03-0.04 | N
Kerosene | 8.32 x 10^6/m3 | 135.000/gal | 0.02-0.05 | N
Liquid Petroleum Gas | 6.25 x 10^6/m3 | 94.000/gal | N | N
Natural Gas | 9.341/m3 | 1.050/SCF | N | N
Coke Oven Gas | 5.249/m3 | 590/SCF | 0.5-2.0 | N
Blast Furnace Gas | 890/m3 | 100/SCF | N | N

N = negligible.

Ash content may be considerably higher when sand, dirt, etc., are present.

La misma tabla en formato _terminal_, se puede crear un archivo en formato _.txt_ o _.csv_.
```terminal
Fuel, kcal, Btu, % Sulphur, % Ash
Bituminous Coal, 7.200/kg, 13.000/lb, 0.6-5.4, 4-20
Anthracite Coal, 6.810/kg, 12.300/lb, 0.5-1.0, 7.0-16.0
Lignite (@ 35% moisture), 3.990/kg, 7.200/lb, 0.7, 6.2
Wood (@ 40% moisture), 2.880/kg, 5.200/lb, N, 1-3
Bagasse (@ 50% moisture), 2.220/kg, 4.000/lb, N, 1-2
Bark (@ 50% moisture), 2.492/kg, 4.500/lb, N, 1-3b
Coke Byproduct, 7.380/kg, 13.300/lb, 0.5-1.0, 0.5-5.0
Residual Oil, 9.98 x 10^6/m3, 150.000/gal, 0.5-4.0, 0.05-0.1
Distillate Oil, 9.30 x 10^6/m3, 140.000/gal, 0.2-1.0, N
Diesel, 9.12 x 10^6/m3, 137.000/gal, 0.4, N
Gasoline, 8.62 x 10^6/m3, 130.000/gal, 0.03-0.04, N
Kerosene, 8.32 x 10^6/m3, 135.000/gal, 0.02-0.05, N
Liquid Petroleum Gas, 6.25 x 10^6/m3, 94.000/gal, N, N
Natural Gas, 9.341/m3, 1.050/SCF, N, N
Coke Oven Gas, 5.249/m3, 590/SCF, 0.5-2.0, N
Blast Furnace Gas, 890/m3, 100/SCF, N, N
```

THERMAL EQUIVALENTS FOR VARIOUS FUELS

Type Of Fuel | kcal | Btu (gross)
------ | ------|----------
Solid fuels | |
Bituminous coal | (5.8 to 7.8) x 10^6/Mg | (21.0 to 28.0) x 10^6/ton 
Anthracite coal | 7.03 x 10^ 6/Mg | 25.3 x 10^6/ton
Lignite | 4.45 x 10^6/Mg | 16.0 x 10^6/ton
Wood | 1.47 x 10^6/m3 | 21.0 x 106/cord
Liquid fuels | |
Residual fuel oil | 10x10^3/liter | 6.3x10^6/bbl
Distillate fuel oil | 9.35 x 10^3/liter | 5.9x10^6/bbl
Gaseous fuels | |
Natural gas | 9.350/m3 | 1.050/ft3
Liquefied petroleum gas | |
Butane | 6.480/liter | 97.400/gal
Propane | 6.030/liter | 90.500/gal

