# Hybrid TG-MTCMOS 4:1 Multiplexer for Low-Power Nanoscale Circuits

A low-power 4:1 Multiplexer designed using a hybrid 
Transmission Gate Logic (TGL) and MTCMOS power-gating 
approach, targeting 90nm CMOS technology.

## Key Results (90nm, VDD = 1.2V)

| Metric         | Conventional TG | Proposed Hybrid | Improvement |
|----------------|-----------------|-----------------|-------------|
| Power (nW)     | 168.9           | 135.4           | 19.83% ↓   |
| Delay (ns)     | 35.12           | 30.12           | 14.23% ↓   |
| PDP (fJ)       | 5.93            | 4.07            | 31.36% ↓   |

## Design Overview

- **Stage 1**: Two conventional 2:1 TG MUX blocks (fast switching)
- **Stage 2**: One MTCMOS-based 2:1 MUX with High-Vth PMOS header switch (leakage control)
- **Tool**: Cadence Virtuoso
- **Technology**: 90nm CMOS

## How It Works

Power gating is applied **only at the final output stage**, 
avoiding transistor count bloat while still cutting leakage 
across the full output path. Total extra transistors: **1**.

## Paper

See `/paper/` for the full paper PDF.
