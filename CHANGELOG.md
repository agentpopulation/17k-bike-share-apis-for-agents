# Changelog

## 2026-11-15 (snapshot-2026-11-15)

- First release: 17,121 endpoints from 281 services, tested 11–15 Nov 2026 (IST), snapshot 15 Nov 2026.
- Rebuilt under the same snapshot with the latest leave-out rules (other addresses of a left-out ArcGIS layer, teaching organisations, more class-layer, name and record rules): 17,059 endpoints from 267 services, 62 fewer endpoints than first published under this snapshot (17,121 from 281 services), tested 11–15 Nov 2026 (IST).
- The repository holds a 1,000-row sample and the services list; the full list is the release download Bike_Share_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz.
- GitHub name: 17k-bike-share-apis-for-agents (was bike-share-api-endpoints).
- Left out: 2 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 ArcGIS layer that keeps a form's default service name (it can hold people's form answers).
- Left out: 2 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 12 rows of ArcGIS Online organisations that are class accounts (3 class sets or more in at least 20% of their rows, 10 class sets or more with no organisation name, or layers signed by students read by hand): their other layers are students' work too.
- Left out: 49 rows of the ArcGIS Online organisations of universities, colleges and schools (many of their layers are students' work).
