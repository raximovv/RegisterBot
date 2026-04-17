# RegisterBot - Tiny CPU Simulator

RegisterBot is a tiny CPU simulator built in pure Python. It models a simple fetch-decode-execute cycle with 8 registers, basic flags, an ALU, and a small instruction set. A local LLM powered by Ollama narrates each instruction step in plain language.

## Features

- 8 CPU registers: `R0` to `R7`
- Program Counter (`PC`)
- Flags: `ZERO`, `NEG`
- ALU operations:
  - `ADD`
  - `SUB`
  - `MUL`
- Instruction set:
  - `MOV`
  - `ADD`
  - `SUB`
  - `MUL`
  - `CMP`
  - `JMP`
  - `JZ`
  - `JNZ`
  - `HALT`
- Rich terminal UI with register table after every step
- Local LLM narration using Ollama

## Tech Stack

- Python
- Rich
- Ollama

## How It Works

This project simulates a tiny CPU architecture:

1. Fetch the current instruction using the program counter
2. Decode the opcode and arguments
3. Execute the instruction
4. Update registers, flags, or control flow
5. Display the new machine state

## Demo Program

The included demo computes factorial of 5 using a loop.

Expected result:

```text
5! = 120
