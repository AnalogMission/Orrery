# Orrery Planetary Synthesizer — roadmap
Last updated: v0.300 (session 7, 12 Oct 2026) · ★ milestone: v0.300 (first-release candidate) · earlier fallback: v0.211

## FIRST RELEASE (session 7) — decided
- **v0.300 ★ is the first-release candidate**: a simplified, weathered "barn find" instrument.
- **Look:** very dark grey worn case (not green), procedural rust/pits/chips, worn glass. No pulsing invitations.
- **Header, one line:** title · TRANSPORT (START, PANIC, REC, now, sync) · VIEW (CLOCK, SKY, SCOPE) · SHOW behind a sun logo (hidden by default).
- **Views:** CLOCK (the planetary cards, fully open; engages the CLOCK preset but doesn't start), SKY (opens here), SCOPE. No 3D view; no single-planet views; card nameplates don't open machines.
- **Presets** (one bank, left): DRONE (SCOPE, ⧗, 1 s fade-ins) · CLOCK (fixed Cs Mercury C1 → Pluto C9, blips on planetary seconds, centred reverb, dry) · BELLS · 1st. START engages BELLS if nothing is lit.
- **Planet keys are mutes:** click toggles, shift-click solos, SUN = all on / all off. Muted scope tubes go dead.
- **MAJOR / MINOR MOONS** keys right of the planets: lit = audible; dark = silent and unglowing.
- **System balance:** 2.5/√N per system so every planet's family sounds about equally loud.
- **INVERT** flips pitch and turns the phosphor screens negative.
- ZODIAC, the card +/− toggle, lamp click-to-mute and the SEQUENCER name are gone.

## Next (offered, not decided)
- Dim muted planets on the Sun's scope; hide switched-off moons in SKY entirely; match mute fade-out to 1 s; side handles and more weathering details.

## Decided (Charlie)
- This is a research project. The Orrery's work is the basis, but the synth architecture changes dramatically.
- There are 9 planet synths. Moons modulate their planet. The Sun is the master bus.
- Every body gets a routing matrix, with its JPL data as routable sources.
- The rack is rebuilt from legendary synth modules.
- Work proceeds from the Sun outward.
- The Orrery Line is the eventual merge of the sequencer and the synth.
- **A whole new ball game (session 2):** the old presets, patches, mod matrix and LFOs are deleted (v0.048). The old sequencer no longer sounds; its strikes are off (v0.027) and its control row is hidden (v0.049).
- **Spin is the first patch point** (v0.027): a planet triggers from its own rotation and orbit, not from orbital distance (the redundancy Charlie disliked in the original Orrery).
- **Each planet carries a beam** fixed on its surface; 0° = the beam on the Sun's centre (local noon). Spin is measured on the solar day (v0.043).
- **The page opens on the real sky** (v0.057): real orbits (J2000 + Kepler) and real spins (IAU/WGCCRE prime meridians; Earth's beam on Greenwich). **now** resets to it; **sync** is the downbeat: every needle to the top and every planet sounds (v0.097; spins to noon, orbit clocks re-zeroed, orbits untouched). Needles trigger only at the top (v0.097).
- **Real time is the default rate** (1:1, v0.052). At 1:1, Earth's hour-angle seconds/minutes/hours are the clock.
- **Triggers** (toggles, any mix; top bar, far right):
  - ORBIT: precession (v0.071, apsidal; slowest) · years (crossing 0°, the J2000 equinox) · months (each 30° zodiac sign, a grid all nine share).
  - SPIN: days · hours (15°) · degrees · minutes (15′) · arcmin · seconds (15″) · arcsec · ms (15 mas, v0.095).
  - Each has a nine-hand rotator (one hand per planet, its progress through the unit).
- **Pitch: one C per planet, Sun outward, low to high** (v0.134): Mercury C-1 and Venus C0 (drones), Earth C1, Mars C2, Jupiter C3, Saturn C4, Uranus C5, Neptune C6, Pluto C7. **C8–C9 are kept for comets.**
- **The card lamp is each voice's mute** (v0.131): click to mute/unmute, shift-click to solo (v0.153); it glows and flickers while the voice sounds (v0.132, v0.135); the sounding note shows on the brass plate (v0.136). The **brass nameplate opens the planet's machine** (v0.146).
- **Every trigger plays the planet's own synth** (v0.137). Trigger keys are a **switch**: click picks one, shift-click stacks (v0.139). Default trigger = SECONDS (v0.138). **Milliseconds retired** (v0.141).
- **Cards (v0.143):** ORBIT (precession, year, month) · LOCAL SOLAR TIME (hours, minutes, seconds) · SPIN (degrees, arcmin, arcsec) · DAYS odometer with a ×10³ MULT drum (v0.148). Dials are **clock faces**: each hand named for what it counts, turning once per the next unit up (v0.142).
- **Deep time is exact** (v0.140): spin carried as whole turns + fraction; back to 1:1 after any run and every dial works.
- **Views:** SCOPE (renamed from ORBITAL, v0.172) and SKY. **Mercury, Venus, Earth, Mars are shown orbiting the Sun** in their scopes (v0.173), true ellipses, apsides marked, Sun-length noon beams (v0.174, future triggers). SKY for Mercury and Venus is a **top-down true-ellipse scene** (v0.154, v0.161): tail at real length, heat, Sun stall (Mercury), endless AU grid (v0.163). Every named moon in the bay appears in SCOPE and SKY, labelled (v0.149, v0.176, v0.177). The Sun's scope is **multi-coloured**: each planet in its own phosphor (v0.178).
- **Mercury breathes with its orbit (Charlie's rule): aphelion = the fundamental; perihelion = the harmonic range, "heating up"** (v0.158). Now **additive**: 32 sine partials opened like drawbars by orbital position (v0.164), with an audible floor (v0.166). Venus has the same voice.
- **The meter counts oscillators** (v0.168) against a 256 budget. **The keybed plays the selected planet** (v0.167).
- **Defaults while working on Mercury:** only Mercury sounds (v0.155, v0.165); navigator opens on MERCURY (v0.156); FX delay and reverb at 0 (v0.162).
- **Cards are read-only data**, uniform for all nine, and show counts, not names, for moons and rings (the names are kept for Charlie's plans).
- **Colour:** every planet wears its card colour everywhere (orbit, dot, name, beam, keybed dots); pitch colour is retired.

## THE RESYNTH (session 5) — decided
- **Keep this interface, resynth it with the old Orrery's engine** (Charlie). Engine II (v0.200–v0.208, Claude's invented synths and tune) was rejected: the motion of the bodies must make the sound.
- **The bells are the bell system Charlie always wanted** ("exactly what I was always wanting with the thousand year mode"); they sound great at the hourglass ⧗ (365,250×). v0.211 ★ MILESTONE is the fallback.
- **Pitch** (the old Orrery's rule, unchanged): f = 320.3 Hz × √(163.2 d ÷ P), P = the body's own orbital period (planets round the Sun, moons round their planet). 320.3 Hz = keybed centre; 163.2 d = geometric centre of the sky's periods; the √ is the 0.5 interval scale. Inner moons high, outer low; INVERT mirrors it.
- **Pan** (the old Orrery's rule, unchanged): pan = sin(ν) × r ÷ r_max in the body's own orbit; WIDTH scales it. A sky-matched pan (ecliptic longitude) is an idea for a toggle right of the navigator keys one day.
- **Ring time**: high bells shorter, linear per semitone (v0.219).
- **PRESETS** live in their own panel left of the navigator keys: BELLS (a preset), INVERT and FIRST (toggles). No preset system yet — Charlie adds buttons as he goes.
- SYNC stays as it is: one beam from the Sun can't strike every planet at once (Charlie).
- Rejected looks (don't repeat): TRANSPORT/VIEW moved beside the navigator keys (v0.220a); calculator, DYMO, bezel-window and bezel-engraved labels on the Sun view.

## CLOCK MODE (session 6) — decided
- **CLOCK** (own group, far left of the button bar): opens SEQUENCER with the planetary cards, throttle 1:1, sky running, delay 0 (restored on release). Excludes BELLS, FIRST, DRONE.
- **Un-wired:** the card trigger keys no longer play each planet's fixed C. In CLOCK the bell engine's own strikes are off; only the gauges strike, through each planet's bell voice. Moons are silent in CLOCK.
- **Nine clocks, fastest → slowest = the ladder:** arcsec · seconds · arcmin · minutes · degrees · hours · month · year · precession. Each clicks on every tick of its own unit (arcsec every arcsecond, v0.252). Coinciding ticks: the slowest clock sounds (downbeat). The DAYS odometer is not a rung (degrees = days was the clash).
- **Pitch = the clock's own tick rate** (ticks per real second × 128, v0.254), so the throttle is the pitch control: as it climbs, each clock leaves the top of hearing while the next slower rises in from below; pulling toward the halt brings fast clocks down. Audible window fades in 25→60 Hz, out 5→12 kHz; out-of-hearing rungs hand their strike to the next faster audible clock. Each planet runs on its own solar day.
- **Look:** a struck dial's bezel lights; a jewel under 12 o'clock shows each clock's pitch on the rainbow — violet low → red high; black = too low to hear, white = too high (v0.258). The MIDI-number-on-face idea was tried and dropped (v0.254–v0.256).
- **Other modes:** BELLS (opens SKY with moons; latches) · FIRST · DRONE (pitch rides the throttle via the old sweep; INVERT mirrors it — "LOVE"). Throttle handle flashes after the first BELLS/DRONE until touched. WIDTH now lives in the OUT section (FX page) to free the button bar for the next build.

## HANDOFF — next round (continue CLOCK in a new chat)
- **Open in CLOCK:** the note rule beyond tick rate (Charlie floated "when a second ticks, read the arcsec gauge for the note" — routing between clocks); whether moons get clocks; whether coinciding ticks should accent instead of replace; ladder spacing is the dials' real gearing (15×, 4×, 15×, 4×, 15×, 24×…), not octaves.
- **Performance:** CLOCK on the cards is heavy (81 DOM dials). v0.255 helped ~25% headless; if still choppy on Charlie's machine: draw each card's dials on one canvas. Also stop invisible work (hidden sky still draws; silenced PLAN engine still computes).
- **Per-body delay (discussed, not built):** nine planet delay buses into the Sun bus, MOON BAY send per moon, controls in the planet sheet. Clock choice open: fastest orbit (rec.), light-time, own day, beam-to-next-moon.
- **Real moon phases (not built):** only planets have real positions; moons run from an arbitrary zero (Earth's Moon and Galileans had real ephemerides in the silenced engine). JPL mean elements would place ~60 majors correctly. 287 moons in the file, 85 voiced; Saturn's 2025 additions not in.
- **3D Saturn (v0.244) never seen running** — check it first.
- **SKY rings:** log scale distorts widths; Keeler/Huygens/Maxwell gaps not cut in 2D; real 26.7° tilt not applied in 2D.
- Still open from before: step 4 synth deck; card lamps wired to the silenced PLAN engine; FIRST crossing order at high throttle; INVERT moons-only; moon counts (NASA vs MOON_TOTAL).

## Next
- **COMETS** (Charlie, session 4): to be studied as tone generators, living in the top two registers (C8–C9). None are in the sky yet. Candidates with good JPL orbits: Encke 2P (3.3 yr), 67P Churyumov–Gerasimenko (6.4 yr), Tempel–Tuttle 55P (33 yr, Leonids), Halley 1P (76 yr, retrograde), Swift–Tuttle 109P (133 yr, Perseids), Hale–Bopp (~2,500 yr). Ideas: silent far out, flaring near perihelion (sunlight ∝ 1/r²); the tail as a sound that always points away from the Sun; the meteor showers they leave behind as Earth crosses their debris. About 4,000 comets are known; ~500 are numbered periodics.
- **THE REGISTER PLAN** (Charlie, session 3 — decided): moons = motion, so moon count sets the register. Low end simple, activity up high. Moons become note triggers (answers open question #2).
  | planet | moons | role | register |
  |---|---|---|---|
  | Mercury | 0 | sub drone | C1 (live v0.119) |
  | Venus | 0 | sub/bass drone (retrograde spin: counter-motion) | C2 (live v0.120) |
  | Earth | 1 | bass line, driven by the Moon | ~C2 |
  | Mars | 2 | low-mid arp (Phobos fast, Deimos slow) | ~C3 |
  | Jupiter | 57 | mid-range notes; families as phrases, Galilean 1:2:4 as rhythm | ~C4 |
  | Saturn | 63 + rings | pad: rings sustain, moons move within | ~C4–C5 |
  | Uranus | 27 | highs | ~C5–C6 |
  | Neptune | 14 | highs; Triton retrograde counter-line | ~C6 |
  | Pluto | 5 | starlight sparkles in the high keys | C7+ |
  Still to decide: what fires a moon (its own orbit — transit, degree — or the planet's triggers); how pitch is chosen inside each register (orbital distance, period ratios, or a chosen scale/chord).
- **Navigator + ORBITAL** (v0.112): one planet selection drives every view. Candidates: scope persistence as true afterglow; trigger blips flashing on the tubes; scope trace in planet colour as an option; SYNTH/FX pages per planet when they exist.
- **Look** (session 3): the Orrery should look like an old machine (Charlie). Cards done as instruments (v0.087), throttle (v0.098), top bar (v0.099), keys/dots/voices (v0.100); candidates to follow: sky chrome, SYNTH/FX pages in the same language.
0a. **Three precessions** (session 3): apsidal (v0.068, orbit turns in-plane) and nodal (v0.073, tilted orbit plane wobbles) are live. Axial (spin axis cone; drives seasons and the tropical year) is next: rename current "precession" → apsidal, add axial (Earth precise from IAU pole drift −0.641°/−0.557° per century; others estimate), season wheel riding it. Possible: nodal trigger/wheel; inclination on the long-term invariable-plane model.
0. **Precession as clocks** (session 3): apsidal precession is live (v0.068). Candidates: a perihelion-crossing trigger (ORBIT, longest clock per planet); Earth's axial precession (25,772 yr, precise) to drift the zodiac — tropical vs sidereal separating; other planets' axial precession only with estimate flags.
0b. **Layout** (Charlie, session 3 notes): planet cards and synths sit on the starfield/grid background, orbits drawn behind them.
0c. **Zodiac framing** (session 3): signs = ecliptic longitude, one shared 12-spoke ring around the system (ORBIT); houses = each planet's own 12, carried by its spin with the beam as ascendant (SPIN). Constellation backdrop is the same from every planet. Option: Milky Way band (plane ~60° to ecliptic, centre ≈266° ecliptic longitude, in Sagittarius).
1. **The zodiac** — decided (session 3): the real sky, not the ancient signs — 13 IAU constellations, unequal. Odometer on the cards (v0.074); stick figures in the sky (v0.075). Still open: sightlines Sun→planet→band, pitch/rhythm from constellations, aspects as triggers, houses from spin. Earlier notes: (Charlie wants to "get slick" with it; discussion opened at the end of session 2). Ideas on the table: twelve signs ↔ twelve notes (pitch from a shared place in the sky); conjunctions/oppositions as triggers; a visible 12-spoke wheel in the sky; equal vs real (13 incl. Ophiuchus) constellations; tropical vs sidereal.
2. **Delay** (Charlie raised it): the delay time is still the old sequencer's (fastest orbit ÷ rate, halved under 3.9 s, ≈3.1 s at 1:1). Idea: time each planet's echo to its own unit (e.g. its minute or second).
3. **The planetary sheet** (v0.102): built as an interface only. Next: decide destinations for the jacks (family output vs per-moon), and what the four blank synth panels become per planet. **The planetary matrix:** a disclosure button on each card expands it to show the routing matrix for every characteristic on the card, moons included (Charlie, v0.041). Moon roles from the v0.020 milestone return only through it.

## The Sun (master bus) — collecting its parts
- **Master filter** (Charlie, v0.011): the old SYNTH-page Filter on the planets' bus belongs to the Sun module (ask before moving its controls).
- **The FX bus** (ring mod, phaser, flanger, chorus, delay, reverb) the planets feed is the Sun's too.
- Doctrine: the Sun's 5-minute oscillation and 11-year cycle shape the bus; solar distance sets each planet's send.
- The Sun's placeholder card was removed (v0.060); the module is still to be built.

## Maybe
- **Audio-rate triggers** (v0.095): ms (and anything finer) outruns the once-a-frame trigger check. Scheduling blips ahead on the audio clock would let them fire at their true rate, where spin becomes a tone.
- **Deep-time precision** (v0.093): far from now the clock resolves only ~1 s, so arcsecond needles step. A full fix would carry time as two numbers (e.g. whole days + seconds) through every phase calculation.
- **Earth's beam on Charlie's longitude** (Turkey, Texas) instead of Greenwich, so Earth's noon trigger fires at local noon.
- **Default trigger = seconds** instead of degrees (degrees at 1:1 can wait ~25 s for a first blip). Charlie said degrees is OK for now.
- **Below the arcsecond** (thirds, milliarcseconds): at real time spin becomes audio-rate (Earth 902 Hz in thirds/s), i.e. rotation as an oscillator.
- **Pitch selection on every planet module** (Charlie, v0.006).

## Open questions
1. **Architecture:** does each planet get its own legendary architecture chosen by its physics, or one standard rack with only the data differing?
2. **Moons:** trigger notes, or only modulate their planet?
3. **Patching:** physics as the only patch, or re-routable with physics as the default?
4. **Pitch:** nine Cs is a placeholder. Later: one physical rule, or the zodiac.

## Inherited, still in the file (switched off, not deleted)
- The old sequencer engine and its hidden control row (`#ctlPanel`: mode, pitch ratio, timing, pitch, system, strike, tutorial). Its System select (Everything) still keeps every planet in the sky, so delete it only when the engine goes.
- Hidden by CSS: sun menu/strike board, orbital geometry buttons, padlock, pitch ribbon, track list (`renderRack` returns early).
- `spinRings()` (unused since v0.059), sleeping voices, dead `exp-mode` CSS, a tutorial that walks old controls.
- The **[v0.020 milestone](orrery-planetary-synth-v0_020-MILESTONE.html)** keeps the per-moon assignments for reference.
