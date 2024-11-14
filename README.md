# washing_machine_verilog
![image](https://github.com/user-attachments/assets/d11efb89-bc69-46a4-a254-a5f013b6d37a)
Here the product price is INR 15.

There are three states -
State 0: 0 INR in the machine
State 1: 5 INR in the machine
State 2: 10 INR in the machine

State Transitions
State 0 (0 INR):
5 INR inserted: Transition to State 1.
10 INR inserted: Transition to State 2.

State 1 (5 INR):
5 INR inserted: Transition to State 2 or if transaction cancelled then transition to State 0 and change of 5 INR.
10 INR inserted: Product dispensed, return to State 0.

State 2 (10 INR):
Nothing inserted and transaction cancelled then change of 10 INR and transitioin to State 0.
5 INR inserted: Product dispensed, return to State 0.
10 INR inserted: Product dispensed, return to State 0 with 5 INR change.
