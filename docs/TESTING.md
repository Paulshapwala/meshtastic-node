# Testing and known issues

Last documentation review: 15 November 2026. Entries summarize the available project discussion, not a fresh bench test.

| Item | Evidence / status |
|---|---|
| Editable design files | KiCad project, schematic, and PCB available |
| PCB file readability | Loaded using KiCad 10.0.8 during packaging |
| Physical assembly | Assembled board referenced in project discussion |
| Continuity investigation | Battery-negative/protection connections investigated |
| XB8089D0 protection | Unresolved; possible solder-joint fault discussed |
| Charging | Design intent discussed; operation and current not measured in the available record |
| Firmware boot and BLE connection | Not established in the available record |
| LoRa communication | Not established in the available record |
| Range and packet reliability | No measurements documented |
| Active/sleep current and battery life | No measurements documented |
| ERC / DRC and fabrication readiness | Not verified during repository packaging |

## Known issue: battery protection

The discussion identifies separate battery-negative and board-ground nets connected through the XB8089D0 protection circuit. A possible poor solder joint was considered, and JP1 was discussed as a temporary bypass. The fault remains unconfirmed. A bypass removes this circuit's protection and must not be presented as a repaired or validated design.

## Next validation steps

1. Confirm fitted component part numbers and inspect the assembled protection circuit.
2. Resolve the protection fault and record measurements demonstrating correct operation.
3. Verify supply rails, controller startup, and the appropriate firmware target.
4. Test charging with the actual module and battery specifications.
5. Test radio communication with a known working node and record settings and results.
6. Measure active and sleep current before estimating battery life.
7. Record ERC/DRC results and review the board before generating manufacturing files.

For each test, record the board revision, firmware version, instruments, setup, expected result, actual result, and date. Avoid publishing device keys, private channel settings, or precise deployment locations.
