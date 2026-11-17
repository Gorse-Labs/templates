# SolarEdge inverter (Loxone, Modbus TCP)

Based on the work of Jonathan Dixon and Lifestyle Logic Limited ([original](https://gitlab.com/joth/loxonetemplates), CC BY 4.0). See [CREDITS.md](../../../CREDITS.md).

The `*_combined` readings hold a value and its scale factor read together, so a scale change can't cause a spike. They must be split and scaled in logic. Use the example project from the original repository:

- [SolarEdge_Example.Loxone](https://gitlab.com/joth/loxonetemplates/-/blob/main/SolarEdge_Example.Loxone)

Status: beta (v0.1 Gorse edition). The original runs on Joth's own system; this edition only adds comments and hint texts.
