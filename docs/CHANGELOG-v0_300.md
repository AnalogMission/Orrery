# Orrery Planetary Synthesizer — changelog
## v0.300 — Cards open, toggle gone
- CLOCK view shows the bottom of every planetary card by default; the +/− button on the nameplate is removed. The CLOCK view no longer engages the CLOCK preset (look without hearing).

## v0.299 — Moon keys are clicky keys
- MAJOR MOONS / MINOR MOONS restyled as navigator-style keys. Lit = audible; dark = silent, no glow in SCOPE (dim dot).

## v0.298 — MAJOR / MINOR MOONS
- Two switches right of the planet keys. Major = the 19 round moons (Moon, Galileans, Mimas–Iapetus, Miranda–Oberon, Triton, Charon); minor = all others.

## v0.297 — CLOCK view doesn't auto-start
- VIEW › CLOCK arms the clock without pressing START.

## v0.296 — Title divider
- Thin divider between the title block and TRANSPORT.

## v0.295 — VIEW beside TRANSPORT
- VIEW group sits right after TRANSPORT; SHOW stays flush right.

## v0.294 — One-line header
- Title, TRANSPORT, VIEW and SHOW on a single line (header ~84 → 67 px).

## v0.293 — (superseded)
- Transport offset attempt; replaced by v0.294.

## v0.292 — SEQUENCER → CLOCK view
- The view button is renamed CLOCK and engages the CLOCK preset; leaving the view releases it. Nameplate lamps are indicators only: they flash on clock blips, no steady synth glow, no click-to-mute.

## v0.291 — Top row spread
- TRANSPORT left, VIEW centre, SHOW right.

## v0.290 — Sun logo on SHOW
- A sun logo opens/closes the SHOW menu; hidden by default.

## v0.289 — START → BELLS
- START engages BELLS when no mode is lit (BELLS lives in SKY, where the page opens).

## v0.288 — No pulsing
- Attract animations on BELLS and the throttle removed.

## v0.287 — START → DRONE
- (superseded by v0.289)

## v0.286 — Shift-click solo
- Shift-click a planet key solos it; again = all on.

## v0.285 — Throttle captions
- 1hr, 10kyr …: no space, unit a shade darker.

## v0.284 — 1 s fade-in
- Held (DRONE) voices fade in over 1 s instead of slamming in.

## v0.283 — System balance
- Each system's level × 2.5/√(voices in system): single-body Mercury/Venus no longer buried under moon-heavy systems (within ~3 dB).

## v0.282 — ZODIAC pulled
- Removed from SHOW; band stays off.

## v0.281 — Quiet unmute
- Unmuting a planet in BELLS waits for the next beam instead of striking at once.

## v0.280 — Navigator row layout
- Presets flush left, planet keys centred, INVERT flush right.

## v0.279 — Phosphor negative
- INVERT in SCOPE: black becomes the phosphor colour, glow goes dark.

## v0.278 — INVERT the scopes
- INVERT also inverts the phosphor screens.

## v0.277 — Keys are mutes
- Planet keys truly mute their system (incl. DRONE), with a fast cut.

## v0.276 — SUN toggles all
- SUN turns all keys on, or all off when all are on.

## v0.275 — Weathering tune
- Rust/wear texture refined.

## v0.274 — Keys are switches
- Planet keys are on/off; a muted planet's scope tube goes dead black.

## v0.273 — First-release simplification
- SUN engages every planet; 3D view removed; single-planet views and card nameplate clicks disabled.

## v0.272 — SYNTH / FX into SHOW
- Moved from VIEW to SHOW.

## v0.271 — Darker case
- Case to very dark grey (no green).

## v0.270 — Barn-find weathering
- Procedural rust, pits, grime, chips and worn glass on mounts, panels and bars.

## v0.269 — BELLS off stops
- Releasing BELLS stops the music.

## v0.268 — DRONE opens SCOPE
- DRONE shows the whole system in SCOPE.

## v0.267 — One preset bank
- DRONE · CLOCK · BELLS · 1st in one bank left of the navigator.

## v0.266 — DRONE on the hourglass
- DRONE sets the throttle to ⧗ (365,250×).

## v0.265 — DRONE throttle (superseded)
- First pass at DRONE setting the throttle; replaced by v0.266 (the hourglass).

## v0.264 — CLOCK reverb centred
- Reverb knobs to centre in CLOCK; restored on release.

## v0.263 — Moon pulled in
- Earth's Moon drawn closer to Earth in SKY.

## v0.262 — Blips
- CLOCK strikes are short blips, not bells.

## v0.261 — Planetary seconds
- CLOCK arms the SECONDS trigger only.

## v0.260 — Fixed Cs
- Each planet strikes its own C, Mercury C1 → Pluto C9.

## v0.259 — WIDTH to the OUT section
- The stereo WIDTH slider leaves the button bar (room for what comes next) and sits in the OUT section beside STEREO, restyled flat. Behaviour unchanged. Note: OUT shows on the FX page; the SYNTH page hides it.

## v0.258 — bezel light and the pitch lamp
- A struck clock's metal bezel lights and fades (no halo outside the dial).
- In CLOCK, a jewel under 12 o'clock in every dial shows that clock's pitch: rainbow on a log scale 25 Hz (violet) → 12 kHz (red); too low to hear = black, too high = white. It swells on each strike.

## v0.257 — BELLS opens the sky
- Pressing BELLS switches to SKY and turns SHOW › moons on.

## v0.256 — strike glow replaces the MIDI windows
- The v0.254 MIDI numbers come off the faces; a struck dial glows instead (opacity only, cheap).

## v0.255 — smoother throttle
- Profiled: the choppiness on throttle moves was repainting the 81 card dials. Static dial faces raster once on their own layer; readout numbers update ≤ 11 Hz; CSS containment on gauges and readouts. (~45 → ~33 ms/frame headless.)

## v0.254 — each clock pitched by its own tick rate; MIDI on the faces
- Fix: v0.253 pitched every rung as octaves under arcsec, so the whole ladder left hearing together and the slow clocks never came in. Now each clock's pitch = its own ticks per real second × 128. Rungs keep their order with the dials' real gearing (15×, 4×, 15×, 4×, 15×…); as the throttle climbs each leaves the top while the next slower rises in from below. Earth at 1:1: arcsec 1,920 Hz · seconds 128 · arcmin 32; at 1 hr/s: minutes 7,680 · degrees 1,920 · hours 128.
- MIDI note drawn in each face (removed in v0.256).

## v0.253 — the nine clocks as a ladder
- CLOCK arms all nine dials (arcsec, seconds, arcmin, minutes, degrees, hours, month, year, precession); each clicks on every tick of its own unit. When ticks coincide the slowest clock sounds (the downbeat). A rung out of hearing passes the strike to the next faster audible clock. The DAYS odometer is not a rung.

## v0.252 — arcsec clicks every arcsecond again
- Reverts v0.249 for ARCSEC.

## v0.251 — CLOCK runs dry
- Delay mix to 0 while CLOCK is lit; restored on release.

## v0.250 — the dials as oscillators
- A dial's note = its turning rate × 8192; the throttle raises every note together. Audible window: fades in 25→60 Hz, fades out 5→12 kHz. (Superseded by v0.253/v0.254.)

## v0.249 — one ping per dial turn
- A dial pings when its hand completes a turn (arcsec once an arcminute). (Reverted for arcsec in v0.252.)

## v0.248 — CLOCK
- New CLOCK button group left of PRESETS: opens SEQUENCER (the planetary cards), throttle to 1:1, starts the sky, releases BELLS/FIRST/DRONE (and is released by them).
- Un-wired: the card trigger keys no longer play the planet's fixed C (PLAN engine); in CLOCK the bell engine's own strikes (BEAM etc.) are off — only the gauges strike, through each planet's bell voice; moons silent.

## v0.247 — plain flashes
- Throttle handle flashes on/off (no glow); any throttle move stops it, including clicking an indent mark. BELLS startup flash is a clean two-state blink.

## v0.246 — throttle invitation
- After the first BELLS or DRONE the throttle handle flashes until touched.

## v0.245 — shimmer interval −24
- Shimmer INTERVAL knob −24…+24 semitones; double-click = 0.

## v0.244 — Saturn in 3D (untested in a browser)
- 3D view + navigator SATURN: true-scale system, translucent oblate Saturn, rings as real bands (D C B A F G; Cassini, Encke, Keeler, Huygens, Maxwell gaps) with Kepler ice particles, every named moon on its orbit, tilted to Saturn's real pole, lit from the Sun. Wheel zooms rings → Phoebe.

## v0.243 — DRONE its own group
- PRESETS (bells · first) | DRONE | navigator | PITCH (invert). DRONE excludes BELLS and FIRST.

## v0.242 — ring particles dimmed
- Saturn ring particles ~¼ brightness, smaller.

## v0.241 — Saturn's rings in SKY
- D C B A F G E at NASA radii, brightness from optical depth, Cassini Division and Encke Gap open; ~2,000 particles on their own Kepler laps (C ring ~5.8 h, A ring ~14.3 h); far half behind Saturn; particles fade at high throttle. Log distance scale (widths distorted).

## v0.240 — presets reshuffled
- Left: bells · first · drone. Right: INVERT alone (PITCH).

## v0.239 — DRONE pitch on the throttle
- DRONE uses the old Orrery's sweep (timing HOLD): the whole chord slides with the throttle, faster = higher; release restores BEAM pitches. INVERT mirrors it (a favourite).

## v0.238 — DRONE
- Every planet and moon held (STRIKE › HOLD); latches; takes turns with BELLS.

## v0.237 — gentle joystick
- 3D stick: ~20°/s turn, ~14°/s tilt at full throw, curved response.

## v0.236 — zodiac in 3D
- The 13 constellations on the inside of the sky sphere, ecliptic circle, boundary ticks; lit by the planet in front.

## v0.235 — the 3D view
- VIEW › 3D (Three.js r128 from CDN, loaded on first use): heliocentric sky in true 3D (real tilts, log distance), brass joystick to turn/tilt (double-click = home), wheel zoom. Planets only.

## v0.234 — BELLS latches
- Stays down and lit; press again to release; releases itself when the throttle leaves the hourglass.

## v0.233 — eccentric moons drawn as ellipses
- Scopes: moons with e > 0.1 (Nereid, Hyperion, Phoebe, irregulars) drawn as true ellipses with apsides on the log rings (planet slightly off focus).

## v0.232 — throttle labels; smoother trails
- 30 min and 3 hr labels on the throttle. Eccentric moon trails sampled 90× (Nereid no longer jagged).

## v0.231 — bells · invert · first
- REVERSE renamed INVERT and moved between BELLS and FIRST in the PRESETS panel.

## v0.230 — invert (reverse)
- Toggle: every bell's pitch mirrored about the keybed's centre (320.3 Hz) in log pitch, f → 320.3² ÷ f. Intervals exact, direction flipped: inner moons low, outer moons high; planets flip too (Mercury below Earth, Pluto on top). Remembered.

## v0.229 — thin brass plates
- Sun view: a slim brushed-brass strip under each scope, name engraved and filled black, two rivets (replaces the v0.218 calculator readouts; v0.226 DYMO tape, v0.227 bezel window and v0.228 bezel engraving were tried and rejected).

## v0.226 — the singing ring
- Sun view: a thin ring round each scope in the planet's colour, lit while the planet or any of its moons rings (the Sun's ring lights as its beam strikes). The labels no longer glow.

## v0.225 — bells pulses
- BELLS pulses amber at startup until pressed or until START.

## v0.224 — stereo WIDTH
- A brass slider right of the navigator keys: left = mono, middle (detent, double-click) = the orbit pans as they are, right = pushed hard left/right (power curve toward ±1). Remembered.
- Pan itself (unchanged, from the old Orrery): pan = sin(ν) × r ÷ r_max — true anomaly in the body's own orbit; centre at periapsis. No randomness.

## v0.223 — the sunbeam
- SKY draws the Sun's beam (gold, soft halo) — the line that strikes in BEAM mode. SHOW › sunbeam toggles it (on by default, remembered).

## v0.222 — presets row; singing bodies glow
- BELLS and FIRST move into a PRESETS panel left of the navigator keys, moulded like them.
- Scopes: every body glows (a halo in its tube's phosphor) while its bell sings, flaring on the strike, fading with the decay. Sun tube, planet tubes and the inner four.

## v0.221 — FIRST
- Toggle: one note per planet's system per sweep — as the Sun's beam crosses a system, only the first body it strikes rings; the rest are held until the beam has turned another half revolution. Muted bodies don't take the turn. (At high throttle a whole system can cross in one frame; then the winner is list order.)

## v0.220 — BELLS
- One button for the bell system: navigator to SUN, all mutes/solos cleared (moon levels kept), every planet on BEAM, delay ½ + reverb 6.5 s full, throttle on the hourglass ⧗ (365,250×), sky started.
- (An earlier v0.220 moved TRANSPORT and VIEW beside the navigator keys; Charlie rejected it and it was deleted.)

## v0.219 — high bells ring shorter
- Bell key tracking: the lowest bell in the sky keeps the full envelope (3 s decay, 3 s release); ring time falls linearly per semitone to 15 % at the highest bell. Range re-measured from the bells in the sky each second.

## v0.218 — who is singing (Sun view)
- Calculator-style name readouts under the Sun view's scopes, glowing with their system (replaced in v0.226/v0.229).

## v0.217 — keybed dots in planet colours
- The dots over the keys light in the sounding planet's colour (moons in their planet's); pitch ticks match.

## v0.216 — the strip centred
- The body LED strip sits centred in the voice bar, unlabelled; empty wings either side for future controls.

## v0.215 — one LED per sounding body
- The voice bar: 95 LEDs, Sun → Pluto, each planet followed by its moons by distance; glow in planet colour with the bell, white flash on strike, dark red when muted. The Sun's LED flashes when its beam strikes.

## v0.214 — scope geometry and brightness
- Fix: every point of an orbit now sits at its TRUE distance on the tube's log scale (Nereid's perihelion was drawn inside 100,000 km; it is at 1.37M km). Eccentric orbits sampled by angle.
- Orbits and bodies brighter; graticule, ticks, distance rings and the spin line dimmer.

## v0.213 — labelled distance rings
- Scopes: the unlabelled quarter rings are gone; faint dashed rings at each tenfold distance (moon systems, Sun) or round AU steps (inner four), labelled.

## v0.212 — the datasheet
- Every planet's sheet has a DATASHEET above the MOON BAY (bay now scrolls): BODY · ORBIT · SPIN · ENVIRONMENT (fields all nine share, same order, nine-step rank bars) · NOW · LIVE · ONLY [PLANET] (what the others don't share). From the NASA NSSDCA table already in PHYS; derived values computed.

## v0.211 ★ MILESTONE (saved as -MILESTONE.html) — STRIKE keys
- Each planet's trigger bar gets STRIKE: BEAM (the Sun's beam strikes, default) · RADAR (every body's beam strikes) · PERIAPSIS (once per orbit at closest approach) · HOLD (drone). A switch per planet, applied to the planet and its moons, remembered.
- The bells Charlie wants: the old Orrery's bell voice (sine, 5 ms attack, 3 s decay), pitch from orbital period, ½ delay, 6.5 s reverb.

## v0.210 — the MOON BAY sings
- Every moon with a voice in the engine is a live strip: lamp = mute (shift-click = solo within its planet), fader = level (double-click = unity), glows while its bell rings. Family strip mutes and scales the family. Moons with no voice are dimmed. Remembered.
- Navigator solo brings a planet's moons with it.

## v0.209 — resynth, step 1: the old engine speaks
- The old Orrery's engine (v0.608) is plugged back in (PL_ONLY off) and voices the nine planets; the new planet modules are silent. Rotational Music Box: the Sun's 25.38-day beam strikes each body; delay ½ and reverb 6.5 s back on.
- Fix: the old engine only heard the navigator's selected system (Mercury → silence); it now always hears the whole sky.
- Navigator keys are switches: click = only that planet, SUN = all, shift-click = hold a planet on. Built on clean v0.178.

## v0.200–v0.208 — Engine II (abandoned)
- Claude's rebuild: nine "flagship" synth voices, moon oscillators, a tune. Rejected (the tune was invented, not made by the sky). Not carried forward; only the navigator switches survive into v0.209.

## v0.178 — the multi-coloured Sun scope
- On the Sun's scope each planet glows in its own colour (Charlie's invention): orbit, trail, dot, label and beam in the planet's phosphor; the Sun and its tube stay amber.

## v0.177 — SKY = bay
- SKY draws every named moon (swarms included, unnamed S/ left out), all labelled; drawing only.

## v0.176 — Saturn's small six
- Daphnis, Aegaeon, Methone, Anthe, Pallene, Polydeuces added to the scope.

## v0.175 — Phobos visible
- Moon rings drawn clear of the planet dot; fast moons stay as dim dots.

## v0.174 — Sun-length beams
- Scope beams reach exactly to the Sun: they cross it at local noon (future triggers).

## v0.173 — the inner four around the Sun
- Mercury, Venus, Earth, Mars tubes: Sun at centre, true ellipse with apsides, trail, noon beam; Earth's and Mars's moons scaled up around them.

## v0.172 — SCOPE
- VIEW button ORBITAL renamed SCOPE.

## v0.171 — planet beams on the Sun's scope
- Each planet's noon beam on the Sun's tube.

## v0.170 — zero-size fix
- The tail's 0/0 on a zero-size view (the cause of the dead throttle) fixed.

## v0.169 — the loop can't die
- Non-finite canvas values drawn safely and logged; the main draw guarded.

## v0.168 — oscillator meter
- The meter counts oscillators running (and buffer sources) against a 256 budget, red past 75 %. Additive planets stop their silent saws.

## v0.167 — play the planet
- The keybed plays the navigator's selected planet synth (held, mono; a drone takes the key while held).

## v0.166 — audible floor
- Partials up to ~32 Hz stay open at aphelion (C-1 alone was silent on speakers).

## v0.165 — Venus muted
- Mercury alone again.

## v0.164 — additive
- Mercury and Venus built from 32 sine partials (partial 1 = sine sub); the orbit opens them like drawbars toward perihelion. Saws silenced.

## v0.163 — real tails, endless grid
- Range rings run to the view's corners at any zoom (1-2-5 steps, labelled). Tails at real length: Mercury sodium 3–24 M km, Venus ion ~45 M km, end marked.

## v0.162 — dry FX
- FX delay and reverb mix 0 by default (were 25 % and 100 %).

## v0.161 — Venus too
- The scene and the breath generalised; Venus: cloud disc, evenly hot night, blue ion tail. Venus unmuted.

## v0.160 — no stall caption
- The Sun-stall caption removed; ring and readout row stay.

## v0.159 — magnetosphere out
- Removed from Mercury's scene (Charlie).

## v0.158 — Mercury breathes
- Cutoff from true distance: 18 Hz at aphelion → 4 kHz at perihelion.

## v0.157 — voice readout
- Top-left readout of the live oscillators, filter and state in the Mercury view.

## v0.156 — Mercury selected
- The navigator opens on MERCURY.

## v0.155 — Mercury alone
- Venus–Pluto boot muted.

## v0.154 — top-down
- Mercury's scene seen from straight above (true ellipse undistorted), flat range grid.

## v0.153 — apsides + solo
- Perihelion/aphelion diamonds with distances; shift-click a lamp to solo a planet.

## v0.152 — Sun-centred
- Mercury scene rebuilt equatorial: Sun at centre, Mercury on its real ellipse.

## v0.151 — Mercury, alive
- Mercury gets its own SKY scene (it had none: no moons): sodium tail, heat, magnetosphere, Sun stall.

## v0.150 — moon names on the scope
- Every named moon labelled in the single-planet scope view.

## v0.149 — scope moons = bay moons
- Every named moon in the MOON BAY drawn on its scope (irregular swarms and small inner moons joined).

## v0.148 — MULT drum
- A multiplier window beside the day wheels steps ×1 → ×10³ → … ×10¹⁵ when the wheels fill: no ceiling.

## v0.147 — day odometer
- Back to odometer wheels, eight of them.

## v0.144–v0.146 — day display trials
- LCD, then nixie tubes, then red bubble LED — all rejected. v0.146 also: the brass nameplate opens the planet's machine (was the porthole); the emblem porthole is hidden.

## v0.143 — three rows
- Cards: ORBIT · LOCAL SOLAR TIME (hours, minutes, seconds) · SPIN (degrees, arcmin, arcsec), then a DAYS counter.

## v0.142 — clock faces
- Each hand named for what it counts and turning once per the next unit up (seconds hand once a minute).

## v0.141 — milliseconds retired
- MILLISEC trigger, gauge and old header button removed (Charlie: faster than any frame; a pitch, not a trigger).

## v0.140 — deep-time precision
- Spin carried as whole turns + exact fraction (fmod + the v0.093 carry): dials, triggers, day count, sync and now stay exact after runs hundreds of millions of years out.

## v0.139 — trigger keys are a switch
- Click picks one trigger (others off; click the lit one again = off); shift-click stacks.

## v0.138 — seconds by default
- Every planet armed on SECONDS (degrees took minutes to fire at 1:1); saved trigger settings reset.

## v0.137 — each planet its own voice
- A trigger strikes the planet's own synth instead of a shared sine blip.

## v0.136 — the note on the plate
- The sounding note is engraved on the brass nameplate (held for drones, ~0.7 s after a blip).

## v0.135 — flicker
- Lit lamps flicker like a filament: slow breath, jitter, rare dips.

## v0.134 — Cs from the Sun outward
- Mercury C-1 · Venus C0 · Earth C1 · Mars C2 · Jupiter C3 · Saturn C4 · Uranus C5 · Neptune C6 · Pluto C7. C8–C9 kept for comets.

## v0.133 — two octaves down
- Mercury drone C-1 (8.18 Hz), Venus C0; spin blips two octaves lower; pitch floor 20 → 4 Hz.

## v0.132 — lamps glow
- A lamp burns bright and breathes while its voice is sounding.

## v0.131 — the lamp mutes
- Each card's nameplate lamp is its voice's mute (Charlie): click to silence, click again to bring it back; dark grey when muted. Same switch as the sheet's ON.

## v0.130 — the Sun's black unit
- The Sun's scope gets its own black container (Charlie): a black-anodised plate (the master unit), a brass pinstripe inset around the edge, brass screws, and engraved brass sun rays radiating round the bezel. The nine planet mounts stay brushed steel.

## v0.129 — coloured phosphor
- Each scope's phosphor is tinted in its planet's colour (Charlie): the planet hue lifted to phosphor strength for the trace, graticule and sweep; near-white in that hue for the hot dots; a deep shade of it for the dark screen. The Sun's tube glows amber. Applies to the single full-viewport view too.

## v0.128 — swappable instruments
- Each ORBITAL scope is now bolted into its own square mount, like an avionics gauge (Charlie): a bevelled, brushed-steel plate seated in a dark panel cut-out, four slotted screws at the corners (each turned its own way), a shadowed recess for the round bezel, and a riveted brass nameplate engraved with the name under the dial. The single-planet view stays full-viewport.

## v0.127 — trigger names spelled out
- The sheet's trigger keys read in full (Charlie): PRECESSION · YEARS · MONTHS · DAYS · HOURS · DEGREES · MINUTES · ARCMIN · SECONDS · ARCSEC · MILLISEC.

## v0.126 — triggers in the workspace
- Each planet's TRIGGERS move off its card and into the top bar of its sheet (Charlie), one row centred between the nameplate and ✕, above the synth controls and the moon bay. Drones show DRONE · Cn beside the keys.
- Fix: the sheet's count line is singular when it should be ("1 MOON · 1 NAMED · 1 FAMILY").

## v0.125 — spaced controls
- More room between TRANSPORT, VIEW and SHOW (Charlie): 34 px either side of an engraved divider between each group.

## v0.124 — the navigator panel
- The planet keys leave the header for their own enamel panel directly under the throttle, above the workspace and viewport they drive (Charlie). The header is back to one row: logo, then TRANSPORT · VIEW · SHOW.

## v0.123 — one control row
- The second header row is now TRANSPORT · VIEW · SHOW, centred, left to right (Charlie). The logo keeps the top left on its own; the planet keys stay centred on top.

## v0.122 — navigator on top
- Swapped (Charlie): the navigator's planet keys now sit at the top of the screen, centred in the header's first row; the VIEW buttons (SYNTH · FX · SEQUENCER · SKY · ORBITAL) moved down into the centred row beneath, where the keys were.

## v0.121 — the navigator walks the synths
- **On SYNTH, the planet keys step through each planet's synth** (Charlie): a planet key shows that planet's synth alone, full width with big knobs (SOURCE · SHAPE · AMP · TO THE SUN · PHYSICS). **SUN** shows the original SYNTH page, the master voice (the Sun's bus). Switching between SEQUENCER and SYNTH keeps the selected planet: SEQUENCER shows its full sheet, SYNTH its synth.

## v0.120 — Venus up an octave
- Mercury drones on **C1** (32.7 Hz), Venus on **C2** (65.4 Hz) (Charlie). The cards read DRONE · C1 and DRONE · C2.

## v0.119 — voices begin: drones, per-planet triggers, a synth per planet
- **Mercury and Venus drone on low C (C1, 32.7 Hz)** (Charlie): the sub. With START they hold a sustained note through their own voices (Osc 2 at each planet's orbit÷rotation ratio, filter, Drive/Atmos); they no longer spin-blip. Their cards read DRONE · C1.
- **TRIGGERS move onto each sequencer card** (Charlie): the header trigger bar and its nine-hand rotators are retired. Every card carries its own strip of trigger keys (PRE · YR · MO · DAY · HR · DEG / MIN · ′ · SEC · ″ · MS), lit amber when armed, remembered per planet. Defaults: degrees for Earth→Pluto, nothing for the two drones.
- **Each planet's sheet is now its synth page** (Charlie): SOURCE (Osc 2 · Drive · Atmos), SHAPE (Cutoff · Res · Speed→Cut), AMP (Attack · Release · Light→Amp), TO THE SUN (Spin→Pan · Level, plus ON and DRONE switches) are working knobs on that planet's voice: drag up/down, double-click to reset. Planets with moons get a fifth panel, PHYSICS, with their own links (e.g. Jupiter: Io→Ring, Europa→O2, Ganymede→Cut, Callisto→Amp, Rings, Swarm); these start at 0 since v0.021's clean slate.
- Unchanged for now: Earth→Pluto still blip on the nine Cs (placeholder until the register plan below is built).

## v0.118 — SEQUENCER
- The VIEW button PLANETS is renamed **SEQUENCER** (Charlie): it is the orbital sequencer. Same page, same key (P).

## v0.117 — transport under the logo
- TRANSPORT (START · PANIC · REC · now · sync) moves down below the logo (Charlie): the left column now stacks logo, transport, SHOW, all on one left edge.

## v0.116 — brass-ringed navigator
- The navigator's black well is ringed in brass, the same ring as the throttle's slot (Charlie).

## v0.115 — breathing room
- More space between the navigator keys and the voice bar (Charlie): the navigator row gets 12 px below it (was 2).

## v0.114 — steady phosphor
- **No glow, no flicker** (Charlie): the scopes drop every glow halo and the spin sweep's fading wedge (a single thin line now). Nothing blurs like the gauge needles: anything turning too fast to follow (the sweep, a moon's dot and trail) fades out smoothly between 0.5 and 2 turns a second, leaving its orbit line.
- **A single planet fills the viewport** (Charlie): no bezel or round tube; the phosphor screen, graticule, crosshair and scanlines run edge to edge, with the planet's name in phosphor at the top left. The 10-up keeps its round tubes.

## v0.113 — navigator row
- The navigator keys are now exactly the planet-sheet keys (Charlie): wide moulded keys with symbol and full name, in their planet colours, the current one down and lit. They sit on their own new row across the header, centred in a black well. Behaviour unchanged from v0.112.

## v0.112 — the navigator and the orbital scopes
- **Navigator** (Charlie): ten clicky planet keys, SUN first, in the centre of the top bar, moulded in their colours; the current one stays down and lit. One selection drives whatever is showing:
  - **Deck (PLANETS):** SUN = the PLANETS mixer; a planet = its sheet. The porthole, ✕ and Esc go through the navigator too.
  - **SKY:** SUN = the whole sky; a planet = that planet's own equatorial system view (Mercury and Venus have no moons, so they keep the whole sky).
  - **ORBITAL:** SUN = all ten scopes; a planet = its scope alone, full size.
- The planet keys left the sheet's own top bar (the navigator replaces them).
- **ORBITAL view** (new, beside SKY in VIEW): two rows of five round phosphor CRTs set in the enamel panel: brass-rimmed steel bezels, green phosphor, graticule rings and crosshair, degree ticks, scanlines, curved-glass vignette and glint, engraved labels. Top-down and live: the Sun's tube shows the nine planets on log-scaled orbits (labelled); each planet's tube shows its moons on their real Kepler orbits. Every body leaves a short phosphor trail; the centre body's spin sweeps the tube like radar at its real rotation (backwards for Venus, Uranus, Pluto); a bright mark on each planet's rim points to the Sun; Saturn shows a ring band. Click a tube to bring it up alone; click the single tube to return to all ten.

## v0.111 — coloured keys
- The planet keys lose their jewel dot; each key is now moulded in its planet's colour, with cream lettering (Charlie). The open planet's key stays down and lights up in its own colour with a glow.

## v0.110 — SHOW under TRANSPORT
- The SHOW row now starts in line with the TRANSPORT caption instead of flush left under the logo (Charlie); it keeps the alignment on resize.

## v0.109 — porthole returns
- In the expanded sheet, clicking the planet's porthole on its card (beside ARCSEC/MILLISEC) closes the sheet and returns to the PLANETS view (Charlie). ✕ and Esc still work.

## v0.108 — clicky planet keys
- **Every family on the moon console opens by default** (Charlie); the group masters still fold their strips.
- **Planet selector centred in the sheet's top bar** (Charlie) as a row of bakelite push-keys in a black well: each key carries a jewel in its planet's colour, the planet's symbol and its name; keys sink when pressed, and the open planet's key stays down, lit like an amber lens.

## v0.107 — the moon console
- **MOON BAY is a mixing console** (Charlie): moons run left to right, one vertical channel strip each — lamp, live orbit dial, name engraved vertically (major moons bold), period, a fader (not wired) and an output jack at the foot.
- Each family is a **group master strip** in the planet's colour (brass fader cap, brass group jack) with its moon strips to its right. Click a master to fold its strips away; families of 8 or fewer open by default, the big irregular clouds (e.g. Norse, Ananke, Carme, Pasiphae) start folded. The console scrolls sideways.
- Family description, distance span and unnamed count moved to the master strip's tooltip; each moon's details are on its strip's tooltip.

## v0.106 — throttle toggle
- The brass THROTTLE plate is gone (Charlie). Instead, **throttle** is a toggle at the end of the SHOW row: on by default; off hides the throttle and the workspace takes the room.

## v0.105 — the brass plate
- **THROTTLE** moved to the centre of the panel, engraved into a small brass nameplate above the slot (Charlie).

## v0.104 — THROTTLE
- The rate slider is labelled **THROTTLE** (Charlie), engraved in cream B612 at its top left like the top-bar captions.

## v0.103 — the sheet in the workspace
- **The planet sheet is no longer a popup** (Charlie): it opens in the workspace below the throttle, in place of the planet card row, and the sky and keybed stay below it. Closing (✕ or Esc) brings the card row back.

## v0.102 — the planet sheet
- **Click any planet's porthole** and its machine opens over the whole deck (Charlie); the throttle stays in reach above it. Close with ✕ or Esc; a row of portholes at the top right jumps between planets.
- **Left:** the planet's instrument card, unfolded.
- **Top right:** four blank synth panels (SOURCE · SHAPE · AMP · TO THE SUN) with dead knobs marked NOT WIRED.
- **MOON BAY:** every named moon, grouped by family. Saturn: Shepherds, Co-orbitals, Alkyonides, Trojans, Major, Inuit, Gallic, Norse. Jupiter: Inner, Galilean, Themisto, Himalia, Carpo, Valetudo, Ananke, Carme, Pasiphae. Uranus: Inner, Major, Irregular. Neptune: Inner, Triton, Nereid, Irregular. Pluto: Binary, Small. Earth and Mars: Major. Mercury and Venus: the bay stays dark.
- Each family row folds open (Major and Galilean open by default) and shows a one-line description, distance span, named count (+unnamed), retrograde count, a lamp and a brass family output jack. Each moon shows a lamp (lit on the near side of its orbit), a live orbit dial on its real period (backwards for retrograde moons), period, distance and an output jack. **Nothing is patched;** the jacks have no destination yet.
- Unnamed provisional moons (S/…) are counted per family, not listed.

## v0.101 — moons in the porthole
- **Every moon in the data now orbits inside its planet's emblem porthole** (Charlie): real positions from each moon's Kepler orbit (same solve() as the sky), the orbit plane seen nearly edge-on (Saturn and Uranus on their ring tilt). On the near half a moon passes in front of the planet; on the far half it slips behind the disk and dims. Distance is log-scaled from the limb to the rim; dot size from mass; major moons cream, small ones dimmer.

## v0.100 — keys, dots and voices
- **Same instrument style as the top bar** (Charlie). Voice meter: jewel lamps (dark lens off, amber lit with glow, white-hot on a strike) set in a black bezelled well; the count engraved in cream B612 Mono. Dot strip: a recessed black lamp rail; every dot a jewel lamp with bezel, glint and a glow in its planet colour. Keybed: black bakelite keys on the enamel panel, lit from above with a dished front lip; sharps glossy black casting a shadow; C labels engraved cream; a brass rail along the top; frequency ticks glow in planet colour. Sizes, layout and key hit-zones unchanged.

## v0.099 — the control panel
- **Zodiac** off by default (Charlie); the SHOW toggle brings it back.
- **Top bar in the instrument style** (Charlie): enamel panel; captions and logo engraved in cream B612; every button a black bakelite push-key with cream lettering, sinking when pressed; a key that's ON lights as a backlit amber lens; START a brass key; PANIC red bakelite; the trigger rotators set in steel bezels; the voice bar an engraved strip. Sizes and layout unchanged.

## v0.098 — the throttle
- **Orbit needles blur** (Charlie): PRECESSION, YEAR and MONTH fade to the spinning blur when they turn faster than ~3 turns a second, like the spin needles.
- **The throttle:** the rate slider is restyled as part of the machine: an enamel panel with screws, a recessed slot with a brass rim, a ridged brass lever handle, and the scale engraved in cream B612 Mono (the nearest mark lights gold).
- **Always under the voice bar** (Charlie): the throttle now sits directly below the voice bar on every page (on PLANETS it used to sit below the cards).

## v0.097 — the top of the dial is the trigger
- **Needles trigger only at the top** (Charlie). Every card needle now shows progress through its own unit and crosses 12 o'clock exactly when that unit's trigger fires; the number under it is the count. Faces re-divided to match: DAY 24 h · HOUR 60 min · DEGREE 60′ · MINUTE 60 s · ARCMIN 60″ · SECOND 15″ · ARCSEC 1000 mas · MILLISEC 15 mas. The top-bar rotators work the same way.
- Needles too fast to follow (over ~3 turns a second, e.g. ARCSEC and MILLISEC at real time on Earth) fade to a spinning blur, like a propeller, instead of strobing.
- **SYNC** now puts every needle at the top and sounds every planet once (the downbeat), even with no trigger toggled on. Spin needles: spins to noon, as before. Orbit needles (PRECESSION, YEAR, MONTH): their clocks are re-zeroed at each planet's place at that moment; the orbits don't move, and the orbit triggers count from the sync. MONTH now reads "MONTH n" since the sync (it was SIGN n from the equinox). The constellation drum is unaffected.
- **now** clears the orbit offsets: years and months count from the J2000 equinox again.
- Correction to v0.095's notes: the top-bar ms hand was never changed; it always showed the true trigger hand.

## v0.096 — breathing room
- Fix (Charlie): the DIST · AU / SPEED · km/s / SUN · × captions butted against the counter windows' bezel rings, and CONSTELLATION against its screen's bezel. Both now sit clear below them.

## v0.095 — milliseconds
- **ms** trigger, last in TRIGGERS · SPIN, with its nine-hand rotator: one blip per millisecond of each planet's hour angle (15 milliarcseconds of spin). Its hands show the millisecond within the second (one turn a second), since a hand turning 1000× a second would only strobe.
- Note: at real time on Earth that is 1000 blips a second, faster than the screen; triggers are checked once a frame, so ms behaves as a steady pulse at the frame rate on most planets.
- **MILLISEC** gauge on every module, beside ARCSEC (0–1000, ten majors): needle and counter show the ms within the current second. The emblem moves to the right of it.

## v0.094 — indicator lamps
- Each module's nameplate lamp now sits dim and flares bright (white-hot centre, glow in the planet's colour) every time that planet's trigger fires a note, fading over about half a second, like an indicator bulb (Charlie). Lamps only flash when sound is running (START).

## v0.093 — the frozen-sky fix
- The real cause of "stops right here" (Charlie): a run to the far right puts the clock ~100+ million years out (≈5×10¹⁵ s). A double can't hold a fraction of a second at that size, so each frame's small step (1/60 s at real time) vanished and the sky froze at any slow rate. v0.092's slider change was not the cause.
- The time step is now compensated (Kahan): the lost fraction is carried and added back, so time always advances — in steps of the clock's resolution (≈1 s that far out; finer nearer now). **now** returns to full precision.
- Known limit: far from now, the fastest needles (arcseconds) step rather than glide.

## v0.092 — slider fix
- Fix (Charlie): dragging all the way right and then back left stopped the thumb just short of 1:1. The 1:1 detent was moving the thumb under the pointer mid-drag, and Safari dropped the drag. The detent now only affects the rate while dragging (100–125 = real time); the thumb settles onto the 1:1 mark when released there. A full right-then-left drag now reaches stop.

## v0.091 — smooth stop
- Restores stopping, as a glide (Charlie): from the far left of the slider up to just short of 1:1, the rate eases continuously from stopped to real time (rate = (pos/100)^1.5), so the arcseconds wind down to a halt. A "stop" mark sits at the far left.
- A small 1:1 detent (pos 100–125) still snaps to real time, so clicking the thumb at 1:1 doesn't slow the sky.
- (v0.076 had removed the halt without Charlie's go-ahead.)

## v0.090 — emblems
- The spare cell beside ARCSEC holds each planet's emblem: the planet painted in a brass-ringed porthole on a starry black field, with its name and astronomical symbol (☿ ♀ ♁ ♂ ♃ ♄ ⛢ ♆ ♇) engraved beneath. Mercury cratered grey, Venus cloud bands, Earth blue with land and ice caps, Mars rust with a polar cap, Jupiter belts and Great Red Spot, Saturn with rings, Uranus tipped on its side with its rings near vertical, Neptune deep blue with a dark spot, Pluto with its heart. Static SVG, drawn once.

## v0.089 — coloured modules
- Each card's enamel panel takes its planet's colour (38% planet colour mixed into the dark enamel), so the nine read as different modules in one rack. Older browsers without CSS color-mix fall back to the grey enamel.

## v0.088 — smooth gauges
- **No dial repaints.** Each dial face is drawn once; the needle and brass hub are separate layers turned by a CSS transform. v0.087 rewrote the needle inside each SVG, repainting 90 dials every frame.
- **No strobing.** Each needle now points at the value written under it, on that dial's own scale: hour on a 24 h face, degree on 360°, minute / arcmin / second / arcsec on 60. v0.087's needles ran one unit finer (the arcsecond needle spun ~15 turns a second at 1:1 on Earth). The fastest needle is now ¼ turn a second at real time.
- DAY's needle: the planet's place in its year (once per orbit, from perihelion); its counter: days since the page opened.

## v0.087 — the cards become instruments
- Every planet card is now a vintage instrument module, from the approved mockup, sized to the existing card space (~187 px wide; fits above the rate slider at 1440×800 and up):
  - hammertone enamel panel with screws; brass nameplate with the planet's colour as an indicator lamp; the fold + as a small knob;
  - odometer wheels for distance (AU), speed (km/s) and sunlight (×), the last wheel turning over at the end like a real counter;
  - constellation name drum in a recessed screen with index arrows;
  - centre-zero SEASON meter (S ← 0 → N; reads NONE with the tilt for Mercury, Venus, Jupiter);
  - ORBIT gauges (precession, year, month) and SPIN gauges (day, hour, degree, minute, arcmin, second, arcsec): graduations, zero index, needle in the planet's colour with counterweight, brass hub, glass glare; value engraved under each.
- Needles show progress through their unit (the same hands as the top-bar triggers); values show the count.
- Type: B612 / B612 Mono (Airbus cockpit typeface), loaded from Google Fonts.
- The old text rows still run, hidden; fixed data under the + restyled to the panel.

## v0.086 — SHOW under logo and transport
- Undoes v0.084–85's layout (which pushed TRANSPORT right): logo/title and TRANSPORT side by side where they were, and SHOW (caption inline) in one compact row beneath both. VIEW and TRIGGERS follow as before. Checked at 1183 and 1920 px.
- Below ~1600 px wide, TRIGGERS still wraps to a second line (unchanged from before v0.084).

## v0.085 — compact SHOW
- Fix for v0.084: the SHOW buttons kept their full 30 px header size under the title, making the left column wide and tall and shoving TRANSPORT/VIEW across (only tested at 1920 px; bad at ~1180). Now small (20 px) buttons in a tight single row, so the title column stays narrow.
- Note: below ~1600 px wide the TRIGGERS group still wraps to a second line (as before v0.084).

## v0.084 — SHOW under the title
- The SHOW group now sits under the logo and title (Charlie): two rows on the left — ORRERY / PLANETARY SYNTHESIZER, then SHOW (keys · dots · names · moon names · moons · beams · zodiac · to scale) in a single row. TRANSPORT, VIEW and TRIGGERS follow to the right as before.
- Fix: the version in the title had been stuck at v0.070 since v0.071; it now reads the current version.

## v0.083 — moons off
- Moons are no longer drawn in the sky by default (both heliocentric views). **moons** toggle in SHOW brings them back; "moon names" only shows when moons are on. Drawing only: moon data and modulation are unaffected.

## v0.082 — hairline breaks
- Perihelion/aphelion breaks narrowed from ~10 px to ~4 px (Charlie: just enough for a beam to slip through).

## v0.081 — breaks, no dots
- The perihelion/aphelion dots are gone (Charlie: they read as planets). Each apsis is marked only by a ~10 px break in the orbit line, the same size on every orbit (the segments touching each apsis are trimmed, not skipped).

## v0.080 — apsis dots
- Shading softened (Charlie: aphelion was hard to see): aphelion now ~42% of perihelion's brightness (was ~12%), and the whole orbit brighter.
- A dot at perihelion (larger, brighter) and at aphelion (smaller, dimmer), each with a short break in the orbit line around it.

## v0.079 — orbit shading
- Each planet's orbit is brightest (and a touch thicker) at perihelion and fades toward aphelion, in its card colour. Shaded by place in the orbit (true anomaly), not by 1/r², so near-circular orbits show it too; the bright side turns with apsidal precession.
- Sky view in every geometry (circles, to scale); the top-down view in true/to-scale geometry.

## v0.078 — beams off
- The planets' beams (v0.043 noon lines) are no longer drawn by default (Charlie: no longer necessary). **beams** toggle in SHOW brings them back. Drawing only: spin, triggers and the day count still measure from the Sun exactly as before.

## v0.077 — cards fold
- Everything that isn't motion (ORBIT, SPIN, BODY, RINGS, MOONS and the data source line) is folded away by default.
- A small **+** at each card's top right opens that card's fixed data (becomes **−**); each card folds independently.

## v0.076 — smooth dials, no halt
- The planet-module tick (card readouts and wheels, trigger rotators, trigger detection, audio parameters) now runs every animation frame instead of every 50 ms (20 fps), which made the dials step visibly at slow rates (1:1–1 min). A 50 ms fallback keeps triggers running in a hidden tab.
- **Halt removed** (Charlie): the stop sign is gone and the slider's left end snaps to 1:1. The slider can no longer stop the sky (START/transport unchanged).

## v0.075 — stick figures
- **Zodiac band** in the equatorial sky view: the 13 ecliptic constellations drawn as stick figures (about 140 bright stars, hand-entered J2000 positions converted to ecliptic), with the ecliptic line, IAU boundary ticks and names.
- Fixed on screen, a backdrop: the stars are directions, so the band holds its size at any zoom (all 13 always in view; outer orbits can pass in front).
- Longitude around the band; ecliptic latitude lifts a star off the floor (compressed so the figures hold together).
- A constellation with a planet in it (seen from the Sun, same as the card odometer) lights in that planet's colour.
- **zodiac** toggle in SHOW (on by default).

## v0.074 — constellation odometer
- New live row **constellation** on every card: a three-line window (previous · current · next), rolling upward continuously as the planet crosses each constellation; the current name is in the planet's colour and crosses the centre line halfway through it.
- The sky, not history (Charlie): the 13 real constellations along the ecliptic, IAU 1930 boundaries, in J2000 ecliptic longitude (Ophiuchus 247.7–266.3°; Scorpius only 6.6°, Virgo 43.7°). Our longitudes are J2000, fixed to the stars, so no precession offset.
- Seen from the Sun (heliocentric). *Approximation:* by longitude only; a planet far off the ecliptic (Pluto, up to 17°) can actually sit in a non-zodiac constellation.

## v0.073 — tilted orbits, nodal precession
- Orbit paths and planets in the equatorial sky view are lifted off the floor (the J2000 ecliptic) by each orbit's real inclination; moons ride their planet's height. Pluto 17.1°, Mercury 7.0°, Venus 3.4°, Saturn 2.5°; Earth lies flat (it defines the floor).
- Each ascending node Ω turns at its JPL rate (Standish table, deg/century), so the tilted orbits wobble around at high speed: Mercury −0.125, Venus −0.278, Mars −0.293, Jupiter +0.205, Saturn −0.289, Uranus +0.042, Neptune −0.005, Pluto −0.012.
- *Estimate flag:* inclination held at J2000 (its fitted linear drift only holds for centuries; the real long-term motion circles the invariable plane). Node rates fitted for 1800–2050.
- Drawing only: audio and triggers unaffected. Top-down view unchanged (height doesn't show from above).

## v0.072 — trigger grains in the card listing
- The v0.071 clock strip atop each card is removed (Charlie: they belong in the listing).
- Live section now lists every trigger grain, slowest first, each with a wheel: precession (ϖ°, ↺ backwards) · year (orbits since open) · month (sign 1–12 · degree in sign) · day · hour · degree · minute · arcminute · second · arcsecond. New rows' wheels are the same hands as the top-bar rotators; the existing day/degree/arcminute/arcsecond wheels are unchanged.
- ORBIT section: "perihelion at" row removed (now the live precession row); rate kept as "precession rate".

## v0.071 — precession trigger, card rotators
- **precession** trigger, first in TRIGGERS · ORBIT (slowest of all): blips when a planet's perihelion longitude crosses a whole turn (0°, the J2000 equinox). Off by default. Its nine-hand rotator runs backwards for Saturn, Neptune, Pluto.
- **Card clocks:** under each planet's name, the ten trigger rotators with that planet's hand only (prec · yr · mo | day · hr · deg · min · ′ · sec · ″), identical to the top-bar hands. The older day/degree/arcmin/arcsec row gauges stay.

## v0.070 — perihelion dial
- A dial beside "perihelion at", hand in the planet's colour, pointing the way the orbit's perihelion points in the sky (0° = right, counterclockwise; 90° up). Turns slowly clockwise-backwards for Saturn, Neptune, Pluto.
- The JPL rate moved to its own row, "precession" (°/century, ↺ backwards), so the dial fits the card.

## v0.069 — perihelia on the cards
- **"perihelion at"** row in every card's ORBIT section: current longitude of perihelion ϖ (deg, from the J2000 equinox) and its JPL rate per century; ↺ for Saturn, Neptune, Pluto.
- Live seasons (Mars Ls, Neptune, Pluto) and Pluto–Neptune 3:2 resonant angle now use the turning ϖ(t), not the fixed J2000 value, so they stay in step at high speed.

## v0.068 — perihelia turn (session 3)
- **Apsidal precession.** Every planet's longitude of perihelion ϖ now advances at its rate from the JPL table already used for the positions (Standish 1800–2050, deg/century): Mercury +0.1605, Venus +0.0027, Earth +0.3233, Mars +0.4444, Jupiter +0.2125, Saturn −0.4190, Uranus +0.4081, Neptune −0.3224, Pluto −0.0406. Saturn, Neptune and Pluto turn backwards. *Estimate flag:* fitted for 1800–2050; approximate over millennia.
- Mean longitude keeps its own clock, so M = L − ϖ(t); positions, years/months triggers and solar-day spin all follow the turning orbit with no jump.
- **"to scale" button** in SHOW (next to moon names): linear AU with real ellipses, where the turning shows. Off = circles as before.

## v0.000

*Predecessor history: Orrery orbital sequencer, CHANGELOG-v0_608.md and earlier.*

**Session 1 — 6 Oct 2026 (Opus).** The project forks from Orrery v0.608. The direction was set (see README): planets as synths, moons as modulators, a JPL-data mod matrix per body, the Sun as master bus, and a rack rebuilt from legendary analog modules. Nothing was listened to. All checks were headless.

---

### v0.000 — Fork from Orrery v0.608 (via v0.609)
- **X mode removed** (Orrery v0.609): the Music of the Spheres room and its audio graph, the logo-click X mode with its red flash and "X MODE" overlay, and the related CSS and keyboard guards. The logo click is now inert. Some `exp-mode` styling remains dead in the file, unreachable and harmless.
- **Bell room removed** (v0.609): the "A Thousand Years" bell room and the hourglass Sun-click easter egg. The ordinary **"A Thousand Years" scene is kept**.
- The file went from 603 KB with 3 scripts to 530 KB with 1 script.
- **Renamed** to **ORRERY PLANETARY SYNTHESIZER v0.000** in the header and the tab title.
- Verified with `node --check` and a headless load → START → logo click → Space, with no page errors.

### v0.001 — PLANETS page; Mercury, the first planet synth
- **Fifth rack page, PLANETS** (button under the logo, key **P**): nine modules left to right, Mercury → Pluto, with the Sun (master bus) at the end. Only Mercury is built; the others show their moon count and "not built yet".
- **Mercury module:** its own audio graph into the main mix. While **On**, it plays Mercury's strikes in place of the shared patch (hooked in `audioNoteOn`/`audioNoteOff` through `plTakes`). Code: `PHYS`, `PL`, `PLAN`, `plBuildUI`.
  - **Voice:** two sawtooths a 3:2 fifth apart (its spin–orbit resonance), a 24 dB lowpass, and a VCA. **Drone** is on by default (no moons to strike it): the gate is held open while Mercury is in the sky and the transport runs. With Drone off, strikes use attack plus ring-out.
  - **Physics → sound, live from the Orrery clock:** orbital speed (vis-viva, 38.9–59.0 km/s) sweeps the cutoff ±1.6 oct; sunlight (∝ 1/r²) moves the amplitude; spin (58.6-day sidereal rotation) moves the pan.
  - **Defaults:** low cutoff from the dark albedo (0.068), and a wide sweep from the highest eccentricity.
  - **Readouts:** distance, speed, sunlight, spin, live cutoff.
  - **Data:** NASA NSSDCA Mercury Fact Sheet (updated 11 Jan 2024), retrieved 6 Oct 2026; source kept in `PHYS.Mercury.src`.
- Rack buttons tightened to fit five.
- **Known:**
  - Mercury's LED on the voice meter doesn't light while the module plays.
  - The drone takes its pitch from the scene's Mercury voice, clamped to 20 Hz–8 kHz.
  - Module settings are not yet saved in patches or scenes.
- **Checks:** headless at 1190 and 1500 px, a layout sweep from 1000 to 1950 px, PANIC rebuilds the module on the new context, and Drone and On toggles throw no errors. Mercury's drone measured −26 dB RMS. Not listened to.

### v0.002 — PLANETS page on its own; thin sliders
- With PLANETS open, the sky, tracks, ribbon and keys are hidden (`body.pl-only`, set in `rackSyncBtns`). The page fills the window, with the rate slider below it.
- Module sliders are now a 2 px track with an 8 px thumb (Safari and Firefox).
- The Mercury card is fixed at 210 px wide.

### v0.003 — Old synth unplugged
- **`PL_ONLY = true`:** the old shared synth no longer reaches the output. In `buildChain`, `g.lvl` isn't connected to `mix`. The old voices still run silently, so the sequencer, the meter and the pitch still work.
- **Planet modules bypass the old FX bus** (ring mod, phaser, flanger, chorus, delay, reverb, and the scene trim). They go straight into the output stage: drive → soft comp → limiter → master.
- **Only built planets make sound.** For now, that's Mercury.
- **Cutoff key-tracks.** The Cutoff knob is set at C3 and follows the note. Before this, a 436 Hz drone under a 240 Hz cutoff was nearly silent.
- **Levels at master** (Everything scene, 1 day/s): Mercury's drone measured −24 to −26 dB RMS, peaks −16 to −19. With Mercury off, the output is silent.

### v0.004 — Double-click a planet slider to centre it
- Applies to every slider on the planet modules. Log sliders (Cutoff, Attack, Release) centre on their log midpoint: Cutoff 600 Hz, Attack ~89 ms, Release ~450 ms.

### v0.005 — Voice meter given room
- The voice bar is 24 px tall (was 10), with 4 px of padding at the top, so the "n / N voices" count no longer touches the top bar.

### v0.006 — Honest meter, again
- The voice meter was still counting strikes on the 72 unplugged (silent) old voices. Under `PL_ONLY`, `voiceAudible` now counts only bodies played by a planet module, and a drone counts while the transport runs. Everything scene: 1 / 73 with Mercury on, 0 with it off.

### v0.007 — Venus; the first universal rules
- **Venus module** built from the NASA NSSDCA Venus Fact Sheet (updated 11 Jan 2024), retrieved 6 Oct 2026.
- **Universal rules** (`PHYS` comment block). The same physics drives the same parameter on every planet:
  - **Osc 2 interval = orbital period ÷ sidereal rotation.** Mercury gets exactly 3:2, a fifth. Venus gets 0.925, about 136 cents below: a slow, beating, sour interval, sitting below because Venus spins backwards.
  - **Speed → cutoff and sunlight → amp are scaled by each orbit's real variation**, no longer stretched to full range. Venus (e 0.0068) barely moves; Mercury still sweeps about −0.7 to +1.0 of its range (was ±1).
  - **Spin → pan.** A retrograde spin pans the other way (↺ in the readout).
  - **Pressure → Drive and Atmos.** These are two new stages on every module: a tanh WaveShaper before the filter, and the planet's own convolution room. Vacuum Mercury defaults to 0 / 0; 92-bar Venus to 70% / 65%.
- **Venus defaults:** cutoff 2.2k @C3 (brightest albedo, 0.77), res 2, attack 900 ms, release 4 s, drone on.
- The module description line is generated from the data (moons, Osc 2 interval, retrograde, e, albedo, pressure).
- **Measured** (Everything, 1 day/s): Mercury −25.7 dB RMS, Venus −28.4 dB RMS at the module output; both together −21.6 dB RMS / −12.2 dB peak at master. No errors. Not listened to.

### v0.008 — Planets into the old FX bus
- **All planet modules now sum into `plBus()`, which feeds `mix`.** From there the signal runs through the full old FX chain: ring mod → phaser → flanger → chorus → delay → reverb → output stage. The FX page controls the planets again.
- **`plBus` cancels the old 73-voice bus trim (`BUS_TRIM`) and the scene trim**, so the planets arrive at their own level. It's rebuilt after PANIC.
- **Measured** (Rotational Music Box scene, reverb 100% wet, Mercury + Venus): −26 dB RMS / −16.4 dB peak at master, and the same after PANIC. No errors.

### v0.009 — Earth and the Moon
- **Earth module** from the NASA NSSDCA Earth Fact Sheet (updated 15 Nov 2024); **Moon** from the Moon Fact Sheet (updated 11 Jan 2024). Both retrieved 6 Oct 2026.
- **`plLunar(jd)`: real Sun and Moon mechanics** (main terms of Meeus' lunar theory). It gives Sun and Moon longitude, the Moon's latitude (the nodes), the Moon's distance, the Sun's distance and sidereal time. Phase, tides, echo and eclipses are all computed from it at the Orrery clock's date, not scheduled. Eclipses happen only when the geometry lines up: syzygy plus the Moon near a node.
  - **Validated:** a scan from 1 Jan 2026 finds the real eclipses of 17 Feb 2026 ☉, 3 Mar 2026 ☾, 12 Aug 2026 ☉, 28 Aug 2026 ☾, 6 Feb 2027 ☉, 20 Feb 2027 ☾, 18 Jul 2027 ☾ and 2 Aug 2027 ☉. On 6 Oct 2026 the echo is 2.495 s (Moon at 373,954 km).
  - The Orrery's own drawn Moon is a simple circle and isn't used for this.
- **Universal rules extended:**
  - Osc 2 ratio is folded into an octave either side. Earth's 366 spins per year → 1.431, +620¢.
  - **Seasons:** sin(solar longitude) × sin(tilt) ÷ sin 30°. Earth gets ±0.78; Mercury and Venus get none.
  - **Pressure → Atmos/Drive** is written down: p = log10(P/1 mbar) ÷ log10(92 bar/1 mbar); Atmos 65%·p, Drive 70%·p². This gives Earth 39/26.
- **Earth defaults:** plays strikes (it has a moon, so no drone), attack 12 ms, release 3 s, cutoff 834 @C3 (albedo 0.294), res 3.
- **The Moon on Earth:**
  - **Tides:** the semidiurnal tide at Greenwich, lunar + 0.46× solar, each ∝ 1/distance³. Spring/neap and perigee/apogee come out of the math. Tide→Cut ±0.8 oct.
  - **Moonlight:** illuminated fraction drives Osc 2 (Moonlight→O2 60%).
  - **Echo:** a delay at the real light time there and back (2.4–2.7 s), lowpassed, with feedback (Echo 45%, Fdbk 30%).
  - **Eclipses (toggle, on):** a solar eclipse ducks Earth up to −92%; a lunar eclipse dims and reddens the echo and takes the moonlight out of Osc 2.
- **Readouts:** season, moon (% lit, distance), echo seconds, tide, eclipse status, and the next eclipse with a **go** button that jumps the sky to two hours before it.
- **Known:** at 1 day/s an eclipse lasts about a quarter of a second, so slow the rate to hear one. Tides update at 20 Hz, so above a few days/s they alias.
- **Measured:** Earth −34.9 dB RMS (strikes) at its output; frozen at the 6 Feb 2027 eclipse, the module read "☉ SOLAR 78%" with the amp ducked to 0.28. No errors. Not listened to.

### v0.010 — Mars, Phobos and Deimos
- **Data:** NASA NSSDCA Mars Fact Sheet including "Satellites of Mars" (updated 19 May 2025), retrieved 6 Oct 2026.
- **Mars voice, from the universal rules:**
  - Osc 2 = 669.6 spins per year → folded to 1.308, **+465¢**.
  - Cutoff 759 @C3 (albedo 0.25).
  - 6.36 mbar → Atmos 11 / Drive 2.
  - e 0.0935 → a strong speed sweep.
  - Seasons from its real solar longitude Ls (heliocentric longitude − 85.06°), with the 25.19° tilt giving ±0.85.
  - Plays strikes (it has moons): attack 8 ms, release 1.8 s, res 4.
- **Phobos and Deimos as modulators:**
  - Each raises a tidal term cos 2(rotation − moon longitude) on the filter.
  - **Phobos** outruns Mars's day, so its tide runs backwards (↺), laps the sky every 11.1 h, and sweeps fast.
  - **Deimos** laps every 5.5 d and sweeps slow.
  - Defaults are ±0.6 / ±0.25 oct (Phobos's real pull is about 69× Deimos's).
- **Transits:** the moon's shadow lands on Mars when its separation from the Sun line is under asin(R_Mars ÷ a). That's 21.2° for Phobos and 8.3° for Deimos, combined with the Sun's Martian declination.
  - A Phobos transit ducks Mars up to 33%; a Deimos transit up to 3%.
  - Phobos transits come out of the geometry in every season except near the solstices (Ls ≈ 90° and 270°), where the Sun's declination exceeds 21°.
  - The **Transits** toggle is on by default.
- **Readouts:** Ls and season, each moon's tide and sky lap, and transit status.
- **Known:**
  - Phobos and Deimos positions use mean motion from the Orrery's epoch, not a JPL ephemeris, so transit *seasons* are physical but transit *times* aren't real-world.
  - The echo stage is Earth-only now; in v0.009 it was any planet with moons.
  - **In Rotational Music Box at 1 day/s, the Sun's beam strikes Mars about once per Martian year (687 s)**, so Mars is mostly silent there unless Drone is on or the rate goes up. Earth has the same issue: about once per 365 s.
- **Measured:** master −23.3 dB RMS (Mercury, Venus, Earth). No errors. Not listened to.

### v0.011 — The old master Filter on the planets
- **The SYNTH page Filter** (cutoff, resonance, type, slope) now filters the planets' combined output: `plBus` → two biquads (24 dB, or one stage plus an allpass at 12 dB) → old FX bus. It reads `NFILT` and `VOICE.slope` at 20 Hz (`plBusFilter`).
- **Not carried over:** Filter EG, keytrack and matrix pins on cutoff. Those are per-voice in the old engine.
- The scene's filter setting now colours the planets. Rotational Music Box loads lowpass 3 kHz, 24 dB.
- **Measured on the planet bus:** cutoff 3 kHz −4.4 dB, 200 Hz −16.8 dB, 20 kHz −5.7 dB. At master, the reverb tail and output stage soften the difference. No errors.

### v0.012 — Drones off by default; Jupiter and the Galilean moons
- **Drone is off by default on every planet**, including Mercury and Venus (Charlie).
- **Data:** NASA NSSDCA Jupiter Fact Sheet (updated 2 Oct 2024) and Jovian Satellite Fact Sheet (updated 6 Dec 2023), retrieved 6 Oct 2026.
- **Jupiter voice, from the universal rules:**
  - Osc 2 = 10,477 spins per year → 1.279, **+426¢**.
  - Cutoff 923 @C3 (albedo 0.343).
  - No surface (>>1000 bar) → Atmos 65 / Drive 70.
  - e 0.0487 sweep. Strikes; attack 20 ms, release 3.5 s.
  - Tilt 3.13°, so seasons aren't used.
- **`plGalilean(jd)`:** real positions of Io, Europa, Ganymede and Callisto (Meeus ch. 44). The Laplace relation λIo − 3λEu + 2λGa reads **180.0°**, as it does in the real system. Each moon takes a module role at its real period, so Io:Europa:Ganymede (1:2:4) lock as a polyrhythm:
  - **Io → ring mod.** A new stage, Jupiter only, with the carrier at 3× the note. It pulses with Io's magnetic latitude in Jupiter's tilted field (9.4° tilt at 200.1°; pulse = |cos|⁶, twice per ~13 h), standing in for its flux tube and radio storms. Io→Ring 50%.
  - **Europa (bright ice) → Osc 2 level** (50%).
  - **Ganymede (largest, own magnetic field) → cutoff** (±0.6 oct).
  - **Callisto (dark, outside the resonance) → amp** (25%).
- **Readouts:** each moon's angle, Io's radio pulse, and the Laplace angle.
- **Known:**
  - Jupiter's rotation zero is the Orrery's epoch, not System III, so the Io radio pulse has the right rhythm but not the real-world timing.
  - The ring-mod carrier ratio (×3) is a placeholder, not physics.
  - Not yet used: the inner moons (Metis, Adrastea, Amalthea, Thebe), the irregular swarm, Galilean eclipses and transits, and Jupiter's faint rings.
- **Measured:** a Jupiter strike at 110 Hz gave −32.4 dB RMS at the module output. No errors. Not listened to.

### v0.013 — The sky is back on the PLANETS page
- v0.002's PLANETS-only view is removed (`body.pl-only` gone). The orbital view, ribbon and keys show under the planet modules again.
- At 1920×1080 CSS px, the deck takes about 520 px and the sky about 200 px. The tallest cards (Earth) can clip at the bottom of the deck. No errors.

### v0.014 — Jupiter's rings and irregular swarm
- **Rings (resonator bank, Jupiter only).** Five ring resonators from the NASA NSSDCA Jovian Rings Fact Sheet (updated 14 Oct 2015): halo, main, Amalthea gossamer, Thebe gossamer, and the Thebe extension. Each is a bandpass (Q 60) fed after the VCA.
  - **Pitch** by Kepler's third law at the ring's middle radius: 6× the note at the halo, down to ×1.65 at the Thebe extension.
  - **Strength** by optical depth: the gossamer rings sit at about 0.4 of the main ring.
  - **Stirring:** each ring is stirred by the tide of the inner moons that feed it. Metis + Adrastea stir the main ring and halo, Amalthea the Amalthea ring, Thebe the Thebe ring and extension. Inner-moon data is from the Jovian Satellite Fact Sheet; positions use mean motion from the Orrery's epoch, not an ephemeris.
  - **Rings** 35% by default.
- **Swarm (granular cloud, Jupiter only).** All 87 irregular moons from the Jovian Satellite Fact Sheet (`JUP_IRR`).
  - **Families** are assigned by orbit: Himalia 9, other prograde 4, Ananke 26, Carme 30, Pasiphae 18.
  - Each moon sheds one triangle grain every time it crosses the Sun–Jupiter line (twice per orbit), so grain density follows the sky's rate.
  - **Pitch** from the period (Himalia, 250 d = 4× the note). **Size** sets loudness and length. **Position** sets pan.
  - **Retrograde moons play reversed grains.** Capped at 16 grains per 50 ms tick.
  - **Swarm** 35% by default.
- **Readouts:** ring stirring (main / Amalthea / Thebe %) and swarm grains per second.
- **Measured:**
  - Swarm density: 1 day/s ≈ 0.3 grains/s (too sparse to hear), 1 mo/s 9.6/s, 1 yr/s 106/s.
  - Master: −22.1 dB RMS at 1 mo/s, −19.6 dB RMS / −7.9 peak at 1 yr/s.
  - On a 110 Hz strike, the ring sum measured −25.7 dB RMS against −34.2 dB at the module output, so the rings are prominent at 35%.
  - No errors. Not listened to.
- **Known:** at 1920×1080 the Jupiter card runs to about 530 px, and the deck scrolls.

### v0.015 — Saturn: rings, gaps, moons, swarm
- **Data:** NASA NSSDCA Saturn Fact Sheet (updated 18 Mar 2025), Saturnian Rings Fact Sheet (19 Apr 2022) and Saturnian Satellite Fact Sheet (22 Jul 2025), retrieved 6 Oct 2026.
- **Voice, from the universal rules:**
  - Osc 2 = 24,226 spins per year → 1.479, **+677¢** (just under a fifth).
  - Cutoff 920 @C3 (albedo 0.342). No surface → Atmos 65 / Drive 70.
  - e 0.052. Strikes; attack 25 ms, release 4.5 s.
  - **Seasons** from the real northern spring equinox (11 Aug 2009) with a 26.73° tilt. On 6 Oct 2026 it reads Ls ≈ 198°, just past the May 2025 equinox, which matches.
- **Rings:** seven resonators, D C B A F G E.
  - Tuned by Kepler at each ring's middle radius. Strength by optical depth: B and A strongest, D, G and E faint.
  - Stirring: A by Janus, F by its shepherds Prometheus and Pandora, G by Aegaeon, E by Enceladus's plumes. D, C and B are steady.
  - Rings 45%. Makeup set by measurement: the rings sit about 7 dB under a dry strike.
- **Gaps:** the Cassini Division and Encke Gap are cut out of the ring sound as peaking notches (up to −30 dB). Mimas (its 2:1 resonance) deepens the Cassini notch; Pan's tide deepens the Encke notch. Gaps 70%.
- **Moons:**
  - **Titan** (1.5-bar atmosphere) breathes Saturn's Atmos room ±. Titan→Atmos 40%.
  - **Enceladus**'s plumes peak far from Saturn, as observed, and feed the E ring.
  - **Iapetus** (dark leading face, bright trailing face) swings Osc 2. Iapetus→O2 50%.
  - **Hyperion** (chaotic rotation): a smoothed random tumble target every eighth of its orbit, moving the cutoff. Hyperion→Chaos 30%.
- **Swarm:** 122 irregulars: the 59 on the satellite sheet plus the 63 announced in 2023 (periods from Kepler).
  - Families by orbit: Norse 100 (retrograde, reversed grains), Inuit 15, Gallic 7. Phoebe (548 d) = 4× the note.
  - The 128 moons announced in March 2025 and later discoveries aren't on the sheet yet.
  - Swarm 30%.
- **Generalised:** rings and swarm now come from per-planet tables (`RINGS`, `IRR`, `IRR_REF`), shared by Jupiter and Saturn.
- **Measured:** at 1 yr/s, swarm ≈ 67–78 grains/s; master (all planets) −19.4 dB RMS / −7.2 peak. No errors. Not listened to.
- **Known:** small-moon positions use mean motion from the Orrery's epoch, not an ephemeris. At 1080 px tall the Saturn card is taller than the deck, so the deck scrolls.

### v0.016 — Readouts no longer reflow
- Saturn's rings line wrapped intermittently as its numbers changed width, so the card jumped. Every planet readout is now `white-space: pre` (never wraps). The Saturn rings/gaps and Jupiter rings values are padded to a fixed 3-character width.
- **Checked:** all six built cards held a constant height over 60 samples at 1 mo/s. No errors.

### v0.017 — Uranus, with all 29 moons
- **Data:** NASA NSSDCA Uranus Fact Sheet (2 Oct 2024), Uranian Rings Fact Sheet (14 Oct 2015) and Uranian Satellite Fact Sheet (11 Mar 2023), retrieved 6 Oct 2026. S/2025 U1 (56,250 km, 0.40 d) is from NASA's JWST announcement (19 Aug 2025).
- **All 29 Uranian moons are now in the sky** (`BODIES`): 13 added — Cupid, Perdita, Mab, S/2025 U1, Francisco, Caliban, S/2023 U1, Stephano, Trinculo, Margaret, Prospero, Setebos, Ferdinand.
  - Masses are estimated from radius at 1300 kg/m³.
  - Everything now has 86 bodies (was 73); the Uranus system has 29.
  - All systems load without errors.
- **Uranus voice:**
  - Osc 2 = 42,718 spins per year → 1.304, **+459¢**.
  - Retrograde spin, so it pans backwards. Cutoff 842 @C3 (albedo 0.300). No surface → Atmos 65 / Drive 70. Strikes; attack 15 ms, release 4 s.
  - **Seasons:** tilt 97.77° → ±1.98, double Earth's and the most extreme, counted from the 7 Dec 2007 equinox. On 6 Oct 2026 it reads Ls ≈ 75°, approaching the 2028 northern solstice.
  - **Field→Wobble:** the magnetic dipole is tilted 58.6° (at 53.6°), so the filter wobbles once per 17.24 h day, scaled by sin(tilt). 40%.
- **Rings:** 12 resonators (6, 5, 4, Alpha, Beta, Eta, Gamma, Delta, Lambda, Epsilon, nu, mu), tuned by Kepler.
  - The narrow rings use Q 220, so they ring like struck wires.
  - Epsilon is stirred by its shepherds Cordelia and Ophelia.
  - Rings 40%; they sit about 5 dB under a dry strike.
- **Major moons:**
  - **Miranda** (shattered cliffs) → resonance spikes. Miranda→Res 30%.
  - **Ariel** (brightest) → Osc 2. Ariel→O2 50%.
  - **Umbriel** (darkest) → amp dips. Umbriel→Amp 25%.
  - **Titania** (largest) → cutoff. Titania→Cut ±0.6.
  - **Oberon** (outermost) → Atmos. Oberon→Atmos 30%.
- **Inner moons:** the 14 crowded inner moons shed glassy **sine** grains (Puck = 4× the note). About 34 grains/s at 1 day/s. Inner moons 30%.
- **Swarm:** 10 irregulars (9 retrograde, so reversed grains; Margaret prograde), Sycorax = 4× the note. Swarm 30%.
- **Generalised:** grain clouds are now `plGrains(list, ref, keys, bus, wave)`. Jupiter and Saturn use the same code.
- **Measured:** master at 1 yr/s −21.8 dB RMS / −9.8 peak. No errors. Not listened to.
- **Known:** major- and inner-moon positions use mean motion from the Orrery's epoch, not an ephemeris.

### v0.018 — Neptune, with all 16 moons
- **Data:** NASA NSSDCA Neptune Fact Sheet (3 Oct 2024), Neptunian Rings Fact Sheet (14 Oct 2015) and Neptunian Satellite Fact Sheet (11 Mar 2024), retrieved 6 Oct 2026.
- **All 16 Neptunian moons are now in the sky:** 8 added — Hippocamp, Halimede, Sao, S/2002 N5, Laomedeia, Psamathe, Neso, S/2021 N1. Everything now has 94 bodies.
- **Voice:**
  - Osc 2 = 89,668 spins per year → 1.368, **+543¢**.
  - Cutoff 828 @C3 (albedo 0.290). No surface → Atmos 65 / Drive 70. e 0.0097 (almost no sweep). Strikes; release 4.5 s.
- **Seasons from the pole (new, general method `plSunDec`).** The Sun's declination is computed from Neptune's heliocentric longitude and its IAU pole (RA 299.36°, Dec 43.46°). It gives −27.9° in 2005 (the southern summer solstice), −20.5° now, and +28° in 2087 (the northern solstice).
- **Field→Wobble:** dipole tilted 46.9° at 288°.
- **Winds→Drift:** the fastest winds in the solar system (to 580 m/s) drift Osc 2 by up to ±40¢ on a slow random walk.
- **Rings:** Galle, LeVerrier, Lassell, Arago, Adams. Arago's optical depth isn't given, so 0.001 is assumed. The rings are faint, about 15 dB under a dry strike.
  - **Adams arcs:** Courage, Liberté, Égalité 1 and 2, Fraternité. They gate the Adams resonator as they sweep past the Sun line, at the ring's Kepler period. Arc spans are approximate (duty ≈ 8%). Adams arcs 60%.
- **Moons:**
  - **Triton** (captured, retrograde) → cutoff, running backwards (↺). Triton→Cut ±0.6.
  - **Nereid** (e 0.75, most eccentric) → level from its real Kepler distance (0.25–1.75× mean). Nereid→Amp 30%.
  - **Proteus** → Osc 2. Proteus→O2 40%.
- **Grains:** the 6 inner moons shed sine grains (Larissa = 4× the note; ~26/s at 1 day/s). The 7 irregulars (4 retrograde) are the swarm (Halimede = 4×). Grain tables are now general (`INNER`, `INNER_REF`).
- **Measured:** master at 1 yr/s −18.1 dB RMS / −7.1 peak. All systems load. No errors. Not listened to.
- **Known:** Triton, Proteus and arc positions use mean motion from the Orrery's epoch, not an ephemeris.

### v0.019 — Sky toggle; planets open by default
- **New "sky" button** in PANELS (beside tracks / keys / dots) shows and hides the orbital viewer. With it off, the planet deck takes the room and the rate slider, ribbon and keys stay. The choice is remembered (`orrery.sky`).
  - At 1920×1080 the deck goes from 518 to 715 px, so every built card fits without scrolling.
- **The PLANETS page opens on every load**, regardless of the last rack page used.
- No errors at 1300 and 1920 px.

### v0.020 — Pluto; all nine planets across the screen
- **Data:** NASA NSSDCA Pluto Fact Sheet (updated 11 Jan 2024), retrieved 6 Oct 2026, including Charon and the four small moons (barycentric). All 5 moons were already in the sky.
- **Voice:**
  - Osc 2 = 14,178 spins per year → 1.731, **+950¢**. Retrograde spin.
  - Cutoff 2.0k @C3 (Bond albedo 0.72, the brightest after Venus). 13 µbar → no drive.
  - e 0.244, the widest speed sweep; it saturates near perihelion.
  - Strikes; attack 10 ms, release 3 s.
- **Seasons from the pole** (`plSunDec`, RA 132.99°, Dec −6.16°): equinox about 1988; subsolar latitude 49°N in 2015, matching New Horizons' sunlit north; 64°N now.
- **Sun→Atmos:** Pluto's nitrogen air sublimates near the Sun and freezes out far from it, so its Atmos room scales with sunlight³ (40%). This is a modelled relation, not a measured curve.
- **Charon→Wobble:** Pluto circles a barycentre 2,126 km from its centre, outside the planet, every 6.387 d. Pitch wobbles up to ±30¢ (30%).
- **Small moons:** Styx, Nix, Kerberos and Hydra shed sine grains. Pitch ∝ 1/period and they sit near 3:4:5:6 with Charon, so the grains form a chord. Hydra = 2× the note.
- **Neptune 3:2 readout:** the resonant angle 3λP − 2λN − ϖP (mean longitudes) holds near 240–247° from 1700 to 2300. It never nears 0°, which is why Pluto and Neptune never meet.
- **Layout:** planet cards now share the width (min 186 px, max 230 px). At 1920 px all nine fit with no scroll; at 1500 px the row scrolls. Some long readout lines clip at 186 px.
- **Measured:** master at 1 mo/s −21.7 dB RMS / −9.3 peak. No errors. Not listened to.
- **Known:** at today's date Pluto's filter runs very bright (fast near perihelion, plus a high northern summer).

---

## ★ MILESTONE — v0.020 saved as `orrery-planetary-synth-v0_020-MILESTONE.html`
All nine planets built with their per-planet controls and moon assignments: Earth's tides, echo and eclipses; Mars's transits; Jupiter's Galilean roles, rings and swarm; Saturn's rings, gaps and moons; Uranus's and Neptune's field wobble, winds, arcs and grains; Pluto's Charon wobble. Keep this file as the reference for that work.

---

### v0.021 — Uniform data cards; controls and assignments stripped for the matrix (Charlie)
- **Every planet card shows the same rows, in the same order, readouts only:**
  - **orbit · now** (live): distance, speed, sunlight, spin angle, season as the Sun's subsolar latitude ("none" when the tilt is under 5° from upright).
  - **orbit:** semi-major axis, period, eccentricity, inclination, perihelion, aphelion.
  - **spin:** rotation (↺ retrograde), day length, axial tilt.
  - **body:** mass, radius, density, gravity, Bond albedo, temperature, pressure, magnetic field.
  - **rings** (or none).
  - **named moons** (count and list; long lists scroll in the card).
  - **unnamed moons** (count, total and source).
- **Moon counts:**
  - Named = the names in NASA's tables: Earth 1, Mars 2, Jupiter 57, Saturn 63, Uranus 27, Neptune 14, Pluto 5.
  - Unnamed = latest total − named: Jupiter 58 (of 115, NASA APOD Jun 2026), Saturn 230 (of 293, NASA Aug 2026), Uranus 2 (of 29), Neptune 2 (of 16).
- **No controls on the cards.** Sliders, On/Drone and the Eclipses/Transits/go buttons are removed. Every planet stays on with drone off. "cutoff now" is removed.
- **Sound: unique assignments zeroed.** Every moon, ring and grain modulation is set to 0, so that routing can be built in the matrix. Each planet keeps its common voice: oscillators (Osc 2 interval rule), filter, envelope, Drive/Atmos, and the shared speed→cutoff, sunlight→amp, spin→pan and season links.
  - Pluto's atmosphere is now 0 (its sunlight-driven room was a unique assignment).
  - Grain clouds no longer run while zeroed.
- The physics (lunar theory, Galilean positions, rings, swarms) is all still computed and ready to become matrix sources.
- **Checked:** no inputs or buttons on any card; seasons read Earth 5°S (6 Oct, correct), Uranus 73°N, Pluto 64°N. No errors. Not listened to.

---

**Session 2 — 7 Oct 2026 (Opus).** v0.022–v0.067. Spin became the first patch point: per-degree blips on nine Cs, then a full trigger bar (years and months on the orbit; days down to arcseconds on the spin, with hour-angle units that make Earth a real-time clock). Each planet got a beam, spin was re-measured from the Sun (solar day), and the page now opens on real IAU spins, with **sync** as the downbeat and 1:1 real time as the default. Presets, patches, the old mod matrix and LFOs were deleted; the old sequencer was silenced and its controls hidden; the header was rebuilt (TRANSPORT | VIEW | SHOW | TRIGGERS). All checks headless; Charlie listened throughout.

### v0.022 — The dots show the planets
- **Keybed dots follow the planet modules** (Charlie). Each planet that is on lights two dots, its note (Osc 1) and its Osc 2 interval (dimmer), in the planet's own colour. Brightness follows the planet's VCA, so strikes flash and fade.
- **True-frequency ticks** on the keys are tinted by planet too.
- With `PL_ONLY`, the 73 old sequencer voices no longer light dots. They're unplugged, so they were showing notes nobody could hear.

### v0.023 — Names under the panel toggles
- **names** and **moon names** moved from their own VIEW group to a second row under PANELS (sky · tracks · keys · dots), right side of the top bar (Charlie). Same buttons and wiring; the VIEW caption is gone.

### v0.024 — Orbits in card colours
- **Each planet's orbit is drawn in its card colour** (`PLAN_COL`) in the top-down and edge-on sky views (Charlie). Brighter while the planet module is on, dimmer when off; a muted body keeps its grey dashed ring.

### v0.025 — Card colours everywhere, pitch colour retired
- **Pitch colour (v0.495) retired** (Charlie): `sweepColorsOn()` returns false. Bodies no longer wear the colour of the note they sing.
- **Planet dots and names** in the sky now use their card colours (`BODY_COL`, identical to `PLAN_COL`), matching their orbits. Moons keep their own palette.

### v0.026 — No "orbit · now" caption
- The **orbit · now** caption is removed from every planet card (Charlie). The live rows (distance, speed, sunlight, spin, season) now sit directly under the planet name.

### v0.027 — Spin, the first patch point
- **Spin blips** (Charlie): every degree a planet turns, it plays one short sine blip at its own pitch (3 ms attack, ~25 ms decay) through its pan, echo and output, so it shares the planet's level and the FX bus. At most one blip per planet per frame. This is a variation on the beams, meant to free the sound from orbital distance carrying all the weight.
- **Spin gauge**: a small dial beside each card's spin readout, its hand in the planet's colour, turning with the planet (backwards for Venus, Uranus and Pluto). The degree readout is fixed-width.
- **Boot scene rate** (Rotational Music Box) is now 5 min/sec (was 1 day/sec). A saved user boot default keeps its own rate.
- Rates at 5 min/sec: Jupiter and Saturn about 3 blips/s, Earth and Mars about 1/s, Uranus and Neptune about 2/s; Pluto about one every 5 s; Mercury about one every 45 s, Venus about one every 3 min.
- **Old sequencer strikes off** (Charlie): the planets speak only through their spin blips. The keybed dots now light from each blip, fading over ~180 ms.

### v0.028 — Nine Cs for the spin blips
- **Spin pitch** (Charlie): each planet blips on a C, one octave per planet, by distance — outer lowest, inner highest. Low: Pluto C1 (33 Hz), Neptune C2, Uranus C3. Mid: Saturn C4, Jupiter C5, Mars C6. High: Earth C7, Venus C8, Mercury C9 (8.4 kHz). The blips no longer borrow the old sequencer's orbital-period pitch, and the 20 Hz–8 kHz clamp no longer applies to them.

### v0.029 — A quieter viewer
- **Sun's beam** no longer drawn (Charlie): `drawRadarBeams` returns early while `PL_ONLY`.
- **Sun menu removed** (the smiling-sun strike board, top-left of the viewer, and its planet tree). Hidden with CSS; the code is still in the file.
- **Orbital geometry buttons removed** (True · Circles · To Scale). The viewer stays on Circles. Hidden with CSS.
- The pitch/timing lock button (padlock) is still there, and the info line under the time still reads "Sun's beam · pitch from orbital period", which is now stale.

### v0.030 — Padlock pulled, caption updated
- **Pitch/timing padlock removed** from the viewer (Charlie: this system won't use it). Hidden with CSS; the lock stays off.
- **Viewer caption** now reads "spin blips · one per degree · nine Cs by distance" (was "Sun's beam · pitch from orbital period").

### v0.031 — Spin at three grains
- **SPIN section gains three live rows with gauges** (Charlie): **degree** (0–359°, one sweep per rotation), **arcminute** (0–59′ within the current degree, one sweep per degree) and **arcsecond** (0–59″ within the current arcminute, one sweep per arcminute). Hands in the planet's colour; retrograde planets turn backwards.
- Display only. The blips still fire once per degree.

### v0.032 — Degree, arcminute, arcsecond move up
- The three spin gauges (v0.031) move to the live rows at the top of each card, between sunlight and season (Charlie).
- The single **spin** row and its gauge (v0.027) are removed; **degree** replaces it. The retrograde ↺ still shows on the SPIN section's rotation row.

### v0.033 — Spin rings in the sky
- **Three rings around each planet** in the heliocentric views (Charlie): inner = arcsecond (within the arcminute), middle = arcminute (within the degree), outer = degree (of the whole turn). Each is an arc from 12 o'clock in the planet's colour over a faint full circle; retrograde planets (Venus, Uranus, Pluto) sweep the other way. Names move out past the rings.
- Computed straight from the sim clock and `PHYS.rotH`, the same as the card gauges.

### v0.034 — Spin rings, second design
- **The planet's dot is now the arcsecond** (Charlie): a pie in the planet's colour that fills from 12 o'clock over a dim disc, one sweep per arcminute.
- **Rings pulled in one layer:** arcminute ring directly around the dot, degree ring outside it (was three rings around the dot). Retrograde planets still sweep the other way; names sit just past the degree ring.

### v0.035 — Pitch slider hidden
- **The pitch ribbon** (−10 to +10 oct, above the keys) is hidden for now (Charlie). Hidden with CSS; scenes still load it at centre, so nothing is bent.

### v0.036 — Tracks pulled
- **tracks** toggle removed from the PANELS group (Charlie).
- **The track list itself** (`#rack`, with its per-body rows and the frequency export) is hidden for good and `renderRack()` returns immediately, so the list is never built. The rest of its code is still in the file.

### v0.037 — The dot becomes a ring
- **Arcsecond is now a tiny ring** (Charlie), replacing v0.034's filled pie. Each planet is drawn as three concentric rings only — arcsecond, arcminute, degree — with no filled dot underneath. Ring spacing 2.5 px; the innermost ring is 70% of the old dot radius.

### v0.038 — Dimmer stars
- **Starfield behind the orbital viewer at half its previous brightness** (Charlie): `DIM` 0.5 → 0.25 (the v0.523 field was already at half). Applies to the stars, their glints and the faint Milky Way band.

### v0.039 — Moon counts, no names
- **Moon names removed from the cards** (Charlie has plans for them). The two lists become one **MOONS** section with three counts: named, unnamed, total.
- The per-planet moon-total source note (e.g. "NASA APOD, Jun 2026") no longer shows on the card; `MOON_SRC` is still in the file.

### v0.040 — Delay mix 25%
- **Default delay mix 25%** (Charlie): the boot scene (Rotational Music Box) was 50%; the engine's own fallback was 0%. Both now 0.25. Other factory scenes keep their own values.

### v0.041 — Ring count, no names
- **RINGS section shows a count only** (Charlie): Jupiter 4, Saturn 7, Uranus 13, Neptune 5, others 0 (`RING_COUNT`). Named rings only; gaps, arcs and ringlets are not counted. Names stay in `RING_NAMES`, unshown.
- **Coming (Charlie):** a disclosure button on each card that expands it to show the routing matrix for every planetary characteristic and component, moons included.

### v0.042 — Day counter
- **day** row added above degree on each card (Charlie): whole rotations (one full 360° turn) counted from when the page opened. Running time backwards counts down; jumping with "now" or the date picker jumps the count.

### v0.043 — Each planet's beam, and spin measured from the Sun
- **Spin is now Sun-referenced** (Charlie): every planet carries a beam fixed on its surface, and 0° is the moment that beam points at the centre of the Sun (local noon). `plSolarTurns(n)` = sidereal rotations − orbital revolutions (longitude = ϖ + ν, unwrapped via the mean anomaly), so the beam returns to the Sun once per **solar day**. Checked headless over 10 days: Earth 24.000 h, Mars 24.66 h, Jupiter 9.93 h, Pluto 153.3 h; Venus ≈117 d and Mercury ≈176 d on average (they vary with orbital speed).
- Everything spin-based follows it: the card's degree/arcminute/arcsecond gauges, the sky's spin rings, the spin blips, and the **day** counter, which now counts noons (beam passing the Sun) since the page opened.
- **Beams drawn in the sky**: a thin line from each planet in its colour, fading out, as long as the planet–Sun distance, so at noon it touches the Sun's centre. It turns with the planet (the same way round as the orbit; backwards for Venus, Uranus and Pluto). Top-down and edge-on views.
- Blip rates change for the slow spinners: Mercury now blips about once every 2.3 min at 5 min/sec (was 47 s), Venus about once every 93 s (was 3.2 min). The others barely move.

### v0.044 — Day gauge
- **The day row gets a gauge** like degree, arcminute and arcsecond (Charlie). Following the same rule (each gauge sweeps once per unit of the grain above it), the day hand sweeps once per **orbit**: it shows the planet's place in its year, from perihelion (mean anomaly). The number beside it is still the noon count.

### v0.045 — Sync: a downbeat
- **sync** button beside **now** in the transport (Charlie). It turns every planet so its beam points at the centre of the Sun (spin phase 0) without touching the NASA/JPL orbits; the spin phases were never real data (no IAU prime meridians), so nothing true is lost. Stored per planet as `PHYS[n]._spinOff`.
- The day counters restart at 0, and every degree readout jumps to 0°, so all the planets blip together on the downbeat; from there they drift apart at their real solar-day rates.
- Checked headless: 100 ms after sync, all nine within 1.4° of the Sun line (prograde just past 0°, Venus, Uranus and Pluto just under 360°), all day counters 0, beams visibly on the Sun.
- The offset lasts until the page reloads; **now** keeps it.

### v0.046 — Opens synced
- **The page opens synced** (Charlie: the default state for testing from here on). Every beam starts on the Sun and every day counter at 0; the orbits are still the real sky at the present moment. Checked on load: all nine at spin phase 0.0000.
- Terminology: the beam crossing the Sun is **local noon** (solar transit). Perihelion is the orbit's closest point to the Sun, a different event.

### v0.047 — Old matrix retired
- **MATRIX button and page removed** (Charlie: a whole new mod matrix is coming). The **M** shortcut and its hint are gone; a remembered matrix page falls back to PLANETS. The matrix grid is hidden on every page.
- **Scenes no longer load matrix pins**, so `MOD.pins` stays empty and nothing is routed (this also stops the old matrix's lift on the delay and reverb wet). The LFOs and the rest of the engine code are still in the file, unused.

### v0.048 — Presets and the old matrix deleted
**A whole new ball game (Charlie).** File down from 12,106 to 10,571 lines.
- **Presets deleted:** all 66 factory scenes, their level trims (`SCENE_TRIM`) and pitch fixes (`PITCH_FIX`), the patch library (`PATCHES`, ~40 patches), the patch browser and LCD, the `[ ]` patch keys, and saved user scenes/patches (no longer read). The SCENE zone in the header is gone (pick, save, ×, import/export, boot default). One state remains, `FACTORY[0]` "Default" (was Rotational Music Box: 5 min/sec, delay 25%, trim +0.5 dB); the page always boots into it, then syncs.
- **Old mod matrix deleted:** sources, destinations and pins (`MOD`, `MOD_SRC`, `MOD_DST`), the sky-as-source per body, the "hands" that turned controls, the JS-written destinations, the matrix grid UI and its LEDs.
- **LFOs deleted with it** (they were the matrix's sources): the four LFOs, their page and **LFO** button, scopes and shapes. The Modulation row and its tab are gone. Rack buttons are now SYNTH · FX · PLANETS.
- **Kept:** the audio bus the matrix used to own (mix → gain → pan → ring mod/phaser/flanger → chorus → delay → reverb), now built by a small `modBuildNodes()`.
- Day counter: an ε so a synced beam sitting exactly on the noon line can't read −1.
- Checked headless: loads and plays with no errors; spin blips on all nine Cs; SYNTH and FX pages render; sync, now, `[` and `M` cause no errors.

### v0.049 — The old sequencer's control row pulled
- **MODE · PITCH RATIO · TIMING · PITCH · SYSTEM · STRIKE · HELP (tutorial)** are gone from the header (Charlie); the header is now one row and the planet deck moves up. The row is hidden with CSS; its selects stay in the DOM at their boot values (System: Everything, so every planet stays in the sky; Timing: Beams; Pitch: Orbital Period), because the old engine still reads them. Nothing they control reaches the sound: the blips have their own clock and pitches.
- Checked headless: plays with no errors, all nine blips on their Cs, SYNTH/FX/PLANETS pages fine.

### v0.050 — TRIGGERS
- **New TRIGGERS group in the top bar** (Charlie): **days · degrees · arcmin · arcsec**, four toggles choosing which spin grains fire the blips. Any mix can be on; a planet blips when any enabled grain ticks over, at most once per frame. Degrees is on by default; the choice is remembered (`orrery.trig`).
- All grains count from the Sun line (solar day), so with sync they all start together at noon.
- At 5 min/sec, arcminutes and arcseconds tick faster than the screen refreshes for most planets, so those planets blip every frame (about 60 a second, a buzz). Slower rates spread them out.
- Checked headless over 2 s windows: degrees 33 blips, none 0, arcmin 100, arcsec 135 (the frame cap; headless runs at a low frame rate), days 0 (no noon in 2 s).

### v0.051 — Hour-angle triggers: the real-time clock
- **TRIGGERS gains hours · minutes · seconds of rotation** (Charlie), interleaved with the angle units: days · hours · degrees · minutes · arcmin · seconds · arcsec. Hour angle: 1 hour = 15°, 1 minute = 15′, 1 second = 15″ (24 per solar day, 1,440, 86,400).
- Because spin is measured from the Sun, **Earth's hour-angle units are the clock**: at real time (1:1) Earth's seconds trigger ticks once per real second, minutes once per real minute, hours on the hour. Checked headless: 10 s of sim time = exactly 10.0000 Earth seconds. Every other planet runs its own clock in the same units (Jupiter's minute ≈ 24.8 real s, Venus's ≈ 1.9 real hours; corrected in session 2).

### v0.052 — Real time by default
- **The rate slider boots at 1:1, real time** (Charlie); was 5 min/sec. Checked headless: sim time advances 1.002 s per real second; the slider sits on the 1:1 mark.
- At real time with **degrees** (the default trigger), blips are sparse: Jupiter about one every 99 s, Earth every 4 min, Mercury every ~12 h. **seconds** gives the clock pulse (Earth once a second).

### v0.053 — Rotators under the triggers
- **A dial under each TRIGGERS toggle** (Charlie), seven in all. Each has nine hands in the planet colours; a hand is that planet's progress through the current unit of the grain (day, hour, degree, minute, arcmin, second, arcsec), from 12 o'clock, measured from the Sun line. A hand passing 12 is that planet's trigger. After sync all hands start at 12 and fan out at their own rates; the slow grains (days, hours) stay bunched, the fast ones (seconds, arcsec) spread around the dial.
- Updated once a frame (`trigDials()` in the planets' tick). Checked headless: no errors; the fan-out shows 1.5 s after sync.

### v0.054 — Years and months
- **TRIGGERS gains years and months** (Charlie), ahead of days: years · months · days · hours · degrees · minutes · arcmin · seconds · arcsec, each with its nine-hand rotator.
- They run on the **orbit**, not the spin: `plLonU(n)` is the unwrapped heliocentric longitude from the J2000 spring equinox (ϖ + ν). **Years** fire as a planet crosses 0°; **months** fire at every 30° boundary (equal zodiac signs), a grid shared by all nine. Sync does not move them (the orbits stay real).
- Checked headless: Earth sits at 13.7° today (7 Oct, Sun opposite at ~194°, correct); measured over one Earth year, years come out at Mercury 88.6 d, Venus 224 d, Earth 365.3 d (eccentric orbits vary with where they are).
- The zodiac treatment is to be discussed next (Charlie).

### v0.055 — Orbit and spin triggers split
- The trigger bar is two groups with a divider (Charlie): **TRIGGERS · ORBIT** (years · months) and **TRIGGERS · SPIN** (days · hours · degrees · minutes · arcmin · seconds · arcsec). Each group is ordered largest to smallest for every planet; across the groups the order depends on the planet (Mercury's solar day is two of its years).

### v0.056 — 1:1 no longer halts
- **Bug (Charlie):** at real time, clicking the rate thumb stopped the sky. The halt zone ran right up to the 1:1 mark (slider positions 0–124, 1:1 at 125), so any click on the left half of the thumb landed in it. Reproduced headless: clicks 5–30 px left of the 1:1 centre all gave rate 0.
- **Fix:** halt is now only the far left (positions 0–44, ~20 px); 45–124 is a **1:1 detent** that snaps the thumb onto the mark. Checked: clicks 5–20 px left of 1:1 now stay at 1:1; a click at the far left still halts.

### v0.057 — Real spins: the page opens on NOW
- **Problem (Charlie):** opening synced put every planet at noon, so every trigger had a full unit to wait before anything sounded (a minute or more for Earth).
- **Real spin phases from the IAU rotation models** (`IAU_ROT`, WGCCRE 2015: pole α0/δ0, W = W0 + Ẇ·d). Each planet's beam sits on its prime meridian (Earth: Greenwich; Jupiter: System III), and `plRealPhase(n)` works out the Sun's hour angle there from the real orbit (ecliptic → equatorial at ε = 23.439°). Pluto's IAU pole is the right-hand-rule one, so its sign is flipped to match ours.
- **The page opens on it** (no longer synced), and **now** sets it too: real orbits and real spins. **sync** still makes the downbeat. Trigger counters re-arm quietly, so neither change makes a burst.
- Checked headless at 07:47:54 UTC on 7 Oct: Earth's beam at 299.8°, Greenwich mean time gives 296.75°; the 3.05° (12.2 min) difference is the equation of time for early October, as it should be. All nine land at scattered phases. Drift between the IAU model and our clock over 30 days: Jupiter 0.2°, Earth 1.4°.

### v0.058 — Header rearranged
- **PANELS** (sky · keys · dots / names · moon names) moved left, beside **SYNTH · FX · PLANETS** (Charlie). The **TRIGGERS** (orbit and spin) now sit at the far right.
- Checked at 1920 (one row) and 1440 (the triggers wrap to a second row, right-aligned).

### v0.059 — Spin rings off the planets
- The three spin rings around each planet in the sky (v0.033–v0.037) are removed (Charlie); each planet is its coloured dot again, with its name beside it. The beams stay. `spinRings()` is still in the file, unused; the cards and the trigger dials carry the spin readouts.

### v0.060 — Sun card pulled
- The greyed **Sun** placeholder ("master bus, not built yet") is removed from the end of the planet deck (Charlie). The deck is the nine planets, Mercury to Pluto. The Sun module itself is still on the roadmap.

### v0.061 — View buttons on their own row
- The header is two rows (Charlie): **logo · transport · triggers** (far right) on top, and the view buttons underneath, under the logo and transport: **SYNTH · FX · PLANETS**, then **sky · keys · dots · names · moon names** in a single line (the PANELS caption is dropped). Done with flex `order` and a full-width break, so nothing moved in the DOM except the break.
- Checked at 1920 and 1440: both fit in two rows; at 1440 the triggers now stay on the top row.

### v0.062 — Reverse and date pulled
- The **reverse** button and the **date** picker are removed from the transport (Charlie), with their handlers and the date readout's refresh. Time runs forward from now; **now** and **sync** remain. (`timeDir` stays at +1; `jumpSkyTo` is still used by now.)

### v0.063 — SKY beside PLANETS, one or the other
- **sky** moves from the view toggles to a rack button, **SYNTH · FX · PLANETS · SKY** (Charlie). SKY and PLANETS take turns: SKY shows the orbital viewer and closes the planet deck; PLANETS opens the deck and hides the viewer. SYNTH and FX open the deck as before, alongside whatever is showing. The last choice is remembered and the page opens on it.
- Checked headless: planets → deck only; sky → viewer only; synth → deck (synth page) with the sky; planets again → deck only. No errors.

### v0.064 — View buttons beside the transport
- The header is one row again (Charlie): logo · transport (START · PANIC · REC · now · sync) · **SYNTH · FX · PLANETS · SKY** · **keys · dots · names · moon names** · triggers at the far right. The v0.061 row break is switched off.
- At 1920 everything fits on one row; at 1440 the triggers wrap to a second row, right-aligned.

### v0.065 — Header tidied
- Every group is captioned and divided (Charlie): **TRANSPORT** | **VIEW** (SYNTH · FX · PLANETS · SKY) | **SHOW** (keys · dots ¦ names · moon names) | **TRIGGERS · ORBIT** | **TRIGGERS · SPIN**. A divider now separates TRANSPORT from VIEW (it was missing), and a short one splits keys/dots from the name toggles.
- VIEW and SHOW buttons share one height (30 px) and spacing, and their captions line up with TRANSPORT's.

### v0.066 — Header groups share one top line
- TRANSPORT, VIEW and SHOW now hang from the same top line as the TRIGGERS (Charlie), instead of being centred in the taller bar. Measured headless: every caption at y = 10 px and every button row starting at y = 24 px; the logo sits level with the button row.

### v0.067 — Logo raised
- **Fix (Charlie):** v0.066 padded the logo down below the button row. The brand block now hangs from the same line as the buttons: logo and title span y = 24–52 px, exactly level with START (24–52).
