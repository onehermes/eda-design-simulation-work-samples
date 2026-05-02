# Expected Results

This filter should behave like a standard first-order low-pass network.

## What To Expect

| Frequency range | Expected behavior |
| --- | --- |
| Well below `1.59 kHz` | Output should be close to the input amplitude |
| Around `1.59 kHz` | Output should be about `-3 dB` relative to the input and the phase should be near `-45 deg` |
| Well above `1.59 kHz` | Output should drop with a slope of about `-20 dB/decade` |

## How To Interpret The Plot

- The magnitude plot should stay near `0 dB` at low frequencies.
- The response should begin rolling off near the calculated cutoff frequency.
- The phase plot should trend from near `0 deg` toward `-90 deg` as frequency increases.

## Validation Idea

If the response looks wrong, check the following first:

- Ground node `0` is present
- The input source is configured as an AC source
- The capacitor value is `100 nF`, not `100 uF`
- The resistor value is `1 kOhm`, not `1 MOhm`
- The AC sweep range is wide enough to show the roll-off

## Limitation

This simulation demonstrates transfer behavior, but it does not prove PCB parasitics, part tolerance effects, or real-world assembly quality.
