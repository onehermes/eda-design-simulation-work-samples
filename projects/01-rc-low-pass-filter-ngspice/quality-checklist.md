# Quality Checklist

- [ ] Ground node is present
- [ ] Units are clear and consistent
- [ ] AC source is configured
- [ ] Simulation command is included
- [ ] Expected behavior is documented
- [ ] Limitations are stated

## Review Notes

- The circuit should use SPICE ground node `0`.
- Resistance and capacitance values should be written with explicit units.
- The `.ac` command should be visible in the netlist.
- The control block should run the simulation and produce a plot or print output.
- The documentation should explain the expected cutoff frequency.
- The sample should state that simulation is not the same as hardware validation.
