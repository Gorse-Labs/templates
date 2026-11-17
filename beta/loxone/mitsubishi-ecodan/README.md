# Mitsubishi Ecodan Monitor (Loxone, Modbus RTU)

For Ecodan heat pumps (FTC4/5/6) via a Mitsubishi MelcoBEMS MINI (A1M or A1M+) interface. RTU, 9600 baud, 8N1.

Read only: nothing is written to the heat pump. 47 readings: temperatures (outdoor, flow, return, tank, zones, rooms), setpoints, operating mode, defrost, compressor frequency, pumps and boosters, fault code and kWh totals.

Based on the work of Jonathan Dixon and Lifestyle Logic Limited, CC BY 4.0. See [CREDITS.md](../../../CREDITS.md).

## Still to confirm on a real unit

- Units of Electrical power used (379) and Heat power produced (380): kW or W
- Whether the kWh registers reset daily or keep running
- That Loxone Config accepts the signed data type on the temperature registers

Status: beta v0.1, unverified. A Control template (setpoints, modes, Force DHW, holiday) is available to signed-up testers.
