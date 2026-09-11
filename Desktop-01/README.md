
# Desktop-01 – Random BSOD & RAM Troubleshooting

## Overview

This project involved troubleshooting a desktop computer that was experiencing random Blue Screen of Death (BSOD) errors. The system displayed different error messages each time, and the crashes could not initially be reproduced consistently.

## Issue

The computer would occasionally crash with a BSOD and display different error messages on different occasions such as MEMORY_MANAGEMENT, CRITICAL_PROCESS_DIED, FAULTY_HARDWARE_CORRUPTED_PAGE, SYSTEM_SERVICE_EXCEPTION, and KERNEL_SECURITY_CHECK_FAILURE. The crashes appeared to be random and occurred during both normal use and periods of inactivity.

## Initial Troubleshooting

I first attempted to determine whether the crashes could be reproduced through system usage or stress testing.

* Turned off XMP in BIOS
* Tried DISM Repair
* Ran SFC Scan
* Ran system stress tests to place the hardware under load.
* Allowed the system to remain idle for extended periods.
* Monitored the system for additional crashes.
* Compared the behavior during normal use, stress testing, and idle periods.

The BSODs remained unpredictable and could not be reliably reproduced through these tests.

## RAM Troubleshooting

Because inconsistent BSODs can be caused by faulty memory, I began testing the RAM configuration.

* Swapped the RAM sticks between different motherboard slots.
* Tested the system with individual RAM sticks installed one at a time.
* Compared system behavior with different RAM configurations.

The issue persisted, so I proceeded with dedicated memory testing using MemTest86.

## MemTest86 Testing

I used MemTest86 to test the system memory for hardware errors.

The memory test identified a large number of errors within minutes of starting the test, providing evidence that the RAM was the likely source of the system instability.

## Diagnosis

Based on the MemTest86 results and the previous troubleshooting steps, I determined that one of the RAM sticks was faulty.

## Resolution

The failing RAM stick was removed from the system and the remaining memory was tested to verify system stability.

After removing the faulty module, the system was able to operate normally without the previous random BSOD issues. RAM stick was replaced with a new module.

## Skills Demonstrated

* Hardware troubleshooting
* BSOD troubleshooting
* RAM diagnosis
* MemTest86 memory testing
* Component isolation
* System stability testing
* Troubleshooting through a process of elimination
