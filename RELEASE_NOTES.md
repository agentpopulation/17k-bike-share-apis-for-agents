## Bike-share API endpoints, snapshot 15 Nov 2026

- 17,121 endpoints passed a keyless data call, tested 11–15 Nov 2026 (IST)
- 281 services · 60 country codes · 16,136 keyless JSON rows

### Download

- `Bike_Share_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 17,121 rows, 447.4 kB gzipped (4.4 MB as CSV), SHA-256 `dcf6b2a0f03f087ef344bea6fb2ec1a952e23d3720e48dec74e6cce62161746e`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Bike_Share_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Bike_Share_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 3,257 · Wrap one station_status or vehicle_status URL as a get_bike_availability tool: pass the system and a station or a point, return bikes, e-bikes and open docks, or the nearest available vehicles, with the feed's last_updated time.
- 📱 App features: 4,269 · Draw a station map for one city from station_information (name, position, capacity), shade the service area from system_regions, and mark no-ride and no-parking zones from geofencing_zones.
- 🧠 Grounding and data pipelines: 8,390 · Load system_information, pricing plans and vehicle types on a schedule into your own store, so an answer about what a ride costs or which e-bikes a city offers cites the operator file and its date.
- 🧪 Evals and testing: 17,121 · Run your GBFS parser against a fixed set of feeds from many operators and versions; check that station ids, coordinates, counts and prices parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 2 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 ArcGIS layer that keeps a form's default service name (it can hold people's form answers).
- Left out: 1 ArcGIS class or coursework layer (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Overlap: 2 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 17,121 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 8 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 26 of these URLs are also in 1.3m-government-open-data-apis.
- Overlap: 16,136 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 1 of these URLs is also in 53k-hazards-apis-for-agents.
- Overlap: 13 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 3 of these URLs are also in 12k-parking-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 11–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Bike-share API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
