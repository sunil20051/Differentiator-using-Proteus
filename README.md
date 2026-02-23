## Experiment No: 3
DIFFERENTIATOR USING OP-AMP (μA741)
## Aim
To design and simulate a Differentiator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the rate of change of input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Capacitor C = 0.01 µF
•	Resistor Rf = 10 kΩ
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
<img width="1600" height="901" alt="image" src="https://github.com/user-attachments/assets/0f1a19bd-f6f4-45e4-bc23-e1f9f6be5d4a" />

## Connection Details:
•	Input signal → Capacitor (C) → Inverting terminal (Pin 2)
•	Feedback resistor (Rf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
A Differentiator circuit produces an output voltage proportional to the rate of change of input voltage.
## Working Principle:
•	When input changes rapidly → output amplitude increases
•	When input is constant → output is zero
•	Output is inverted
## Procedure
1.	Open Proteus software.
2.	Select μA741, capacitor, resistor, signal generator, and CRO.
3.	Connect circuit in differentiator configuration.
4.	Apply ±15V power supply.
5.	Set input sine wave (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.

## Tabulation
| S.No | Input Signal    | Frequency | Expected Output               | Practical Observation        |
| ---- | --------------- | --------- | ----------------------------- | ---------------------------- |
| 1    | Sine Wave       | 1 kHz     | Cosine wave (90° phase shift) | Phase shifted sine observed  |
| 2    | Square Wave     | 1 kHz     | Triangular Wave               | Triangular waveform obtained |
| 3    | Triangular Wave | 1 kHz     | Parabolic Wave                | Slight curved waveform seen  |
| 4    | Sine Wave       | 500 Hz    | Larger amplitude cosine       | Increased output amplitude   |
| 5    | Sine Wave       | 2 kHz     | Smaller amplitude cosine      | Reduced output amplitude     |
## Waveforms
•	Sine input → Cosine output (90° phase shift)
•	Square input → Positive & negative spikes
•	Triangular input → Square wave
<img width="1373" height="875" alt="image" src="https://github.com/user-attachments/assets/1ca476a2-7720-49cc-b0ce-06347e62c177" />

## Result
The Differentiator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the rate of change of input voltage.
The circuit behaves as a differentiator.
## Conclusion
•	Output depends on frequency.
•	Output leads input by 90° (for sine input).
•	Higher frequency → Higher output amplitude.
•	Used in wave shaping and signal processing applications.
## Viva Questions
1.	What is a differentiator?
2.	Write the output equation of differentiator.
3.	Why is output leading input?
4.	What happens at very high frequency?
5.	What is practical differentiator?

## Answer
1.  A differentiator is an op-amp circuit in which the output voltage is proportional to the rate of change (derivative) of the input voltage. It uses a capacitor at the input and a resistor in the feedback path.
2.  Vout = -RC(dVin/dt)
3.  The output depends on the rate of change of the input. For a sine wave input, differentiation produces a cosine wave, which is shifted by +90°, so the output leads the input by 90°.
4.  At very high frequency, the gain increases significantly, which can cause noise amplification and instability. The circuit may become unstable and produce distorted output.
5.  A practical differentiator is a modified differentiator circuit that includes an additional resistor and capacitor to reduce noise and improve stability at high frequencies.

