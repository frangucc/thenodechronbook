# Sensors

FROM
[https://www.element14.com/community/docs/DOC-82963/l/element14-essentials-sensors-ii](https://www.element14.com/community/docs/DOC-82963/l/element14-essentials-sensors-ii)


Refactor this text into our API.

**Merge this data from element14**

**Sensors I**

1. Introduction
Sensors are the interface between the physical world determined by the laws of physics (i.e., mass, acceleration, conductivity, force, magnetic fields, etc.) and the digital world, which interprets the information that sensors provide for use in a wide range of products - from embedded Internet of Things (IoT) devices to smart phones to even the common household toaster. Because there are so many types of sensors available today, it would be a challenge to discuss all of them in one learning module. Since electronic design engineers often work with very compact integrated circuits (IC), this learning module will focus on some of the essential IC sensors in use today.
2. Objective
The objective of this learning module is to provide you with the essential knowledge of IC sensors. You will first review the purpose of IC sensors and what physical conditions or stimuli they sense. In subsequent sections of this learning module, you will gain an understanding of how sensors are classified as well as their characteristics and the types of commonly used IC sensors.
Upon completion of this learning module, you will be able to:
 Define a sensor
 Explain the difference between a sensor and a transducer
 Identify the types of physical conditions or stimuli that are measured by sensors
 Explain how sensors are classified
 Discuss the characteristics of sensors
 Identify the types and applications of capacitive, inductive, electrical current, smoke detection, and temperature sensors
 Describe the requirements of a MEMS sensor
3. DefinitionBack to Top
What is a sensor? Or, what isn't a sensor? Let's begin this learning module with the definition of a sensor, which is sometimes confused with a similar term, transducer.
According to The Handbook of Modern Sensors: Physics, Designs and Applications, a sensor is defined as "a device that receives a stimulus and responds with an electrical signal."
Sensors are also called detectors, as well. But there is a slight difference between the terms and how they sense the physical world. Detectors sense information of a qualitative nature (i.e., presence of human movement), while a sensor measures physical stimuli quantitatively (i.e., ambient temperature in degrees Celsius). For the remainder of this learning module, we will use the terms "sensor" and "detector" as the same thing.
In some circles, the terms "sensor" and "transducer" are considered equivalent. But technically speaking, they are not. While it is true that a transducer receives a stimulus or a form of energy just like a sensor, a transducer's output is not an electrical signal; rather, the output of a transducer is another form of energy. In this context, a transducer is an energy converter.
A set of headphones is an example of a transducer since they convert an electrical signal into sound waves. A solar cell is also a transducer since it converts light energy into electrical energy. An electrical motor can be considered a transducer since it converts electrical energy (input voltage) into the mechanical energy (torque) needed to drive a rotating load (e.g., a centrifugal pump). But since it has a physical output, it is best characterized as an actuator.
What may cloud the meaning of the term sensor is a special category of sensor technology, the complex sensor. These sensors consist of various stages of sensing and transduction. For this learning module, we will define sensors and transducers as if they were simple sensors or transducers.

4. Classification Back to Top
There are many types of sensors, ranging from displacement, level, velocity, acceleration, pressure, flow, humidity, ionizing radiation, temperature and many more. The growth of smart phones and the IoT has spawned the development of many more types of sensors, especially the highly integrated, intelligent, low-power sensors. As suggested in the previous sections, there are both simple and complex sensors. Yet these antipodal classifications do not represent all the different ways of classifying sensors. Knowing the classification of sensors can save an engineer a lot of time when he or she is trying to select a sensor for a circuit design. So, here are the main sensor classifications:
Passive and Active
Passive and active sensors are common ways of classifying sensors according to how their output signal is generated. Passive sensors do not require an external source of energy to produce an output signal. The energy of the input stimulus is converted by the sensor into an output electrical signal. A thermocouple is an example of a passive sensor. Conversely, active sensors do require an external source of energy (commonly called the excitation signal) to generate an output signal. The active sensor uses the excitation signal and modifies it to produce an output signal. An example of an active sensor is a temperature-sensitive resistor or thermistor. The excitation signal is modified by the resistor relative to temperature; variations based upon resistance can then be measured.
Absolute and Relative
Absolute and relative sensors are also two common ways of classifying sensors. However, these sensors are classified according to what reference is used to generate the output signal. Absolute sensors sense a stimulus that is referenced against an absolute scale and is independent of conditions. For example, a thermistor's output is referenced against the Kelvin temperature scale. Conversely, a relative sensor generates an output signal that is referenced against a special type of reference. For example, some pressure sensors are relative sensors because they use atmospheric pressure (14.696 psi) as the reference for their output signal.
Digital and Analog
Analog sensors are a type of sensor that produces an output signal that is continuous and proportional to the measurand. Digital sensors produce an output signal that is binary (0 or 1) and use analog to digital (A/D) data conversion.
Other Classifications
There are other ways to classify sensors, but, for the most part, these are for special situations. These special situations can include:
 Characteristics
 Sensing material
 Applications
 Type of stimulus
5. The Physical Stimuli of Sensing Back to Top
Naturally, a sensor implies that "something" is sensed. So, let's now talk about what phenomena are sensed. Sensors are used to measure a variety of physical or material phenomena. These phenomena are sensed because they give us an objective "look" into the physical world, which is then converted into a form that embedded devices, computers and microcontrollers - the digital world - can understand and an engineer can employ in circuit designs.
The most common types of physical stimuli include acoustic, biological, chemical, electrical, magnetic, optical, thermal, radioactive, and mechanical. The following table summarizes the stimuli and the physical condition being sensed.
Stimulus
Sensed Physical Conditions
Acoustic	Wave amplitude, phase or polarization; spectrum; wave velocity
Electric	Charge, current, potential, voltage, electric field, conductivity, permittivity
Magnetic	Magnetic field, magnetic flux, permeability
Mechanical	Linear or angular position, acceleration, force stress, pressure, strain, mass, density, moment, torque, shape, roughness, orientation, stiffness, crystallinity, structural
Optical	Wave amplitude, phase or polarization; wave velocity; refractive index, emissivity, reflectivity, absorption
Thermal	Temperature, flux, specific heat, thermal conductivity
6. Sensor Characteristics Back to Top
We had previously mentioned that sensor characteristics are a special way of classifying sensors. If you need to select a sensor for a circuit design, the usual place to begin the selection process is reading the sensor specs or characteristics listed in a datasheet. While datasheets are always informative, most of them do not explain all their terms.
So, in this section, we will define the characteristics of sensors, explaining them well enough so you can make an informed decision regarding the sensors you use. (Note: Since this is an Essentials learning module, the mathematical derivations of these characteristics will not be discussed.) Here are the definitions of the main characteristics of a sensor:
 Accuracy: the maximum difference that exists between the actual value and the indicated value at the output of the sensor. The accuracy can be expressed either as a percentage of full scale or in absolute terms.
 Dead band: the insensitivity of a sensor over a particular range of input signals, where the output stays at a certain value (typically zero) over the dead band.
 Drift: the gradual degradation of the sensor and other components that can make the sensor's output signal slowly change independently of the measurand.
 Hysteresis: a deviation error of the sensor's output at a specified point of the input signal when it is approached from the opposite direction (e.g. low-to-high versus high-to-low). The typical causes for hysteresis are the design, friction and structural changes in the materials.
 Linearity: When a sensor output is directly proportional to its input over the entire range.
 Nonlinearity: a maximum deviation error of the real transfer function when compared to the approximation of straight line.
 Offset: a type of error that represents the difference between the real output value and the specified output value under a particular set of conditions.
 Precision: the degree of reproducibility of a sensor's measured output.
 Range: the minimum and maximum values of a measurable input.
 Repeatability: a reproducibility error that is caused by the inability of a sensor to represent the same value under presumably identical conditions. The possible sources of a repeatability errors can be thermal noise, build up charge, material plasticity, etc.
 Resolution: the smallest change that can be detected by a sensor, expressed as a proportion of the reading (or the full-scale reading) or in absolute terms.
 Response Time: the time for a sensor to approach its true output when a stepped input change has occurred.
 Saturation: when a sensor's output signal is no longer responsive to a specific level of an input stimulus. Saturation exhibits a span-end, non-linearity.
 Sensitivity: the minimum input of physical parameter that will create a detectable change in output.
 Stability: the ability of a sensor to maintain its output parameter constant over time. Changes in stability, also known as drift, can be due to components aging, decrease in sensitivity of components, and/or a change in the signal to noise ratio.
7. Types of IC SensorsBack to Top
IC sensors are the result of the new capabilities of large-scale, silicon processing that enables the inclusion of sensing and signal processing into a very compact, IC-sized package. As a result, electronics engineers now have a full palette of PCB-mountable sensors to employ in their circuit designs. IC sensors can sense a wide variety of physical conditions needed for the operation of consumer electronics devices, industrial control equipment, and embedded devices in IoT systems. The most commonly used IC sensors are grouped in the following categories:
 Capacitive
 Inductive
 Current
 Smoke Detection
 Temperature
- 7.1 Capacitive Sensors
Capacitive sensors are used detect and measure proximity, position or displacement, humidity, fluid level, acceleration and more. The ability of capacitive sensors to sense a wide range of materials makes capacitive sensing an ideal choice for many applications.
To understand how capacitance can be used as a sensing medium, let's review the definition of capacitance:
	C = Capacitance
ε = Permittivity of the Dielectric
A = Area of Plate Overlap
d = distance between plates
Capacitive sensors take advantage of the geometry of the flat capacitor, where capacitance as inversely proportional to the distance between the plates and directly proportional to the overlapping area of the plates. Thus, by changing the distance between the capacitor plates or the area of plate overlap, or causing variations in the dielectric material positioned between the plates, capacitance will be varied. This variable capacitance can then be used, along with a microcontroller and other signal conditioning circuitry, to produce an electrical output signal that's proportional to the change in capacitance as a result of the displacement.

The above scenario is realized in a popular application of capacitive sensing - touch sensing - used in tablets, smart phones and other types of touch pads. Capacitive touch sensing has become an alternative to traditional pushbutton switch, user interfaces because it requires no mechanical movement and it enables a completely sealed and modern-looking design.
A capacitive touch sensor is a copper sensor pad that's created on a printed circuit board that will have a parasitic capacitance to ground located elsewhere in the design. A covering plate is secured over the pad to create a touch surface.
Touching the covering plate over a pad creates an additional parallel capacitance essentially coupled to ground. This adds to the overall capacitance generated by the touch sensor used to detect a finger press.

The capacitance generated by the touch sensor is used in conjunction with a dual comparator with SR latch peripheral found on a Microchip PIC MCU along with external components to generate a relaxation oscillator. This configuration will generate an oscillation on the Q bar output of the SR latch. The frequency of oscillation will be determined by the capacitance, generated by the touch sensor and represented here by Cs. By itself, the capacitive touch sensor generates a particular frequency of oscillation.

The frequency of the oscillator is then measured in fixed intervals, using both Timer0 and Timer1 peripherals. Any shift due to a user's touch is detected and validated in software.
 

Microchip CAP1208-1-A4-TR 8-Channel Capacitive Touch Sensor, QFN
The Microchip CAP1208 is a multiple channel capacitive touch sensor used in Desktop and Notebook PCs, LCD Monitors, Consumer Electronics and Appliances.
It contains eight individual capacitive touch sensor inputs with programmable sensitivity for use in touch sensor applications. Each sensor input is calibrated to compensate for system parasitic capacitance and automatically recalibrated to compensate for gradual environmental changes.
The CAP1208 includes Multiple Pattern Touch recognition that allows the user to select a specific set of buttons to be touched simultaneously. It also has Active and Standby states, each with its own sensor input configuration controls.
Power consumption in the Standby state is dependent on the number of sensor inputs enabled as well as averaging, sampling time, and cycle time. Deep Sleep is the lowest power state available, drawing 5μA (typical) of current. In this state, no sensor inputs are active, and communications will wake the device.

Microchip CAP1298-1-A4-TR 8-Channel Capacitive Touch Sensor with Proximity Detection & Signal Guard, QFN
The Microchip CAP1298 is a multiple channel capacitive touch sensor used in computer, consumer electronics and appliances.
While similar to CAP1208, the CAP1298 can also be configured to detect proximity on one or more channels with an optional signal guard to reduce noise sensitivity and to isolate the proximity antenna from nearby conductive surfaces that would otherwise attenuate the e-field.
The CAP1298 also has Active and Standby states, each with its own sensor input configuration controls. The Combo state allows a combination of sensor input controls to be used which enables one or more sensor inputs to operate as buttons while another sensor input is operating as a proximity detector.

Microchip  MTCH102-I/MS 8-Channel Proximity/Touch Controller MSOP
The Microchip MTCH102 provides an easy way to add proximity or touch detection to any application with human machine interface.
It can integrate up to two, five and eight capacitive touch/proximity detection sensors which can work through plastic, wood or even metal front panels with Microchip's proprietary Metal over Capacitive technology. It also supports a wide range of conductive materials as sensors, like copper pad on PCB, silver ink, PEDOT or carbon printing on plastic film, Indium Tin Oxide (ITO) pad, wire/cable, etc.
The MTCH102 uses a sophisticated scan optimization algorithm to actively attenuate noise from the signal. The sensitivity adjustment and flexible power mode allow users to easily configure the device at run-time. An active-low output will communicate the state of the sensors to a host/master MCU or drive an indication LED.

Microchip  MTCH101-I/OT Single-Channel Proximity Detector SOT-23
The Microchip MTCH101 provides an easy way to add proximity or touch detection to any human interface application.
The device integrates a single-channel capacitive proximity detection, which can work through plastic, glass or wood-front panel. It also supports a wide range of conductive materials as sensor, like copper pad on PCB, silver or carbon printing on plastic, Indium Tin Oxide (ITO) pad, wire/cable, etc. On-board adjustable sensitivity and power mode selection allow the user to configure the device at run time easily. An active-low output will communicate the state of the sensor to a host/master MCU, or drive an indication LED.
- 7.2 Inductive Sensors
Inductive sensors are a type of displacement sensor used to sense changes in position, distance and proximity. One of the advantages of inductive sensing is that non-magnetic materials (e.g., stainless steel, brass, plastics, woods, and others) can be penetrated by a magnetic field without any loss of positional accuracy. Another differentiating advantage of inductive sensors is that they can work in severe environments where capacitive sensors cannot.
Inductive touch sensors are a common replacement for electromechanical pushbutton switches in severe or outdoor environments. An inductive touch system uses the magnetic coupling between a solid metal target and an inductive sensing coil. The target is a passive, electrically conductive layer that is arranged to displace or deform along the measurement axis relative to the coil. The sensor coils are one or more inductors, implemented as flat spiral coils, etched into the copper layer of a PCB. The inductance of the coil is determined by the number of turns and the dimensions of the pattern etched into the PCB.
If a user presses on the front panel, then the coupling between the target and sense coil will change due to the minute shift in the target's position. When the user presses the front panel, it deflects slightly. This deflection, on the order of microns, is inductively detected.

Side View - Inductive Touch Sensor

Top View - Spiral Coil
The fundamental principle of operation of inductive touch technology is that the inductance of an inductor varies when a nearby magnetically permeable or electrically conductive material moves relative to the inductor. This is because the magnetically permeable or electrically conductive material provides an alternative route for the magnetic flux which, in turn, varies the inductance. The closer the material is to the inductor, the greater the effect. The coil's inductance decreases as the target approaches and, to a limit, vice versa.

Microchip  MCP2036-I/SL Inductive Sensor Analog Front End Device SOIC
The Microchip MCP2036 Inductive Sensor Analog Front End (AFE) combines all the necessary analog functions for a complete inductance measurement system. The MCP2036 measures a sensor coil's impedance by exciting the coil with a pulsed DC current and measuring the amplitude of the resulting AC voltage waveform. The drive current is generated by the on-chip current amplifier/driver which takes the high-frequency triangular waveform present on the DRVIN input, and amplifies it into the pulsed DC current for exciting the series combination of the sensor coils. The AC voltages generated across the coils, are then capacitively coupled into the LBTN and LREF inputs. An input resistance of 2K between the inputs and the virtual ground offsets the AC input voltages up to the signal ground generated by the reference voltage generator.
- 7.3 Current Sensors
Current sensors detect electrical circuit path current and convert it to an output voltage, which is proportional to the current through the measured path. There are a wide variety of current sensors, with each type rated for a specific current range and environmental condition. Many power and control applications benefit from current sensing, including battery life indicators and chargers, current and voltage regulators, DC/DC converters, ground fault detectors, linear and switch-mode power supplies, automotive power electronics and motor speed controls.
Current Sensing Resistors
Current sensing resistors are the most commonly used way to sense current. They can be considered a current-to-voltage converter, where inserting a resistor into the current path, the current is converted to voltage in a linear way of V = I x R. The main advantages and disadvantages of current sensing resistors include:
Advantages	Disadvantages
 Low cost
 High measurement accuracy
 Measurable current range from very low to medium
 Capability to measure DC or AC current
 Introduces additional resistance into the measured circuit path, which may increase source output resistance and result in undesirable loading effect.
 Power loss since current sensing resistors dissipate power (P=I² x R). Therefore, current sensing resistors are rarely used beyond the low and medium current sensing applications.
The disadvantages can be somewhat overcome by using low-value sensing resistors. However, the voltage drop across the sensing resistor may become low enough to be comparable to the input offset voltage of subsequent analog conditioning circuit, which would compromise the measurement accuracy.
In addition, if the measured current has a large high-frequency component, the current sensing resistor's inherent inductance must be low. Otherwise, the inductance can induce an Electromotive Force (EMF) which will degrade the measurement accuracy as well. Furthermore, the resistance tolerance, temperature coefficient, thermal EMF, temperature rating and power rating are also important parameters of current sensing resistors when measurement accuracy is required.
Current Sensing Techniques
Low-side and high-side current sensing are two common techniques for sensing for circuit current. Low-side current sensing connects the sensing resistor between the load and ground, while high-side current sensing connects the sensing resistor between the power supply and load.

A) Low-side sensing is advantageous because common-mode voltage is near ground potential, providing for the use of single-supply, rail-to-rail input/output op amps. Normally, the sensed voltage signal (VSEN = ISEN x RSEN) is so small that it needs to be amplified by subsequent op amp circuits (e.g., non-inverting amplifier) to get the measurable output voltage (VOUT).
Advantages	Disadvantages
 Low input Common mode voltage
 Low VDD components
 Ground referenced input and output
 Simplicity and low cost
 Ground path disturbance
 Load is lifted from system ground since RSEN adds undesirable resistance to the ground path
 High load current caused by accidental short goes undetected
 

B) High-side current sensing connects the sensing resistor between the power supply and load. The sensed voltage signal is amplified by subsequent op amp circuits to get the measurable VOUT. High-side current sensing is typically selected in applications where ground disturbance cannot be tolerated, and short circuit detection is required, such as motor monitoring and control, overcurrent protection and supervising circuits, automotive safety systems, and battery current monitoring.
Advantages	Disadvantages
 Eliminates ground disturbance
 Load connects system ground directly
 Detects the high load current caused by accidental shorts
 Must be able to handle very high and dynamic Common mode input voltages
 Complexity and higher costs
 High VDD parts
 

Microchip  EMC1701-2-AIZL-TR High-Side Current-Sense and Internal 1°C Temperature Monitor MSOP
The Microchip EMC1701 is a combination high-side current sensing device with precision temperature measurement for Notebook and Desktop Computers, Industrial Equipment, Power Management Systems and Embedded Applications.
It measures the voltage developed across an external sense resistor to represent the high-side current of a battery or voltage regulator. The EMC1701 also measures the source voltage and uses these measured values to present a proportional power calculation.
The EMC1701 contains additional bi-directional peak detection circuitry to flag instantaneous current spikes with programmable time duration and magnitude threshold.
Finally, the EMC1701 includes an internal diode channel for ambient temperature measurement. Both current sensing and temperature monitoring include two tiers of protection: one that can be masked and causes the ALERT pin to be asserted, and the other that cannot be masked and causes the THERM pin to be asserted.

Microchip  PAC1710-1-AIA-TR Single High-Side Current Sense Monitor with Power Calculation DFN
The Microchip PAC1710 is a high-side bi-directional current sensing monitor with precision voltage measurement capabilities. The power monitor measures the voltage developed across an external sense resistor to represent the high-side current of a battery or voltage regulator. The PAC1710 also measures the SENSE+ pin voltage and calculates average power over the integration period.
The PAC1710 can be programmed to assert the ALERT pin when high and low limits are exceeded for Current Sense and Bus Voltage. Available in a RoHS compliant 3 X 3mm 10-pin DFN package.
- 7.4 Smoke Detection Sensors
Smoke detection sensors are used in both residential and commercial alarms throughout the world. They come in two forms: photoelectric and ionization. Photoelectric smoke detectors use a light source to detect smoke, while ionization smoke detectors use a radioisotope to ionize air. Performance-wise, photoelectric smoke detectors respond faster to a fire in its early stage because the detectors are more sensitive to the large combustion particles that emanate during slow, smoldering fires. Conversely, ionization smoke alarms respond faster to fast flaming fires because they can detect small amounts of smoke produced by fast flaming fires, such as cooking fires or fires fueled by paper or flammable liquids.

Microchip  RE46C141S16F CMOS Photoelectric Smoke Detector ASIC with Interconnect SOIC
The Microchip RE46C141 is low power CMOS photoelectric type smoke detector IC. With minimal external components this circuit will provide all the required features for a photoelectric type smoke detector.
The design incorporates a gain selectable photo amplifier for use with an infrared emitter/detector pair. An internal oscillator strobes power to the smoke detection circuitry for 100µs every 8.1 seconds to keep standby current to a minimum. If smoke is sensed the detection rate is increased to verify an alarm condition. A high gain mode is available for push button chamber testing. A check for a low battery condition and chamber integrity is performed every 32 seconds when in standby. The temporal horn pattern supports the NFPA 72 emergency evacuation signal. An interconnect pin allows multiple detectors to be connected such that when one units alarms, all units will sound.
The RE46C141 is recognized by Underwriters Laboratories for use in smoke detectors that comply with specification UL217 and UL268.

Microchip  RE46C166S16F CMOS Photoelectric Smoke Detector ASIC with Interconnect Timer Mode and Alarm Memory SOIC
The Microchip RE46C166 device is low-power, CMOS photoelectric type, smoke detector ICs.
Each design incorporates a gain selectable photo amplifier for use with an infrared emitter/detector pair. An internal oscillator strobes power to the smoke detection circuitry for 100 μs every 10 seconds to keep standby current to a minimum. If smoke is sensed, the detection rate is increased to verify an alarm condition.
A high gain mode is available for push button chamber testing. A check for a low battery condition and chamber integrity is performed every 43 seconds when in standby. The temporal horn pattern supports the NFPA 72 emergency evacuation signal. An interconnect pin allows multiple detectors to be connected so when one unit alarms, all units will sound. A charge dump feature will quickly discharge the interconnect line when exiting a local alarm. The interconnect input is also digitally filtered. An internal timer allows for single button, push-to-test to be used for a reduced sensitivity mode. An alarm memory feature allows the user to determine if the unit has previously entered a local alarm condition. The RE46C166 was designed for use in smoke detectors that comply with Underwriters Laboratory Specification UL217 and UL268.

Microchip  RE46C180E16F CMOS Programmable Ionization Smoke Detector ASIC with Interconnect Timer Mode and Alarm Memory DIP
The Microchip RE46C180 is a low power, CMOS ionization-type, smoke detector IC. With minimal external components, this circuit will provide all the required features for an ionization-type smoke detector.
An on-chip oscillator strobes power to the smoke detection circuitry for 5 ms every 10 seconds to keep the standby current to a minimum. A check for a Low Battery condition is performed every 80s and an ionization chamber test is performed once every 320s when in Standby. The temporal horn pattern complies with the National Fire Protection Association NFPA 72® National Fire Alarm and Signaling Code® for emergency evacuation signals.
An interconnect pin allows multiple detectors to be connected, such that when one unit alarms, all units will sound. A charge dump feature quickly discharges the interconnect line when exiting a Local Alarm condition. The interconnect input is also digitally filtered. An internal 9 minute or 80s timer can be used for a Reduced Sensitivity mode. An alarm memory feature allows the user to determine whether the unit has previously entered a Local Alarm condition.
The RE46C180 is designed for use in smoke detectors that comply with the Standard for Single and Multiple Station Smoke Alarms, UL217 and the Standard for Smoke Detectors for Fire Alarm Systems, UL268.

Microchip  RE46C190S16F CMOS Low Voltage Photoelect ric Smoke Detector ASIC with Interconnect and Timer Mode SOIC
The Microchip RE46C190 is a low power, low voltage CMOS photoelectric type smoke detector IC. The design incorporates a gain-selectable photo amplifier for use with an infrared emitter/detector pair.
An internal oscillator strobes power to the smoke detection circuitry every 10 seconds, to keep the standby current to a minimum. If smoke is sensed, the detection rate is increased to verify an Alarm condition.
A high gain mode is available for push button chamber testing. A check for a low battery condition is performed every 86 seconds, and chamber integrity is tested once every 43 seconds, when in Standby. The temporal horn pattern supports the NFPA 72 emergency evacuation signal. An interconnect pin allows multiple detectors to be connected such that, when one unit alarms, all units will sound. An internal 9 minute timer can be used for a Reduced Sensitivity mode. The RE46C190 was designed for use in smoke detectors that comply with Underwriters Laboratory Specification UL217 and UL268.
- 7.5 Temperature Sensors
Temperature sensing is a fundamental function of control systems in many types of appliances, handheld devices, industrial equipment, as well as others. There are a number of passive and active temperature sensors that can be used to measure system temperature, including thermocouples, resistive temperature detectors (RTDs), thermistors and silicon temperature sensors. These sensors provide temperature feedback to a system controller that oversees control functions such as over-temperature shutdown, turn-on/off cooling fan, temperature compensation, or as a general purpose temperature monitor.

Microchip MCP9701AT-E/TT Low-Power Linear Active Thermistor™ IC, SOT-23
The Microchip MCP9701/9701A is a Linear Active Thermistor Integrated Circuit (IC) converts temperature to analog voltage.
This low-power sensor features an accuracy of ±2°C from 0°C to +70°C (MCP9701A) and ±4°C from 0°C to +70°C (MCP9701) while consuming only 6 μA (typical) of operating current.
Unlike resistive sensors, e.g., thermistors, the Linear Active Thermistor IC does not require an additional signal-conditioning circuit. Therefore, the biasing circuit development overhead for thermistor solutions can be avoided by implementing a sensor from these low-cost devices. The Voltage Output pin (VOUT) can be directly connected to the ADC input of a microcontroller. The MCP9701/9701A temperature coefficients are scaled to provide a 1°C/bit resolution for an 8-bit ADC with a reference voltage of 2.5V and 5V, respectively.
The MCP9701/9701A provide a low-cost solution for applications that require measurement of a relative change of temperature. When measuring relative change in temperature from +25°C, an accuracy of ±1°C (typical) can be realized from 0°C to +70°C. This accuracy can also be achieved by applying system calibration at +25°C. In addition, this family of devices is immune to the effects of parasitic capacitance and can drive large capacitive loads.
This provides printed circuit board (PCB) layout design flexibility by enabling the device to be remotely located from the microcontroller. Adding some capacitance at the output also helps the output transient response by reducing overshoots or undershoots. However, capacitive load is not required for the stability of sensor output.

Microchip TC77-3.3MCTTR Digital Thermal Sensor with SPI™ Interface, SOT-23
The Microchip TC77 is a serially accessible digital temperature sensor particularly suited for low cost and small form-factor applications.
Temperature data is converted from the internal thermal sensing element and made available at anytime as a 13-bit two's compliment digital word. Communication with the TC77 is accomplished via a SPI and MICROWIRE compatible interface. It has a 12-bit plus sign temperature resolution of 0.0625°C per Least Significant Bit (LSb). The TC77 offers a tem- perature accuracy of ±1.0°C (max.) over the temperature range of +25°C to +65°C. When operating, the TC77 consumes only 250 μA (typ.).
The TC77's Configuration register can be used to activate the low power Shutdown mode, which has a current consumption of only 0.1 μA (typ.). Small size, low cost and ease of use make the TC77 an ideal choice for implementing thermal management in a variety of systems.

Microchip  TC622CPA Low Cost Single Trip Point Temperature Sensor DIP
The TC622 is a single point, programmable solid-state temperature sensors designed to replace mechanical switches in sensing and control applications. Both devices integrate the temperature sensor with a voltage reference and all required detector circuitry. The desired temperature set point is set by the user with a single external resistor. Ambient temperature is sensed and compared to the programmed set point. The OUT and OUT outputs are driven to their active state when the measured temperature exceeds the programmed set point. The TC622 has a power supply voltage range of 4.5V to 18.0V while the TC624 operates over a power supply range of 2.7V to 4.5V. It has a usable temperature range of -40°C to +125°C (TC622VXX). The device features low supply current making it suitable for portable applications. Eight-pin through-hole and surface mount packages are available. The TC622 is also offered in a 5-pin TO-220 package.

Microchip  TC74A0-5.0VAT Tiny Serial Digital Thermal Sensor TO-220
The Microchip TC74 is a serially accessible, digital temperature sensor particularly suited for low cost and small form-factor applications. Temperature data is converted from the onboard thermal sensing element and made available as an 8-bit digital word. Communication with the TC74 is accomplished via a 2-wire SMBus/I2C compatible serial port. This bus also can be used to implement multi-drop/multi-zone monitoring. The SHDN bit in the CONFIG register can be used to activate the low power Standby mode. Temperature resolution is 1°C. Conversion rate is a nominal 8 samples/sec. During normal operation, the quiescent current is 200 μA (typ). During standby operation, the quiescent current is 5 μA (typ). Small size, low installed cost and ease of use make the TC74 an ideal choice for implementing thermal management in a variety of systems.

Microchip MCP98244T-BE/MNY DDR4 DIMM Temperature Sensor with EEPROM for SPD, TDFN
The Microchip MCP98244 digital temperature sensor converts temperature from -40°C and +125°C to a digital word.
This sensor meets JEDEC Specification JC42.4-TSE3000B1 Memory Module Thermal Sensor Component. It provides an accuracy of ±0.2°C/±1°C (typical/maximum) from +75°C to +95°C with an operating voltage of 1.7V to 3.6V. In addition, MCP98244 has an integrated EEPROM with two banks of 256 by 8 bit EEPROM (4k Bit) which can be used to store memory module details and vendor information.
The MCP98244 digital temperature sensor comes with user-programmable registers that provide flexibility for DIMM temperature-sensing applications. The registers allow user-selectable settings such as Shutdown or Low-Power modes and the specification of temperature Event boundaries. When the temperature changes beyond the specified Event boundary limits, the MCP98244 outputs an Alert signal at the Event pin. The user has the option of setting the temperature Event output signal polarity as either an active-low or active-high comparator output for thermostat operation, or as a temperature Event interrupt output for microprocessor-based systems.
The MCP98244 EEPROM is designed specifically for DRAM DIMMs (Dual In-line Memory Modules) Serial Presence Detect (SPD). It has four 128 Byte pages, which can be Software Write Protected individually. This allows DRAM vendor and product information to be stored and write-protected. This sensor has an industry standard I2C Fast Mode Plus compatible 1 MHz serial interface.

Microchip  MCP9904T-2E/9Q Multi-Channel Low-Temperature Remote Diode Sensor VDFN
The Microchip MCP9904 is a high-accuracy, low-cost, System Management Bus (SMBus) temperature sensor. The MCP9904 monitors up to four temperature channels. Advanced features such as Resistance Error Correction (REC), Beta Compensation (to support CPU diodes requiring the BJT/transistor model including 45 nm, 65 nm and 90 nm processors) and automatic diode-type detection combine to provide a robust solution for complex environmental monitoring applications.
Resistance Error Correction automatically eliminates the temperature error caused by series resistance allowing greater flexibility in routing thermal diodes. Beta Compensation eliminates temperature errors caused by low, variable beta transistors common in today's fine geometry processors. The automatic beta detection feature monitors the external diode/transistor and determines the optimum sensor settings for accurate temperature measurements regardless of processor technology. This frees the user from providing unique sensor configurations for each temperature monitoring application.
These advanced features plus ±1°C measurement accuracy for both external and internal diode temperatures provide a low-cost, highly flexible and accurate solution for critical temperature monitoring applications.
- 7.6 Micro-Electro-Mechanical Systems (MEMS) Sensors
The ability to microengineer and micromachine components with dimensions on the order of micrometers has brought forth the development of MEMS technology. MEMS is a micro-electro-mechanical system consisting of microcomponents of mechanical and electrical devices that enable the manufacturing of microsensors and actuators in combination with control and signal conditioning circuitry. MEMS are appearing in monitoring and control of applications ranging from biomedicine to IoT embedded systems to smart phones to automated manufacturing.

Microchip  MM7150-AB0 MEMS Module Tri-Axis Gyroscope Tri-Axis Accelerometer Tri-Axis Magnetometer 2g Module
The Microchip MM7150 Motion Module is a simple, cost-effective solution for integrating motion and positioning data into a wide range of applications.
The module contains the SSC7150 motion coprocessor with integrated 9-axis sensor fusion as well as high performance MEMS technology including a 3-axis accelerometer, gyroscope and magnetometer. All components are integrated, calibrated and available on the module for PCB mounting.

**Sensors II
**
Prototyping (basic selection - components, breadboards, veroboard, wires, beginner projects, etc) (11%)

PCBs (circuit boards, etching, printing, patterning, plating, assembly, laminates, substrates, etc) (7%)

Motors (types, drivers, phases, servos, controllers, power, steppers, gears, etc) (8%)

Microcontrollers (single board computers, embedded devices, system-on-a-chip, PICs, EPROMs, etc) (20%)

Sensors (motion, MEMs, environmental, force/pressure, audio/visual, touch, bio, chemical, etc) (11%)

Transistors (switches, amplifiers, tubes, NPN/PNP, FETs & MOSFETs, Darlington pairs, Scottkys, etc) (11%)

Soldering and or Other Tools (soldering irons, soldering stations, solder, solder paste, flow soldering, etc) (4%)

Test & Measurement (meters, probes, scopes, analysers, generators, counters, etc) (11%)

Power (bench tops, uninterruptible, circuit protection, fuses, high voltage, switch-mode, current limiting, AC/DC, etc) (6%)

Industrial Control (panels, interfaces, controls, sensors, diagnostics) (3%)


Robotics (essential parts, applications, software, sample projects) (7%)

**Sensors [consider 5th section]**

**1. Introduction**
Perhaps ever since the introduction of the Dick Tracy Two-Way Wrist Radio many decades ago, the fascination with and utility of wearable devices has steadily increased (1). But today's wearables are a far cry from the creative inventions of Hollywood copywriters from an age gone by. IoT wearable devices today are powerful tools that can sense, process, store, and communicate significant information. The great leap forward in wearable devices is not only the result of its innovative technology, but also the applications they now can provide such as patient monitoring, wellness/sports/fitness, entertainment, and other forms of computing. But all wearable devices today have one thing in common: they all use sensors. And there are all kinds of IoT wearable device sensors available today, including temperature, UV, proximity, heart rate, motion and many others. This learning module is an introduction to some of the common types of sensors used in IoT wearable devices today.
(1) Of course, this statement is the subjective inclination of the author of this learning module. Perhaps the reader may find his/her fascination with wearable devices from The Jetsons' Promotional Wrist Watch or the Star Trek Communicator or some other très chic device. If you are so inclined to evangelize about your preferred technological inspiration, please leave your comments below.
**
2. Objective**
The objective of this learning module is to provide you with basic knowledge of sensors used in IoT wearable devices. You will first review some of the main concepts of sensor technology and then get an overview of the approaches to human body sensing. In the last section, you will learn about the main types and characteristics of sensors for wearable IoT devices.
Upon completion of this learning module, you will be able to:

 Review sensor essentials covered in Sensors I
 
 Discuss how the human body is sensed
 
 Describe how photoplethysmographic technology is used in IoT wearable devices
 List the main types of types of sensors for wearable IoT devices
 Explain the features of the most common wearable device sensors
 
**3. ReviewBack to Top**
In the first Essentials Sensors learning module, the definition of a sensor was presented, as well as the classifications and characteristics of IC sensors. Let's revisit some of the important terms from Sensors I that are applicable to this learning module:

 Definition: According to The Handbook of Modern Sensors: Physics, Designs and Applications, a sensor is defined as "a device that receives a stimulus and responds with an electrical signal."
 
 Categories: There are two main categories of sensors: simple and complex. Simplex sensors typically have a sensing function only, while complex sensors can have both transduction and sensing functions due to the integration of signal conditioning, A-to-D conversion and other circuitry within the sensor's integrated circuit package.
 
 Classifications: Sensors can be classified in a variety of ways. Passive/Active, Absolute/Relative and Digital/Analog are the most common classifications. There are also other ways to classify sensors, but, for the most part, these are for special situations. These special situations include: characteristics, material, applications, and type of stimulus.
 
 Characteristics: Sensor characteristics describe the capabilities and parameters of specific sensors. The common characteristics include: Accuracy, Dead band, Drift, Hysteresis, Linearity, Nonlinearity, Offset, Precision, Range, Repeatability, Resolution, Response Time, Saturation, Sensitivity, and Stability. Sensor characteristics are normally found in a datasheet, user guide or other documentation. These documents provide specific information that's essential to understanding not only how to select a sensor, but also on how to use it in a specific application.

4. Approaches to Human Body Sensing Back to Top
While there are many types of physical conditions that IoT devices are capable of sensing – acoustic, electric, magnetic, mechanical, optical and thermal – wearable devices primarily sense biological (or biochemical) conditions and the body's movement. Gaining an understanding of these conditions with respect to human body sensing is a necessary prerequisite to understand the applications of sensors in IoT wearable devices.
To begin, the physical condition of the human body can be sensed in three different ways: the skin, body fluids and movement. Let's discover in this section of the learning module how these components can be used in a wearable device sensing design.
- 4.1 The Skin
While we may discount the importance of the human skin (excluding perhaps a nice tan at your favorite beach in the summer) or even forget that the skin itself is a body organ, the fact is that the skin is a superb “natural” sensor. It senses both internal and external conditions. And it responds to heat, cold, fear, pressure, pleasure and pain. As a medium for determining the overall condition of the human body, the skin can be leveraged to gather data on body temperature, blood pressure, heart rate,  peripheral capillary oxygen saturation (SpO2) and more.
- 4.2 Body Fluids
Body fluids also tell us a lot about the condition of the human body. Blood has long been used as a medium for sensing the body's medical condition; however, it requires an invasive sensing technique that is not always desirable to use. Therefore, a lot of new and non-invasive techniques are being developed utilizing sweat, tears, saliva and interstitial fluids. In general, body fluids can be used by wearable device sensors because they contain a lot of chemical and biochemical information about the state of the body's functions. What follows is an overview of the information body fluids can provide:
 Sweat contains a lot of biological substances such as sodium, chloride, potassium, calcium, ammonia, glucose, and lactate. For fitness activities, sweat can tell a lot about the body's hydration level and electrolyte balance. Since it is readily accessible by a wearable device, it is the easiest fluid to leverage as a source of information about the condition of the body.
 Saliva contains an incredible amount of biological information. It includes ions of sodium, potassium, chloride bicarbonate, nitrates, urea, uric acid, creatinine, and hundreds of types of proteins. The downside of saliva as a sensing stimulus is that it also possesses, in varying degrees, mucus, food debris and blood, all of which can impede the operation of a sensor.
 Tears are another body fluid that can be used by a wearable device to sense the condition of the body. They contain proteins, electrolytes and sugars like glucose that can be leveraged in diabetes monitoring.
 Interstitial fluids – fluids that surround tissue cells – contain sugars, salts, fatty acids, amino acids, coenzymes, hormones, and more. These fluids tell a lot about the condition of the body and would be typically used in wearable medical devices such as diabetes monitors.
- 4.3 Body Movement
The movement of the body can be utilized in monitoring the motor activities of a human being. The human body's motor activities are useful in patient monitoring, especially for movement disorders such as Parkinson's Disease or diseases related to Parkinson's such as bradykinesia. Motion sensors such as accelerometers, gyroscopes or magnetometers can be placed in wearable devices or in garments to obtain movement data.
5. Introduction to Photoplethysmographic Technology Back to Top
For many years, heart rate monitoring has been recognized as a useful parameter in both diagnosing diseases (e.g., autonomous neuropathy, cardiac arrhythmia or infarction, etc.) as well as in optimizing the physical regimen of an athlete. In general, heart rate monitoring has been accomplished using a variety of technologies, with the most common ones, being:
 Bio-potential (electrocardiography - EKG)
 Electric acoustic (phonocardiography)
 Ultrasonic (echocardiography)
 Bio-electrical (impedance cardiography)
Despite the above time-tested technologies, photoplethysmographic technology (PPG) has found new interest by researchers and designers in the area of heart rate monitoring because of it offers a compact, low cost, simple and low power technology that's a good fit for the growing wearable market of fitness and medical devices.
In its most basic form, PPG technology utilizes an LED and photo-detector as well as associated circuitry to make up a pulse oximeter, which offers a way to determine the heart rate by assessing the arterial pulsability of tiny networks of blood vessels in the tissue of the skin. As an optical sensor, PPG illuminates living tissues with a light source, gathers a portion of the light that propagates through the tissue, and then analyzes the resulting attenuated light. LEDs are typically used as the light source and detector for PPG-based heart rate monitors.
One of the challenges of using PPG technology in this application is that in some areas of the body (e.g., forehead, ankle, and torso) the emitted light is fully absorbed by the body. In these cases, the PPG optical sensor can be operated in an alternative “reflectance” mode where the light source is placed next to the detector to collect the propagated light by means of the light scattering effect. The reflectance mode allows the PPG-based heart rate monitor to be used on many different parts of the body such as the wrist, forearm and ankle – all ideal for use in wearable devices such as smart watches, and fitness or arm bands.
6. Types of Sensors Back to Top
Since the field of wearable IoT devices is expanding so rapidly, it would be difficult to cover every type of sensor that IoT wearable devices would utilize. Electronic textiles, micro needle arrays, wearable colorimetric sensors, body-conformable electronics, one-time/re-usable sensors, invasive/non-invasive sensors, and implantable devices are all part of this exciting yet burgeoning field of technology. Since this is an essentials learning module, we will only focus on the most common types of wearable sensors that feature the following characteristics: low-power, lightweight, compact form factor, and multi-functional.

Silicon Labs Si114x Multi-LED Heart Rate, SpO2, Proximity and Ambient Light
Wearable devices, such as smart watches or activity-tracking wrist and arm bands, typically have more stringent requirements than handheld or other portable devices. They are smaller and must be comfortable to wear, and they need to be lightweight and low-power. To meet these requirements, manufacturers will produce multi-functional, highly integrated sensors. To illustrate this sensor design approach, the Silicon Labs' Si114x Series sensors combine digital UV index sensing with ambient light and blood oximetry sensing on a single chip. This sensor is designed to track UV sun exposure, heart rate, blood oximetry and proximity/gesture control.

Packaged on a tiny 2 mm x 2 mm clear QFN package, the monolithic Si114x sensors integrate multiple photodiodes, an analog-to-digital converter, a signal processor, up to 3-LED drivers and a digital I2C control interface. This low-power sensing family enables long battery life with standby less than 500 nA and an average power of as little as 1.2 uA with once per second real-time UV Index measurements. Capable of controlling one, two and three-LED systems, the sensors enable developers to implement proximity detection with a range over 50 cm, multi-dimensional systems capable of advanced 2D/3D motion sensing, heart rate/pulse oximetry measurements, or cheek detection. The Si114x sensors' LED drivers enable implementation of reflective heart rate and blood oximetry measurement capabilities for health and fitness trackers, as well as touchless interfaces that support end-user control from a distance. Different models in the Si114x family offer advanced motion and gesture sensing.

Si1132 Ultraviolet (UV) Index and Ambient Light Sensor
UV sensing in wearable devices has seen an increase in demand in recent years. UV tracking is helpful for those with an elevated risk for sunburn or for people who have concerns about excessive sun exposure. But conventional UV sensors require UV-sensitive photodiodes along with an external microcontroller (MCU), analog-to-digital converter (ADC) and signal processing firmware. Lacking a high level of integration gives them a larger footprint and places some limits on their use in compact wearable IoT devices.

A good example of how the problem of conventional UV sensors is solved is with the Si1132 UV index and ambient light sensor IC. It's a monolithic sensor that integrates multiple photodiodes, an analog-to-digital converter, a signal processor and a digital I2C control interface in a small 2 mm x 2 mm clear QFN package.
(Note: Standardized by the World Health Organization (WHO), the digital UV index is linearly related to the intensity of sunlight and is weighted according to the Erythemal Action Spectrum developed by the International Commission on Illumination (CIE). This weighting provides a standardized measure of our skin's response to different sunlight wavelengths including UVB and UVA.)

Silicon Labs Si705x Digital Temperature Sensor IC
Temperature sensing is the most commonly measured parameter for monitoring the condition of a human body. Low body temperature can be an indication of hypothermia, but it can also be a symptom of infection, kidney/liver failures, shock, stress and others. On the other hand, high body temperatures can indicate a fever (hyperthermia) accompanying the flu, or can indicate the more harmful heat stroke.

The Silicon Labs' ultra-low-power, high-precision Si705x digital temperature sensor offers accurate temperature sensing in a lightweight and compact form factor that's ideal for wearable and other portable devices. It consumes only 195 nA when sampled once per second, which minimizes self-heating and enables multi-year coin cell battery operation.
Traditional approaches to temperature sensing, using thermistors or embedded MCU temperature sensors, often lack accuracy and possess higher power consumption. Although improved accuracy can be achieved through end-of-line calibration, this technique presents additional manufacturing costs; the sensor's accuracy can still be susceptible to variations in power supply voltage. In contrast, the Si705x sensors' signal processing technology provides stable temperature accuracy over the entire operating voltage and temperature ranges without the need for costly end-of-line production calibration. The Si705x Series sensor maintains its accuracy across the full operating temperature and voltage ranges and has four different accuracy levels up to +/-0.3 °C. Available in a compact 3 mm x 3 mm DFN package, the Si705x  Series sensors feature an industry-standard I2C interface for easy configuration. With a low 1.9 V minimum power supply voltage, it can be connected directly to a battery without the need for an external voltage regulator. It also provides up to 14-bit temperature resolution for high-precision measurement.

Si7005 Relative Humidity and Temperature Sensors
Typical approaches to relative humidity (RH) sensing use discrete resistive and capacitive sensors, hybrids and multi-chip modules (MCMs). These approaches suffer from high bill of materials (BOM) costs, high component counts, large footprints, and the need for labor-intensive calibrations. Silicon Labs solves the problems of conventional RH sensors with its Si7005 digital relative humidity and temperature sensor. It uses low-K polymeric dielectrics for sensing humidity, which enables the construction of a low-power, monolithic CMOS sensor IC with low drift and hysteresis, and excellent long term stability.

Temperature is sensed by a precision band gap referenced circuit on the die. Humidity is sensed by measuring the capacitance change of low-k dielectric layer applied to the surface of the die. Both temperature and humidity are precisely measured in very close proximity on the same monolithic device, providing exceptional measurement accuracy. The Si7005 device consumes only 2 µA on average at one measurement per minute. It integrates sensing elements, an analog-to-digital converter (ADC), signal processing, non-volatile memory for calibration data and an I2C interface in a monolithic CMOS IC. This high level of single-chip integration makes the sensor rugged and reliable, reduces cost and development time, and simplifies board design.

Silicon Labs  CPT112S-A01-GM Capacitive Touch Sensor Controller
It is easy to add capacitive touch to wearable or other portable devices with the Silicon Labs' CPT112S TouchXpress Capacitive Touch Sensor Controller. It supports up to 12 capacitive sensor inputs in a 3 mm x 3 mm QFN package. The I2C interface provides an easy way to track the status of touch sensors, and an interrupt pin can wake the host processor from sleep after a proximity touch detection. The device also comes with advanced features like moisture immunity, wake-on proximity, and buzzer feedback for an enhanced user experience. No firmware development is needed, and all the capacitive touch sense parameters can be configured using a simple GUI-based configurator.

7. Sensor Evaluation BoardsBack to Top
Sensor evaluation boards make it easy to learn, test, and develop sensor applications. Here are some of the currently available sensor evaluation boards for the sensors described in this learning module:

Environmental and Biometric Sensor Puck with Bluetooth Low Energy and iOS/Android App
The SENSOR-PUCK is a demo platform for the Silicon Labs' Si114x Series Optical Sensors and Si701x/2x Series Relative Humidity and Temperature Sensors. Powered by a coin-cell battery, it is controlled by an EFM32™ MCU. A Bluetooth Low Energy (BLE) module is used to broadcast sensor data to iOS or Android smart phones with the downloadable SENSOR-PUCK app. Placing your finger tip over the Si1147 sensor allows you to measure heart rate. Environmental sensing of UV Index, ambient light, relative humidity, and temperature are also provided. For power management, the board features a Touchstone TS3310 boost DC/DC converter.

Silicon Labs  SLEXP8008A Capacitive Touch Sense EVM
The  SLEXP8008A is an evaluation board for the CPT112S TouchXpress Capacitive Sensor Controller. The board serves as a user input peripheral for application development. It can be configured for different touch sense capabilities and also contains breakout pads and other peripherals for user feedback. It has 8-Capacitive Sense touch pads a 4-Channel Capacitive Sense slider. A Buzzer and a 20-pin expansion header is available for connection to a Silicon Labs Starter Kit (EFM8 or EFM32).

Sensor Expansion Evaluation Board Sensor-EXP-EVB
The SENSOR-EXP-EVB is a development board for Silicon Labs' Si701x/2x Series Relative Humidity and Temperature Sensors and Si114x UV Index, Ambient Light, Proximity and 3D Gesture Sensors. The card plugs into the expansion header of the EFM32™ Zero Gecko Starter Kit and is supported with example software and source code in the Simplicity Studio.

Biometric Sensor Expansion Card for EFM32™ Wonder Gecko Starter Kit
The Biometric-EXP is an evaluation board for the biometric applications of the Si7013 Humidity and Temperature Sensor and the Si1146 Proximity/UV/Ambient Light Sensor, which is capable of monitoring pulse rate and peripheral capillary oxygen saturation (SpO2). A Biometric-EXP Software Demo is available for download to an EFM32 Wonder Gecko STK through the Simplicity Studio.


