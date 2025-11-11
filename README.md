# Unbuffered Mult

An "unbuffered mult" is a passive signal splitter that splits one input signal into multiple outputs without using a powered buffer, like a TL074 op amp.
This means the signal can lose voltage or be slightly degraded with each signal tap, making it ideal for voltage non-critical signals like gates and triggers.
However, it is not recommended for voltage precise signals (CV), which require a buffered mult to maintain signal integrity.

**Note:** This is a learning exercise.
