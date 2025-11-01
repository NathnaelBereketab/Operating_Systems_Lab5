# Operating Systems Lab 5 — CPU Scheduling Simulation

description: >
  This project simulates four CPU scheduling algorithms:
  - First Come First Serve (FCFS)
  - Shortest Job First (SJF)
  - Priority Scheduling
  - Round Robin (RR)

build_instructions: |
  To compile the program:
    $ make clean
    $ make

execution: |
  To run the simulator with provided input files:
    $ ./schedsim input0.txt
    $ ./schedsim input1.txt
    $ ./schedsim input2.txt

testing: |
  Use the reference implementation schedsim_ref to verify results:
    $ ./schedsim_ref fcfs input0.txt
    $ ./schedsim_ref sjf input1.txt
    $ ./schedsim_ref rr input2.txt

expected_output: |
  Example (input0.txt):
    *********
    FCFS
    Processes   Burst time   Waiting time   Turn around time
    1           10           0              10
    2           5            10             15
    3           8            15             23
    Average waiting time = 8.33
    Average turn around time = 16.00

author:
  name: Nathnael Bereketab
  course: Operating Systems Lab 5
  year: November 1, 2025
