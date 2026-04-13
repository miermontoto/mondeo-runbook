# Mondeo Runbook - Agent Context

Knowledge base for a **2005 Ford Mondeo Mk3 Estate** with the **2.2 TDCi Duratorq (ZSD-422)** engine.
Spanish-market car (LHD), originally bought in Valencia, currently in **Asturias**. 300,000 km on the clock.
Owner has limited mechanical experience but genuinely loves this car - explanations should be practical
and approachable. At this mileage, maintenance vigilance is key.

## Vehicle Identity

| Field | Value |
|---|---|
| Model | Ford Mondeo Mk3 Estate **Titanium X** (facelift, 2005-2007) |
| Engine | 2.2 Duratorq TDCi (code: ZSD-422, QJBA/QJBB) |
| Displacement | 2,198 cc (inline-4, 16v DOHC, chain-driven cams) |
| Power | 155 PS / 114 kW @ 3,500 rpm |
| Torque | 360 Nm @ 1,800-2,250 rpm |
| Gearbox | 6-speed manual (Getrag M66) |
| Drive | Front-wheel drive |
| Fuel | Diesel (Euro 3/4) |
| Body | CD132 platform, estate/wagon variant |
| Trim | Titanium X (top-of-range), all options except navigation |
| Market | Spanish (LHD), purchased in Valencia, based in Asturias |
| Odometer | ~300,000 km |
| Headlights | Xenon with auto-levelling (F16/F18 = 20A fuses) |
| Audio | Sony stereo with 6-disc CD autochanger |
| Wheels (current) | Ford Focus RS rims (18", 5x108, fit natively) |

## Quick Reference - Most Used Values

| Item | Specification |
|---|---|
| Engine oil | 5W-30, Ford WSS-M2C913-C (or -B/-D) |
| Engine oil capacity | ~6.2 L (with filter) |
| Gearbox oil | 75W-90, Ford WSS-M2C200-C3, 2.0 L |
| Coolant | Ford WSS-M97B44-D (red, OAT-based) |
| Fuel tank | 59 L |
| Front brakes | 300 mm vented discs, 24 mm thick |
| Rear brakes | 280 mm solid discs, 12 mm thick |
| Sump plug torque | 23 Nm |
| Wheel nut torque | 115-142 Nm |
| Wheel bolt pattern | 5x108, M12x1.5 |
| Wheels (fitted) | Focus RS 18" rims, 225/40 R18 (5x108, native fit) |

## Knowledge Base Structure

```
specs/                - technical specifications (engine, fluids, dimensions, brakes, electrical, wheels)
maintenance/          - service schedule, current issues, common problems and diagnostics
references/
  sources.md          - external links organized by topic (entries marked [LOCAL] have offline copies)
  saved/              - offline archive of key references (14 MB, 17 files)
    manuals/          - Haynes manual PDF, Ford technical specs PDF
    official/         - Wikipedia articles (Mondeo Mk3, Duratorq engine)
    specs/            - Vehicle spec pages (auto-abc, ultimatespecs)
    electrical/       - Fuse box diagrams (2 sources)
    forums/           - 8 archived forum threads (TalkFord, Ford Owners Club)
    diagnostics/      - Turbo actuator fault guide (ECU Testing)
```

## Key Things to Know

- The 2.2 TDCi uses a **timing chain** (not belt) - no fixed replacement interval, inspect at ~150k km
- The auxiliary/drive belt is a 100k mile item
- **Turbo actuator failure** is the single most common issue - causes limp mode and flashing glow plug light
- The front subframe must come off for clutch/DMF work - this is a ~6+ hour job
- The EGR valve tends to stick open - cleaning it regularly prevents rough idle
- This engine does NOT have a DPF (diesel particulate filter) in the Mk3 - that was added in the Mk4
- Battery must be a silver calcium type due to the smart charging system
- The estate Titanium X has ~540 L boot space (seats up), ~1,700 L (seats folded)
- Titanium X has ESP, heated/cooled front seats, Quickclear heated windscreen, auto headlights, rain sensor, cruise control, auto-dimming mirror, electric folding heated mirrors with puddle lights, privacy glass
- This car has **all Titanium X options fitted except navigation and heated rear seats**: xenon headlights, 8-way electric driver's seat, park assist, Bluetooth, electric sunroof, Sony 6-CD
- At 300k km, major items already replaced: DMF+clutch, water pump, shocks, aux belt, glow plugs, battery
- Outstanding high-mileage items: timing chain inspection (overdue), gearbox oil, rubber bushes/mounts
- **Spanish market (LHD), Asturias:** ITV annual (car is 20+ years old). Asturias = wet Atlantic climate, watch for corrosion. See `maintenance/service-schedule.md`
- Currently running **Focus RS rims** (same 5x108 PCD/63.4mm bore, direct fit)

## Agent Instructions

When answering questions about this car:
1. Check relevant files in `specs/` and `maintenance/` for detailed data
2. For deeper research, check `references/saved/` first (offline copies), then `references/sources.md` for live links
3. The Haynes manual PDF at `references/saved/manuals/haynes-mondeo-service-repair-manual.pdf` is the most comprehensive single reference
4. Always mention safety precautions for DIY tasks (jack stands, disconnecting battery, etc.)
5. When fluid specifications matter, always cite the Ford WSS code, not just the grade
6. If uncertain about a value, say so - wrong torque specs or fluid types can cause real damage
