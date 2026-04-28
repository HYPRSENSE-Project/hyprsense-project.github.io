# DI-Hyprsense
A publicly funded project by the German Federal Ministry of Research, Technology, and Aerospace (BMFTR) within the "DE:Sign Challenge" initiative, 2026-2028.

## Project Motivation

The HYPRSENSE project, which stands for "Holistic prototYping for imPRoved Sensor design," is dedicated to closing critical gaps in the open-source design flow for creating smart sensor systems. In today's smart sensors, the complex interaction between the chip (including processor and firmware) and other electrical and mechanical components like MEMS (Micro-Electro-Mechanical Systems) is where the real value is created. A successful product that meets time-to-market and cost requirements can only be achieved by considering all these components holistically from the very beginning.
To achieve this, a "virtual prototype"—a complete system simulation model—is essential for rapid optimization cycles. While SystemC and its analog/mixed-signal extension (SystemC AMS) are the standard languages for this, there are significant challenges. The simulation of physical components like MEMS requires specialized algorithms that are not adequately supported by current open-source tools. Furthermore, a large amount of existing design intellectual property (IP) is written in VHDL, and there is no efficient open-source method to integrate it into SystemC virtual prototypes. HYPRSENSE will address these gaps by developing the necessary open-source tools to enable a seamless and efficient design process.

## Main Targets

The project will focus on three key areas of development:

* __SystemC AMS Extensions:__ We will develop and standardize an interface for SystemC AMS that allows the integration of application-specific algorithms for equation solving and time-step control. This will be used to create an open-source library specifically optimized for modeling MEMS, enabling more accurate and significantly faster simulations.
* __[VHDL to SystemC Conversion](https://github.com/HYPRSENSE-Project):__ To enable the reuse of existing IP blocks and reduce modeling efforts, we will create an open-source tool that converts synthesizable VHDL code into a cycle-accurate SystemC model. This closes a major gap for the electronics industry, where VHDL is a predominant language.
* __Sensor Model Demonstrator:__ To showcase the power and facilitate the adoption of the new tools, we will develop a comprehensive open-source demonstrator. This will feature a complete virtual prototype of a smart sensor, including a RISC-V core converted from VHDL and a complex MEMS model, providing a practical and accessible resource for the community.

## Project Partners
The HYPRSENSE project is a collaborative effort between leading industry and academic partners:

  *  __[Bosch Sensortec GmbH](https://www.bosch-sensortec.com/) (Coordinator)__
  *  __[COSEDA Technologies GmbH](https://www.coseda-tech.com/)__
  *  __[MINRES GmbH](https://www.minres.com/)__
  *  __[University of Rostock](https://www.imd.uni-rostock.de/)__

## Events & Workshops
We are excited to share our progress and connect with the community. Members of the HYPRSENSE team will be presenting our work and participating in discussions at the following events. We invite you to join us to learn more about the project and explore potential collaborations.

* __[Chipdesign Germany Forum 2026](https://www.chipdesign-germany.de/de/events/2026/dresden-chipdesign-germany-forum/)__, 5./6. May 2026, Dorint Hotel Dresden

  * Come see our presentation titled "_DI-HYPRSENSE: Virtuelle Prototypen für das Design moderner Sensorsysteme_" in the poster session.

  * Members of the team will be available for meetings at the session area.

## Contact
Bosch Sensortec GmbH<br>
Project DI-Hyprsense<br>
Gerhard-Kindler-Str. 9<br>
D-72770 Reutlingen<br>
Germany<br>
Email: dietmar.eggert@bosch-sensortec.com
