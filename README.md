# Programmable Logic Timer & Stopwatch (Digital Logic Design)

## Project Overview
A hardware-defined digital timing system engineered using **discrete logic ICs**. This project operates without a microcontroller, utilizing synchronous counters and combinational logic to provide high-precision **Stopwatch (Count-Up)** and **Timer (Countdown)** functionality. The system automates a **220V AC load** via a relay interface upon reaching a user-defined time target.

---

## Core Features
* **Dual Mode:** Stopwatch (00:00 to Target) and Timer (Start Time to 00:00).
* **MM:SS Display:** 4-digit 7-segment output.
* **Hardware Control:** Dedicated tactile buttons for **Set**, **Start/Pause**, and **Reset**.
* **Industrial Interfacing:** Relay module for 220V appliance automation.

---

## Technical Architecture
* **Time Base:** 1Hz pulse generation via a precision **555 Timer** circuit.
* **Logic Core:** Cascaded **74LS192** BCD up/down counters managed by logic gates for state transitions.
* **Display Driver:** **74LS47** BCD-to-7-segment decoders with multiplexing logic.
* **Trigger Logic:** Gate-level detection (AND/NOR) to activate the relay at the target time or zero.
* **Power Stage:** 5V DC logic isolated from the 220V AC output using a relay driver.

---

## Design & Implementation
1.  **Simulation:** Full functional validation in **Proteus** to verify synchronous timing and gate-level logic.
2.  **Schematic Capture:** Professional circuit design in **KiCad**.
3.  **PCB Layout:** Designed a production-ready PCB in **KiCad**, implementing specific trace widths for high-voltage safety and signal integrity.

---

## Components List
* **Counters:** 74LS192 BCD Counters.
* **Decoders:** 74LS47 BCD-to-7-Segment.
* **Logic Gates:** 74LS08 (AND), 74LS32 (OR), 74LS04 (NOT).
* **Timer:** NE555.
* **Output:** 5V Relay, LED.
