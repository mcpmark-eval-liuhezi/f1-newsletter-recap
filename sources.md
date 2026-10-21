# Sources — which dataset each figure came from

Every figure in `briefing.md` was retrieved from the F1 data services at pull time. Mapping below.

| Figure | Dataset / service call |
|--------|----------------------|
| 2024 final Drivers' Championship top three with points and wins (Verstappen 437, Norris 374, Leclerc 356) | Driver standings, season 2024 (after round 24) |
| 2024 Constructors' Champion with points (McLaren 666) and full constructors' order | Constructor standings, season 2024 |
| 2024 season opener identification — Round 1 = Bahrain Grand Prix, Bahrain International Circuit, Sakhir, 2024-03-02 15:00 UTC | Race calendar, season 2024 |
| Bahrain winner (Verstappen, 57 laps, 1:31:44.742, fastest lap 1:32.608 lap 39) and podium order | Historic race results, 2024 round 1 |
| Bahrain pole sitter (Verstappen, Q3 1:29.179) | Qualifying results, 2024 round 1 |
| Driver profiles — permanent number, nationality, date of birth for Hamilton, Verstappen, Norris, Leclerc | Driver info, queried per driverId exactly as given by the 2024 standings: `hamilton`, `max_verstappen`, `norris`, `leclerc` |
| 2024 Belgian GP race session identification — Race, session key 9574, 2024-07-28 13:00–15:00 UTC, meeting 1242, Spa-Francorchamps | Historical sessions, 2024, Belgium (Race selected — not Practice 1–3 or Qualifying, session keys 9567–9570) |
| Spa weather — air temp 20.6–21.5 °C, track temp 39.4–42.6 °C, rainfall 0, wind 0.5–2.6 m/s variable, humidity 49–53 %, pressure ~978 hPa | Weather data, session key 9574 (race session) |
| Spa race control messages (verbatim list in briefing) | Race control messages, session key 9574 (race session) |
| 'As of now' live check — nothing live; session status empty, timing feed 404 | Current session status + live timing data, checked at pull time |

## Pull-time notes

- All driver profile fields were taken from the driver-info service responses; no figures came from memory.
- The Spa figures are from the race session only (key 9574); practice/qualifying sessions were excluded by design.
- Weather figures cite the sample records returned by the service (minute-level samples reviewed from 12:08 to 12:45 UTC).
