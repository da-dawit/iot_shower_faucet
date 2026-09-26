# IoT Shower Faucet – Self-Powered Hydro Generator

A SolidWorks design for a shower faucet attachment that generates its own electricity from the flow of water. Water entering the inlet pipe spins a three-stage propeller. A gear train carries that rotation to a small generator, which can power IoT electronics such as flow or temperature sensors without batteries or external wiring.

Designed by Dawit Chun, Dahee Chun, and Woohyeon Hwang.

![Isometric section view](photos/Screenshot%202026-09-26%20112302.png)

## How it works

1. **Water inlet**: water enters through the threaded pipe (`pipe_LH`, `pipe_RH`).
2. **Propellers**: three propellers (`propeller_1st/2nd/3rd`) on a shared axle (`axle`, `axle_3m`) are turned by the flow.
3. **Gear train**: the axle drives a large spur gear (`wheel`), which meshes with a small pinion (`pinion`) to raise the RPM.
4. **Generator**: the pinion turns the generator (`generator`) through `connector_motor_pinion`.
5. **Outlet**: water leaves through the threaded top outlet, which connects to the shower hose or head.

| Side section | Front view |
|---|---|
| ![Side section](photos/Screenshot%202026-09-26%20112250.png) | ![Front view](photos/Screenshot%202026-09-26%20112320.png) |

![Exterior](photos/Screenshot%202026-09-26%20112353.png)

## Files

| File | Description |
|---|---|
| `electric_faucet_assembly_01_02.SLDASM` | Full assembly (open this one) |
| `pipe_LH_01_02.SLDPRT`, `pipe_RH_01_02.SLDPRT` | Housing and water channel halves |
| `propeller_1st/2nd/3rd_01_02.SLDPRT` | Turbine propeller stages |
| `axle_01_02.SLDPRT`, `axle_3m_01_02.SLDPRT` | Propeller shafts |
| `connector_01_02.SLDPRT` | Axle coupling |
| `wheel_01_02.SLDPRT` | Large drive gear |
| `pinion_01_02.SLDPRT` | Small output gear |
| `connector_motor_pinion.SLDPRT` | Pinion-to-generator coupling |
| `generator_01_02.SLDPRT` | DC generator / motor body |
| `photos/` | Render screenshots |

## Opening

Open `electric_faucet_assembly_01_02.SLDASM` in SolidWorks. Keep all the `.SLDPRT` files in the same folder so the assembly can find its parts.
