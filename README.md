# Total energies of neutral isolated atoms

**Author:** Aaron D. Kaplan (@esoteric-ephemera)
**Contact info:** aaron.kaplan.physics [@] gmail.com

### Description:

This respository contains total energies of isolated neutral atoms computed with plane-wave DFT using the following density functional approximations:
- [PBE GGA](https://doi.org/10.1103/PhysRevLett.77.3865)
- [SCAN meta-GGA](https://doi.org/10.1103/PhysRevLett.115.036402)
- [r<sup>2</sup>SCAN meta-GGA](https://doi.org/10.1021/acs.jpclett.0c02405)

These energies are needed for computing cohesive (atomization) energies of solids in the [Materials Project](https://next-gen.materialsproject.org/). For consistency with existing Materials Project data, these energies are computed using the [Vienna *ab initio* Simulation Package (VASP)](https://www.vasp.at/) using the [`MPStaticSet`](https://github.com/materialsproject/pymatgen/blob/31f1e1fb8cc1bb517d59ea8e484965bb641c42a0/src/pymatgen/io/vasp/sets.py#L1414) and [`MPScanStaticSet`](https://github.com/materialsproject/pymatgen/blob/31f1e1fb8cc1bb517d59ea8e484965bb641c42a0/src/pymatgen/io/vasp/sets.py#L1567) input sets defined in `pymatgen`.

For ease of access, the data is provided in CSV format in `atomic_energies.csv`. All energy units are eV.