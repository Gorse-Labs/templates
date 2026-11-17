# Daikin Altherma via HomeHub EKRHH Monitor (Loxone, Modbus RTU)

For Daikin Altherma 3 heat pumps with the Daikin HomeHub (EKRHH), use case 3 (Modbus RTU). 9600 baud, 8N1, default address 1 (set in the ONECTA app).

Read only: nothing is written to the heat pump. Temperatures, flow, power, status and limits. Temp16 and Pow16 values are scaled /100.

Built by Gorse Labs from Daikin document 4P744838-1E. Daikin numbers registers from 1; the template uses 0-based addresses (listed number minus 1).

## Still to confirm on a real unit

- The 0-based addressing (one known reading, e.g. outdoor temperature, confirms it)

If you use a Daikin DCOM gateway instead of the HomeHub, use the Daikin DCOM template in the Loxone Library.

Status: beta v0.1, unverified. A Control template is available to signed-up testers.
