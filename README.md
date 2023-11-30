# Sequence-Detector
This VHDL code library implements a sequence detector that detects the presence of a specific binary sequence. 



The sequence detector takes three inputs:

clock: The clock signal
reset: The reset input
sequence_in: The binary sequence input
The sequence detector has one output:

detector_out: The output of the sequence detector
The sequence detector uses a Moore finite state machine (FSM) to detect the binary sequence. The FSM has five states:

Zero: The initial state
One: The state that is entered if the sequence_in input is 1
OneZero: The state that is entered if the sequence_in input is 0
OneZeroZero: The state that is entered if the sequence_in input is 0
OneZeroZeroOne: The state that is entered if the sequence_in input is 1
The detector_out output is 1 if the current state of the FSM is OneZeroZeroOne. Otherwise, the detector_out output is 0.
