# Cold Storage & Distribution Center — Project Plan

> A working plan for developing a temperature-controlled warehouse and distribution
> center. Figures marked **[assumption]** are placeholders for a reference design and
> should be replaced with local data (site, market, tariffs, regulations) as the
> project firms up.

---

## 1. Executive Summary

| Item | Reference design |
|---|---|
| Purpose | Store and distribute perishable goods (food, beverages, pharma) under controlled temperatures |
| Business model | Third-party logistics (3PL) — storage, handling, value-added services, last-mile distribution |
| Gross building area | ~10,000 m² **[assumption]** |
| Pallet capacity | ~12,000 pallet positions |
| Temperature zones | Frozen, chilled, ambient-controlled, plus temperature-controlled loading dock |
| Fleet | 15–20 refrigerated trucks/vans (owned or contracted) |
| Timeline | ~20–24 months from feasibility to operations |
| Indicative CAPEX | USD 12–20 M (excluding land) **[assumption — varies strongly by country]** |
| Target payback | 6–8 years at 80–85 % steady-state occupancy |

---

## 2. Market & Feasibility Study (Months 1–3)

### 2.1 Demand analysis
- Identify target segments and their temperature needs:
  - **Frozen** (−25 °C to −18 °C): meat, poultry, seafood, ice cream, frozen vegetables
  - **Chilled** (0 °C to +4 °C): dairy, fresh meat, ready meals
  - **Fresh produce** (+2 °C to +12 °C, humidity-controlled): fruit, vegetables, flowers
  - **Pharma** (+2 °C to +8 °C and +15 °C to +25 °C): vaccines, biologics, medicines
- Quantify demand: import volumes, local production, retail/HoReCa growth, seasonal peaks.
- Map competitors: capacity, rates, occupancy, service gaps.
- Interview 10–20 prospective anchor customers; aim for letters of intent covering
  30–40 % of capacity before committing to construction.

### 2.2 Site selection criteria
| Criterion | Why it matters |
|---|---|
| Proximity to ports, airports, highways | Reduces transport time and cost of cold chain |
| Distance to consumption centers | Last-mile delivery efficiency |
| Reliable power supply (ideally two feeders) | Refrigeration is ~60–70 % of operating energy |
| Water availability | Evaporative condensers, cleaning |
| Land size: ~2.5–3× building footprint | Truck yard, parking, future expansion |
| Zoning, soil conditions, flood risk | Permits and foundation cost |
| Labor availability | Shift-based workforce |
| Incentives (free zones, tax holidays) | Improves returns |

### 2.3 Feasibility outputs
- Market report and demand forecast (5–10 years)
- Shortlist of 2–3 sites with scoring matrix
- Preliminary financial model (CAPEX, OPEX, revenue, IRR, NPV)
- Go / no-go decision

---

## 3. Facility Design (Months 3–8)

### 3.1 Zoning & capacity (reference design)

| Zone | Temperature | Share of area | Approx. pallet positions |
|---|---|---|---|
| Frozen storage | −25 °C to −18 °C | 40 % | ~5,000 |
| Chilled storage | 0 °C to +4 °C | 25 % | ~3,000 |
| Produce / multi-temp rooms | +2 °C to +15 °C (adjustable) | 10 % | ~1,200 |
| Pharma (GDP-compliant) | +2 °C to +8 °C / +15 °C to +25 °C | 10 % | ~1,500 |
| Ambient / dry | Controlled ambient | 5 % | ~1,300 |
| Loading dock (anteroom) | +2 °C to +8 °C | — | Staging |
| Blast freezing | −35 °C to −40 °C | small rooms | 2–4 rooms, ~20–30 t/day |
| Offices, amenities, plant rooms | — | 10 % | — |

Design rules of thumb:
- Clear height 10–12 m for selective racking; up to 30–40 m if using automated high-bay (ASRS).
- Rooms designed as **multi-temperature** where possible to follow demand shifts.
- Airlocks / rapid-roll doors between zones; temperature-controlled dock to protect the chain.

### 3.2 Building envelope
- Insulated sandwich panels (PIR/PUR): ~150–200 mm for frozen, ~100–120 mm for chilled.
- Heated / ventilated floor slab under freezer rooms to prevent frost heave.
- Vapor barriers, thermal-break details at all penetrations.
- Fire-rated panels where required by code; fire compartmentation.

### 3.3 Refrigeration system
| Option | Pros | Cons |
|---|---|---|
| Ammonia (NH₃) central plant, often NH₃/CO₂ cascade | Very efficient, low GWP, best for large sites | Toxic; needs specialist operators and safety systems |
| CO₂ transcritical | Natural refrigerant, good heat recovery | Less efficient in hot climates without adiabatic/ejector add-ons |
| HFO/HFC packaged units | Lower initial cost, modular | Higher GWP, refrigerant phase-down risk |

- Recommendation for this scale: **NH₃/CO₂ cascade** (or CO₂ transcritical in cool climates).
- N+1 redundancy on compressors and condensers.
- Heat recovery for underfloor heating, hot water, offices.
- Hot-gas or electric defrost, scheduled to off-peak hours.

### 3.4 Energy & utilities
- Dual power feeders if available + standby diesel/gas generators sized for critical load.
- Rooftop solar PV (refrigeration load matches daytime peak) — 1–2 MWp potential.
- Thermal energy storage (ice/eutectic) to shift load to cheaper tariff periods.
- LED lighting with motion sensors; VFDs on fans and compressors.
- Sub-metering by zone for cost allocation and energy KPIs.

### 3.5 Storage & material handling
- **Racking:** selective (fast movers), drive-in / push-back (bulk, frozen), mobile racking
  (maximizes density in expensive frozen space by ~80 %).
- **Optional automation:** ASRS / shuttle systems — higher CAPEX, much lower labor and
  energy per pallet; consider for frozen zone.
- **Equipment:** reach trucks and VNA trucks rated for cold (heated cabins, cold-rated batteries,
  preferably lithium-ion), pallet jacks, order pickers.
- **Docks:** 1 dock door per ~400–600 m² of storage; dock shelters, levelers,
  separate inbound/outbound sides for cross-docking.

### 3.6 Safety & fire protection
- Ammonia detection, emergency ventilation, machinery room isolation, emergency response plan.
- Fire detection suited to cold rooms (aspirating smoke detection).
- Sprinklers: dry-pipe / pre-action in freezer zones.
- "Man-trapped" alarms and inside-release on all cold-room doors.
- Slip-resistant flooring, PPE and cold-exposure work/rest regimes.

---

## 4. Technology & Systems

| System | Function |
|---|---|
| **WMS** (Warehouse Management System) | Receiving, put-away, FEFO/FIFO, lot & expiry tracking, picking, billing |
| **TMS** (Transport Management System) | Route planning, fleet scheduling, proof of delivery |
| **Temperature monitoring** | Continuous logging of every room and vehicle, alarms by SMS/email, audit trails (21 CFR Part 11 for pharma) |
| **BMS / SCADA** | Refrigeration, energy, door and alarm control |
| **Customer portal / EDI / API** | Real-time inventory visibility, order entry, reporting |
| **Access control & CCTV** | Security, traceability |
| **Telematics** | GPS + reefer temperature tracking on all trucks |

---

## 5. Distribution Operations

### 5.1 Process flow
1. **Inbound:** appointment booking → temperature check of load → quality inspection →
   labeling (barcode/RFID) → put-away to assigned zone.
2. **Storage:** FEFO rotation, cycle counts, continuous temperature monitoring.
3. **Order processing:** order received via portal/EDI → wave planning → picking →
   consolidation in chilled dock.
4. **Outbound:** pre-cooled trucks, load temperature recorded, sealed, dispatched.
5. **Delivery:** route-optimized, proof of delivery with temperature log.
6. **Returns / reverse logistics:** inspection, quarantine, disposal or re-stock.

### 5.2 Fleet
- Mix of heavy reefer trucks (regional/line-haul) and multi-compartment vans (urban last-mile).
- Start with a hybrid model: own core fleet + contracted carriers for peaks.
- Consider electric vans for urban routes as charging infrastructure allows.

### 5.3 Value-added services (higher margin)
- Blast freezing and tempering
- Repacking, labeling, kitting, case-picking
- Fruit ripening rooms (bananas, avocados)
- Customs-bonded storage / cross-docking
- Quality inspection and lab services

---

## 6. Regulatory & Certification Checklist

- Building, environmental and fire permits; environmental impact assessment
- Refrigerant / ammonia safety permits and pressure-vessel certification
- Food safety: **HACCP**, **ISO 22000** / **FSSC 22000**, or **BRCGS Storage & Distribution**
- Pharma: **GDP** (Good Distribution Practice), WHO guidelines, local health authority license
- **ISO 9001** (quality), **ISO 14001** (environment), **ISO 45001** (health & safety)
- Halal certification if serving relevant markets
- Customs-bonded warehouse license (if applicable)
- Vehicle permits and food-transport certifications (e.g., ATP for refrigerated transport)

---

## 7. Organization & Staffing (steady state, ~2-shift operation)

| Function | Headcount (approx.) |
|---|---|
| General manager | 1 |
| Operations / warehouse managers & supervisors | 6–8 |
| Warehouse operators (forklift, pickers, receivers) | 50–70 |
| Inventory control & quality (QA/QC, pharma QP) | 6–8 |
| Refrigeration & maintenance engineers/technicians | 6–10 |
| Transport planners & drivers | 25–40 |
| Customer service, sales, finance, HR, IT | 10–15 |
| Security, cleaning (often outsourced) | 8–12 |
| **Total** | **~115–165** |

Training priorities: cold-chain integrity, food safety/GDP, forklift certification,
ammonia safety, cold-stress awareness, WMS usage.

---

## 8. Financial Plan

### 8.1 Indicative CAPEX (reference design, excluding land) **[assumption]**

| Item | Share of CAPEX |
|---|---|
| Civil works, structure, insulated envelope, floors | 35–40 % |
| Refrigeration plant & distribution | 18–22 % |
| Electrical, generators, solar PV | 8–10 % |
| Racking & material handling equipment | 10–15 % |
| IT systems (WMS, TMS, monitoring, BMS) | 3–5 % |
| Fleet (if owned) | 8–12 % |
| Design, permits, project management | 5–7 % |
| Contingency | 7–10 % |

### 8.2 Operating cost drivers
- Energy (typically the largest after labor): 20–30 % of OPEX
- Labor: 30–40 %
- Maintenance, insurance, depreciation, fuel, IT licenses

### 8.3 Revenue streams
- Storage: charged per pallet per day/week (higher rates for frozen and pharma)
- Handling: per pallet/case in and out
- Value-added services: blast freezing, repacking, ripening, labeling
- Transportation: per drop, per km, or per route
- Dedicated/contracted space: fixed monthly fees from anchor customers

### 8.4 Key financial targets
- Ramp-up: ~50 % occupancy in Year 1 → 75 % in Year 2 → 80–85 % from Year 3
- EBITDA margin at steady state: 25–35 %
- Project IRR target: ≥ 15 %
- Sensitivities to model: energy price, occupancy, storage rate, construction cost, interest rate

### 8.5 Funding options
- Equity + bank project finance (typical 60/40 to 70/30 debt/equity)
- Development bank / green financing (natural refrigerants + solar qualify in many programs)
- Sale-and-leaseback of the building once operational
- Government agri-food / logistics incentives

---

## 9. Implementation Timeline

| Phase | Months | Key deliverables |
|---|---|---|
| 1. Feasibility & business plan | 1–3 | Market study, site shortlist, financial model, go/no-go |
| 2. Land acquisition & financing | 3–6 | Site secured, funding committed, anchor-customer LOIs |
| 3. Concept & detailed design | 4–8 | Layout, refrigeration design, tender documents |
| 4. Permits & approvals | 6–9 | Building, environmental, fire, refrigerant permits |
| 5. Procurement & contracting | 8–10 | EPC/design-build contractor, refrigeration, racking, IT vendors |
| 6. Construction — civil & envelope | 10–18 | Foundations, structure, insulated panels, floors |
| 7. MEP & refrigeration installation | 14–20 | Plant, electrical, fire systems, racking |
| 8. Testing & commissioning | 19–21 | Pull-down, temperature mapping, system integration tests |
| 9. Certification & validation | 20–22 | HACCP/BRCGS/GDP audits, pharma qualification (IQ/OQ/PQ) |
| 10. Recruitment & training | 18–22 | Staff hired and trained, SOPs written |
| 11. Soft launch & ramp-up | 22–24+ | Anchor customers onboarded, gradual volume increase |

> Note: freezer rooms need a **slow, controlled pull-down** (often 1–2 °C per day) to
> protect the floor and panels — plan 3–4 weeks for this in commissioning.

---

## 10. Risk Register

| Risk | Impact | Mitigation |
|---|---|---|
| Power outage | Product loss, liability | Dual feeders, generators, thermal mass, alarms, insurance |
| Refrigeration failure | Product loss | N+1 redundancy, preventive maintenance, 24/7 on-call |
| Ammonia leak | Safety, regulatory | Detection, ventilation, low-charge design, emergency drills |
| Low occupancy in ramp-up | Cash-flow pressure | Anchor LOIs pre-construction, phased build-out |
| Energy price spikes | Margin erosion | Solar PV, efficiency measures, energy surcharge clauses in contracts |
| Construction delays / cost overrun | Late revenue | Fixed-price EPC contract, contingency, experienced contractor |
| Temperature excursions in transport | Claims, reputation | Telematics, pre-cooling SOPs, driver training |
| Regulatory non-compliance | License loss | QA team, internal audits, certification roadmap |
| Labor shortage / turnover | Service quality | Competitive pay, cold-work allowances, training, automation |

---

## 11. Key Performance Indicators

| Category | KPI | Target |
|---|---|---|
| Capacity | Occupancy rate | ≥ 80–85 % |
| Quality | Temperature excursions | 0 critical / month |
| Accuracy | Inventory accuracy | ≥ 99.5 % |
| Accuracy | Order picking accuracy | ≥ 99.8 % |
| Service | On-time-in-full (OTIF) deliveries | ≥ 98 % |
| Speed | Dock-to-stock time | < 2 hours |
| Energy | kWh per pallet position per year / per m³ | Track and reduce yearly |
| Safety | Lost-time injury frequency | 0 |
| Financial | Revenue per pallet position, EBITDA margin | Per business plan |

---

## 12. Sustainability

- Natural refrigerants (NH₃, CO₂) — near-zero global-warming potential
- Rooftop solar + battery or thermal storage
- Heat recovery from refrigeration for floor heating and hot water
- High-performance insulation and rapid-roll doors to cut infiltration losses
- Electric forklifts (lithium-ion) and progressive fleet electrification
- Target green building certification (LEED / EDGE / BREEAM)

---

## 13. Immediate Next Steps

1. Confirm **location / country** and **target customer segments** (food, pharma, both).
2. Commission a market study and gather competitor rates.
3. Shortlist sites and check power capacity with the utility early.
4. Engage a specialist cold-storage design consultant for a concept layout.
5. Build the detailed financial model with local costs and tariffs.
6. Start conversations with 5–10 potential anchor customers.

---

### Information needed to tailor this plan
- Country / city and candidate sites
- Target products and temperature mix
- Desired capacity (pallets or tonnes) and growth horizon
- Budget range and funding structure
- Owned vs. outsourced fleet, and service area
- Any automation ambitions (manual vs. ASRS)
