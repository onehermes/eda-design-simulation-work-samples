# Bill of Materials

| Ref | Part | Example Value | Purpose | Notes |
| --- | --- | --- | --- | --- |
| U1 | NE555 timer | NE555 or equivalent | Generates the astable timing waveform | Verify package and pinout before footprint assignment |
| R1 | Timing resistor | 10 kOhm | Sets charge/discharge timing with R2 and C1 | Example value only |
| R2 | Timing resistor | 100 kOhm | Helps set blink period and duty cycle | Example value only |
| C1 | Timing capacitor | 10 uF | Stores charge for the oscillator timing loop | Check polarity if electrolytic |
| LED1 | Indicator LED | Generic LED | Visible output indicator | Check forward voltage and current |
| R3 | Current-limiting resistor | 330 Ohm | Limits LED current | Confirm with supply voltage and LED type |
| J1 | Power input | 5 V input connector | Provides board power | Confirm connector style and polarity |

## Notes

- Values are illustrative, not a finished production design.
- The final resistor and capacitor values should be checked against the desired blink rate.
- LED current should be calculated before layout or hardware claims are made.
