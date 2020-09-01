August 2020 results:

The results are sorted by medium of communication per application following
format: <communication_medium>\_<application>.

Each of this application are undertaking the same benchmark execution. The
folder is internally organised as follow:

 * com: Communication bandwidth.
 * com_resilience: Communication resilience (not avaialalbe for all communication medium).
 * fusage: Function usage, what function was executed when.
 * isr: IRQs service routine how often they are called.
 * mem-dyn: Dynamic memory allocation monitoring>
 * mem-static: Static memory allocation monitoring.
 * pwr: Measurement of the power at a specific moment of the application.
 * sched: Scheduler measurement providing information about the execution and rtos determinism/latency>

In each one of those folder contains at least:

 * ctf: Folder containing information of the raw capture using ctf 1.8 format.
 * .data or .json: which is the extracted data from the ctf file.


To read the ctf file, babletrace/babletrace2 are two tools deserialiasing the data from the CTF folder.
