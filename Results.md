## Output Waveform and Frequency Analysis

The VCO was simulated using **180 nm CMOS technology**. Each inverter stage uses the following transistor dimensions:

- **Channel Length (L): 180 nm**
- **Transistor Width (W): 1 µm**

These dimensions determine the **drive strength of the CMOS transistors**, which directly affects the **propagation delay** of the inverter stages and therefore the oscillation frequency of the ring oscillator.

---

## Simulated Output Waveforms

![VCO Output Waveform](images/vco_waveform.png)

The above plot shows the simulated node voltages of the ring oscillator. The signals correspond to different nodes in the inverter chain.

### Observations

- The **blue waveform** represents the output of one inverter stage.
- The **green waveform** represents another internal node of the oscillator.
- The signals are **phase shifted**, which confirms the propagation of the signal through multiple inverter stages.
- The output oscillates between approximately **0 V and 1.8 V**, corresponding to the CMOS supply voltage.

---

## Frequency Measurement

Using waveform cursors from the simulation:

- **Cursor 1:** 5.6900329 ns  
- **Cursor 2:** 5.0000000 ns  
- **Measured Period:** ≈ **690 ps**

Therefore,

\[
T \approx 690\ ps
\]

\[
f = \frac{1}{T} \approx 1.449\ GHz
\]

---

## Result

The **CMOS ring oscillator VCO designed using 180 nm technology (W = 1 µm, L = 180 nm)** produces a stable oscillation with an approximate frequency of:

**≈ 1.45 GHz**

The oscillation frequency is primarily determined by the **propagation delay of each inverter stage and the load capacitance at the output nodes**.
