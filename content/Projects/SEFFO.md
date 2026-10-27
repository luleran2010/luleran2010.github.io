---
preview: "[[Pasted image 20261028001713.png]]"
---

# SEFFO

GitHub: [luleran2010/SEFFO: Algorithm for searching adsorption sites and configurations on 2D materials](https://github.com/luleran2010/SEFFO)

![[Pasted image 20261028001713.png]]

Algorithm for searching adsorption sites and configurations on 2D materials

Screener and Enumeration with Force-Field Optimization (SEFFO) is an algorithm to find the adsorption sites and configurations on surface of 2D materials.

## File structure

A calculation of SEFFO needs following directory structure
```
- sites/
	- inp_sites.json
	- inp_slab.json
	- POSCAR
- mol/
	- inp_init.json
	- inp_mol.json
	- slab_bader.json
	- mol_bader.json
	- POSCAR_mol
	- inp_loop.json
	- inp_loop/
		- round1/
		- .../
		- run.sh
```

## Procedures

1. Run *find_sites.py* in *sites/* folder to find all the adsorption sites. See [](Finding%20Adsorption%20Sites.md) for details.
2. Run *guess_initials.py* in *mol/* folder to generate initial guesses of adsorption configurations. See [](Guessing%20Initial%20Structures.md) for details.
3. Run *calc_loop.py* in *mol/* folder to start the DFT-screen loop. See [](DFT-Screen%20Loop.md) for details.

## References

Lu L, Cao W, Botella R. Screener and enumerator with force-field optimization (SEFFO): Algorithm for searching adsorption sites and configurations on 2D materials[J]. Computer Physics Communications, 2025, 308: 109440. DOI: https://doi.org/10.1016/j.cpc.2024.109440
