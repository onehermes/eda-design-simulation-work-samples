# Circuit Notes

This is a standard first-order RC low-pass filter.

## Node Summary

- `in` is the input node
- `out` is the filtered output node
- `0` is the SPICE ground reference

## Why the Circuit Works

At low frequencies, the capacitor impedance is high, so the output tracks the input through the resistor with very little attenuation.

At higher frequencies, the capacitor impedance becomes lower, so more of the signal is shunted to ground and the output falls.

## Simple Math Check

For `R = 1 kOhm` and `C = 100 nF`:

`f_c = 1 / (2*pi*R*C) ~ 1.59 kHz`

That expected value is useful as a check before looking at simulation output.

## Simulation Note

The AC source is set to `1 V`, which makes the output magnitude easy to interpret as the transfer response directly.
