![Microchip logo](images/microchip.png)

# Low-Voltage differential signal interface using OPA of PIC16F17146 Mindi Simulation

**Note : Currently, this repository contains Mindi model of PIC18-Q41 family's OPAMP module. Mindi model of PIC16F17146 family's OPAMP module will be available soon.**

In this example, the OPA module of PIC16F17146 is used to form a differential amplifier configuration. This Mindi simulation simulates the circuit described in the [Pressure Sensor interface with Differential output voltage Code Examples](https://github.com/microchip-pic-avr-examples/pic16f17146-pressure-sensor-interface-mplab-mcc). The simulation consists of a model of the PIC16F17146 OPA module, resistor bridge and generic components representing the rest of the functionality of the circuit. Another Op-Amp circuit is representing constant current circuit.
For more information about getting started with and using the MPLAB Mindi Analog Simulator please refer to the following resources:
- [Using the MPLAB Mindi Analog Simulator with the 8-Bit Operational Amplifier Module Technical Brief](https://www.microchip.com/DS90003293)
- [Microchip Developer - Introduction to MPLAB Mindi Analog Simulator](https://www.microchipdeveloper.com/mindi:mindi-analog-simulator-introduction)
- [Getting Started with the MPLAB Mindi Analog Simulator Document](https://www.microchip.com/DS50002564)

![Circuit](images/ExampleCircuit.svg)

## Related Documentation

* [PIC16F17146 Product Page](https://www.microchip.com/en-us/product/PIC16F17146)
* [PIC16F17146 Data Sheet](https://www.microchip.com/DS40002343)
* [PIC16F17146 Curiosity Nano User Guide](https://www.microchip.com/DS50003037)

## Related Software
* [Pressure Sensor interface with Differential output voltage Code Examples](https://github.com/microchip-pic-avr-examples/pic16f17146-pressure-sensor-interface-mplab-mcc)

### Mindi Simulation
![Mindi](images/mplab-mindi-analog-simulator.png)

Download and open the **Mindi schematic [here](https://github.com/microchip-pic-avr-examples/pic16f17146-differential-signal-interface-to-OPA-mindi/releases/tag/1.0.0)**

Press the _play_ button to simulate with an example stimulus source.

### Tweaking
User can tweak the value of R3 and R3 (RES) in terms of accuracy and variation in value to simulate overall bridge output (Here is is simulating overall variation between 20 to 20.8 KOhm). The given simulation example is having 10 points (Sweep parameters).

There is a specific parameters: 
* The gain can be changed by changing the values of resistors R7 and R5 (This arrangement has a gain of ~55). 

### Don't have Mindi?
You can download and install the [Mindi simulation tool](https://www.microchip.com/mplab/mplab-mindi),or use another SPICE simulator of your own preference. For use with different simulators, a plain spice model can be found in "Opamp_PIC18_Q41.txt" to replace the mindi-optimized "Opamp_PIC18_Q41.lb "