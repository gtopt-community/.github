# GTOpt Community

<img src="banner.png" width="100%"
     alt="GTOpt Community: open-source energy-system optimization / optimización abierta de sistemas energéticos. Electricity, water, fuels, hydrogen, ammonia and heat, from 15 minutes to 30 years.">

**GTOpt** is an open-source optimizer for **planning and operating
energy systems**: generation, transmission, storage and demand expansion,
hydrothermal scheduling with SDDP, and unit commitment and dispatch. It
builds sparse LP/MIP models in C++ and solves them with the solver of
your choice (HiGHS, CBC/CLP, SCIP, cuOpt, CPLEX, Gurobi, MindOpt).

### One consistent model, from minutes to decades

The same formulation of electricity, water, fuels and LNG, hydrogen,
ammonia and heat is used from **daily operation** (15-minute to hourly
blocks) through the **medium term** (months to years, SDDP) to
**expansion planning** (decades). The scales are coupled through SDDP
optimality cuts (water values, storage opportunity costs) and
feasibility cuts (reservoir levels, water rights), so results agree
across horizons.

### Highlights

- **National scale**: built and validated on the Chilean national system
  (SEN), with its network, hydro cascades and irrigation agreements.
- **Storage and water values**: reservoirs, cascades, pumped hydro and
  batteries, with water values and opportunity costs per block.
- **Emissions**: CO₂-eq and local pollutants, caps and prices by zone,
  marginal emission factors per bus and hour, and the CO₂ impact of
  storage.
- **Constraints without code**: PAMPL, an AMPL-like language for
  operating rules such as irrigation agreements.
- **Open and auditable**: published formulation, exportable LP files, LP
  fingerprints, and JSON + Parquet data readable by any tool.
- **Interoperable**: converters from PLP, PLEXOS, PSR SDDP, PSS/E,
  pandapower and more.
- **From laptop to server and GPU**, with careful memory use.
- **Next**: offer-based electricity markets (energy and ancillary
  services, capacity, transmission rights).

### Repositories

| Repository | What it is |
|---|---|
| [gtopt](https://github.com/gtopt-community/gtopt) | The solver, Python tools, browser GUI and web service |

### Get started

- [README and quick start](https://github.com/gtopt-community/gtopt#quick-start)
- [Documentation](https://gtopt-community.github.io/gtopt/)
- [Questions and ideas: Discussions](https://github.com/gtopt-community/gtopt/discussions)
- [Contributing](https://github.com/gtopt-community/gtopt/blob/master/CONTRIBUTING.md)
  (a CLA is required for pull requests)
- [Licensing](https://github.com/gtopt-community/gtopt/blob/master/LICENSING.md):
  AGPL-3.0-or-later with a solver plugin exception, or a commercial
  licence; the Extension SDK is Apache-2.0
- [Publications](https://github.com/gtopt-community/gtopt/blob/master/PUBLICATIONS.md),
  starting with the FESOP paper
  ([IEEE KPEC 2022](https://doi.org/10.1109/KPEC54747.2022.9814781))
- Support, maintenance and training: Black Bear Engineering SpA

---

### En español

**GTOpt** es un optimizador abierto para **planificar y operar sistemas
energéticos**, desarrollado en Chile: expansión de generación,
transmisión, almacenamiento y demanda; programación hidrotérmica con
SDDP; y predespacho y despacho.

- **Un mismo modelo, de minutos a décadas**: la operación diaria
  (bloques de 15 minutos a una hora), el mediano plazo (meses a años) y
  la planificación (décadas) usan la misma formulación de electricidad,
  agua, combustibles y GNL, hidrógeno, amoníaco y calor, acoplados con
  cortes de optimalidad y factibilidad de SDDP.
- **Escala nacional**: probado en el SEN, con su red, cuencas y
  convenios de riego (Maule, Laja).
- **Valores del agua y costos de oportunidad** de embalses y baterías.
- **Emisiones** de CO₂ y contaminantes locales, factores marginales por
  barra y hora, e impacto del almacenamiento en la reducción de CO₂.
- **Abierto y auditable**: formulación publicada, LP exportable y datos
  en JSON y Parquet.
- **Próximo paso**: mercados con ofertas (energía y servicios
  complementarios, suficiencia, derechos de transmisión).

Las contribuciones son bienvenidas; las preguntas pueden hacerse en
español en
[Discussions](https://github.com/gtopt-community/gtopt/discussions).
