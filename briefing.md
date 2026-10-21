# 2024 Season Retrospective — 'Two Years On'

Data edition of the newsletter. Every figure below was pulled from the F1 data services (see `sources.md` for the dataset behind each number). Final standings are after round 24 of 24.

## The Champions

| Pos | Driver | Team | Points | Wins |
|-----|--------|------|--------|------|
| 1 | Max Verstappen | Red Bull | 437 | 9 |
| 2 | Lando Norris | McLaren | 374 | 4 |
| 3 | Charles Leclerc | Ferrari | 356 | 3 |

**2024 Drivers' Champion: Max Verstappen — 437 points**, 63 points clear of Lando Norris (374), with Charles Leclerc third on 356.

**2024 Constructors' Champion: McLaren — 666 points** (6 wins), finishing ahead of Ferrari (652, 5 wins) and Red Bull (589, 9 wins). Mercedes took fourth with 468.

## Season opener — Bahrain Grand Prix (Round 1, 2 March 2024)

The 2024 calendar opened with the **Bahrain Grand Prix at Bahrain International Circuit, Sakhir (Round 1, 2024-03-02, 15:00 UTC)**.

- **Winner: Max Verstappen (Red Bull)** — pole-to-flag, 57 laps, winning time 1:31:44.742, and the race's fastest lap (1:32.608 on lap 39, 210.383 kph).
- **Pole: Max Verstappen** — Q3 1:29.179 (Q1 1:30.031, Q2 1:29.374), lining up P1 on the grid.
- Podium: Verstappen, Pérez (+22.457), Sainz (+25.110); Leclerc and Russell completed the top five.

## Driver profiles

Profile fields below (permanent car number, nationality, date of birth) are as returned by the driver-info service, looked up using the driver identifiers supplied by the 2024 standings.

| Driver | Permanent number | Code | Nationality | Date of birth |
|--------|------------------|------|-------------|---------------|
| Lewis Hamilton | 44 | HAM | British | 1985-01-07 |
| Max Verstappen | 3 | VER | Dutch | 1997-09-30 |
| Lando Norris | 1 | NOR | British | 1999-11-13 |
| Charles Leclerc | 16 | LEC | Monegasque | 1997-10-16 |

*Note: the standings/driver-info service returns permanent number 1 for Norris — flagged in the 'Data follow-ups' issue.*

## Conditions at Spa — 2024 Belgian Grand Prix (Race)

Race session, Sunday 28 July 2024, session key 9574, Spa-Francorchamps (meeting 1242). Session window 13:00–15:00 UTC.

**Weather during the race** (minute-by-minute sample records reviewed from 12:08 to 12:45 UTC):

- Air temperature: 20.6–21.5 °C
- Track temperature: 39.4–42.6 °C
- Rainfall: 0 in every returned sample — no rain recorded; race control itself stated 'RISK OF RAIN FOR F1 RACE IS 0 %'
- Wind: light, 0.5–2.6 m/s, with direction swinging through the full compass (0–358°)
- Humidity: 49–53 %; pressure steady around 978.0–978.3 hPa

**Race control messages** (verbatim, in order):

| Time (UTC) | Lap | Category | Message |
|------------|-----|----------|---------|
| 12:20:01 | 1 | Flag | GREEN LIGHT - PIT EXIT OPEN |
| 12:30:01 | 1 | Other | PIT EXIT CLOSED |
| 12:45:13 | 1 | Other | RISK OF RAIN FOR F1 RACE IS 0 % |
| 12:57:01 | 1 | Drs | DRS DISABLED |
| 13:03:52 | 1 | SessionStatus | SESSION STARTED |
| 13:03:53 | 1 | Flag | GREEN LIGHT - PIT EXIT OPEN |
| 13:05:45 | 2 | Drs | DRS ENABLED |
| 13:07:26 | 2 | Other | TURN 5 INCIDENT INVOLVING CAR 23 (ALB) NOTED - LEAVING THE TRACK AND GAINING AN ADVANTAGE |
| 13:08:40 | 3 | Other | CAR 18 (STR) TIME 1:51.654 DELETED - TRACK LIMITS AT TURN 4 LAP 2 15:06:13 |
| 13:10:58 | 4 | Other | FIA STEWARDS: TURN 5 INCIDENT INVOLVING CAR 23 (ALB) REVIEWED NO FURTHER INVESTIGATION - LEAVING THE TRACK AND GAINING AN ADVANTAGE |
| 13:12:33 | 5 | Other | CAR 4 (NOR) TIME 1:50.504 DELETED - TRACK LIMITS AT TURN 6 LAP 2 15:06:24 |
| 13:28:03 | 14 | Other | CAR 44 (HAM) TIME 1:48.204 DELETED - TRACK LIMITS AT TURN 4 LAP 13 15:26:31 |
| 13:30:13 | 15 | Other | CAR 27 (HUL) TIME 1:50.517 DELETED - TRACK LIMITS AT TURN 6 LAP 14 15:28:54 |
| 13:30:57 | 15 | Flag | YELLOW IN TRACK SECTOR 15 |
| 13:30:58 | 15 | Flag | CLEAR IN TRACK SECTOR 15 |
| 13:31:41 | 16 | Other | CAR 55 (SAI) TIME 1:51.152 DELETED - TRACK LIMITS AT TURN 14 LAP 15 15:30:56 |
| 13:47:00 | 24 | Other | CAR 20 (MAG) TIME 1:49.372 DELETED - TRACK LIMITS AT TURN 4 LAP 23 15:45:21 |
| 13:48:01 | 25 | Other | CAR 4 (NOR) TIME 1:48.464 DELETED - TRACK LIMITS AT TURN 19 LAP 23 15:46:06 |
| 14:05:27 | 34 | Other | CAR 2 (SAR) TIME 1:48.465 DELETED - TRACK LIMITS AT TURN 4 LAP 33 16:03:54 |
| 14:09:59 | 37 | Other | CAR 55 (SAI) TIME 1:47.358 DELETED - TRACK LIMITS AT TURN 4 LAP 36 16:08:24 |
| 14:18:54 | 42 | Other | CAR 55 (SAI) TIME 1:47.226 DELETED - TRACK LIMITS AT TURN 4 LAP 41 16:17:22 |
| 14:23:48 | 44 | Flag | CHEQUERED FLAG |
| 14:23:50 | 44 | SessionStatus | SESSION FINISHED |

No safety car, no red flags and no penalties were issued in the messages returned — the notable entries are the brief single-sector yellow at 13:30:57 and a string of track-limits lap-time deletions, with Sainz (55) hit three times.

## As of now — live check

**Nothing is live at this moment.** The session-status feed returned an empty payload (no event, session type or state), and the live-timing feed returned an HTTP 404 — no live timing data is available. There is no live session to report.
