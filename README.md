# Digital System (ICE3024, 2024 Spring) 

VHDL implementations for three assignments.

## HW1 — Full Adder & 4-bit Adder
Design and simulate a 1-bit full adder and a 4-bit ripple-carry adder in VHDL. The 4-bit adder is built by cascading four full adders and verified using provided testbenches. :contentReference[oaicite:0]{index=0}

**Files (HW1/):**
- `FA.vhd` — 1-bit Full Adder design (inputs: X, Y, Cin; outputs: Sum, Cout).
- `FA_tb.vhd` — Testbench for the Full Adder.
- `4_Bit_Adder.vhd` — 4-bit ripple-carry adder design using four full adders.
- `4_Bit_Adder_tb.vhd` — Testbench for the 4-bit adder.

## HW2 — FSM Sequence Detector (1010)
Implement a sequence detector that outputs `Z=1` when the input stream contains the pattern **"1010"**. Both **Mealy** and **Moore** FSM versions are implemented with asynchronous active-low reset and synchronous state transitions on the rising clock edge. :contentReference[oaicite:1]{index=1}

**Files (HW2/):**
- `*_Mealy.vhd` — Mealy FSM sequence detector.
- `*_Mealy_tb.vhd` — Testbench for the Mealy FSM.
- `*_Moore.vhd` — Moore FSM sequence detector.
- `*_Moore_tb.vhd` — Testbench for the Moore FSM.

## HW3 — FSM Tail Light Controller
Design a Moore FSM-based tail light controller using inputs **CLK, Reset, Left, Right, Brake** and driving an **8-bit LED** output pattern. Reset is asynchronous active-low; other behaviors are synchronized to the rising edge of the clock. :contentReference[oaicite:2]{index=2}

**Files (HW3/):**
- `*FSM.vhd` — Tail light controller FSM (Moore).
- `*FSM_tb.vhd` — Testbench used to verify LED patterns and transitions.
