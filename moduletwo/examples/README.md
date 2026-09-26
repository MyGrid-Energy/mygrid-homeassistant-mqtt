# Example automations

Copy into Home Assistant after **Home Assistant control** is selected on the Control tab (**Enable Home Assistant** is diagnostics only). Replace the sample entity ids with your ModuleTwo Power Setpoint and household entities. For grid power, [VoltBridge Actual power](../../voltbridge/entities.md) is in **kW** (negative = export); ModuleTwo setpoints are in **W**.

| File | What it does |
| --- | --- |
| [surplus-when-heatpump-idle.yaml](surplus-when-heatpump-idle.yaml) | Charge from export when the heat pump is off; idle when surplus is gone |
| [pause-discharge-while-ev-charges.yaml](pause-discharge-while-ev-charges.yaml) | Idle while the EV charges; optional discharge after |
| [force-charge-before-price-spike.yaml](force-charge-before-price-spike.yaml) | Charge before a clock window; idle when the window starts |
| [self-consumption-offline.yaml](self-consumption-offline.yaml) | Local self-consumption (charge on surplus, discharge on deficit) — useful for offline operation or coordinating with another battery Smart Control can't see |
