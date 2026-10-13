# Orrery Planetary Synthesizer — version index
301 versions so far: v0.000–v0.300.

**Lineage:** forked from Orrery orbital sequencer v0.608 → v0.609 (X mode and bell room removed) → renamed v0.000. For v0.001–v0.609 of the sequencer, see VERSIONS-v0_608.md.

| version | notable |
|---|---|
| v0.000 | Fork of Orrery v0.609: X mode and bell room removed; renamed ORRERY PLANETARY SYNTHESIZER |
| v0.001 | PLANETS page (P): nine modules Sun outward; Mercury synth built (3:2 saws, speed→cutoff, sunlight→amp, spin→pan, drone default) |
| v0.002 | PLANETS page hides the sky/ribbon/keys; thin sliders; narrower Mercury card |
| v0.003 | Old synth unplugged (PL_ONLY); planets bypass old FX to the output stage; cutoff key-tracks |
| v0.004 | Double-click any planet slider → centre |
| v0.005 | Voice meter row taller — no longer crammed under the top bar |
| v0.006 | Voice meter counts only planet-module voices (was showing silent old voices) |
| v0.007 | Venus module; universal rules (Osc 2 = orbit÷rotation, eccentricity-scaled sweeps, retrograde pan, pressure→Drive/Atmos) |
| v0.008 | Planet modules routed into the old FX bus (plBus → mix), trims cancelled |
| v0.009 | Earth + Moon: real lunar mechanics (plLunar) → tides, moonlight, 2.5 s light-time echo, eclipses; seasons |
| v0.010 | Mars + Phobos/Deimos: two tidal modulators (Phobos backwards), Martian seasons (Ls), transits |
| v0.011 | Old SYNTH-page master Filter applied to the planets bus |
| v0.012 | Drones off by default; Jupiter + Galilean moons (real positions, Laplace 1:2:4): Io→ring mod, Europa→O2, Ganymede→cut, Callisto→amp |
| v0.013 | Orbital view restored under the PLANETS page |
| v0.014 | Jupiter: ring resonator bank (5 rings, Kepler-tuned, stirred by inner moons) + swarm of 87 irregular moons as grains |
| v0.015 | Saturn: 7 ring resonators + Cassini/Encke notches (Mimas, Pan), Titan→Atmos, Enceladus plumes→E ring, Iapetus→O2, Hyperion chaos, 122-moon swarm, real seasons |
| v0.016 | Planet readouts fixed-width, never wrap (Saturn rings line jitter) |
| v0.017 | Uranus: all 29 moons in the sky (+13), 12 narrow-ring resonators, field wobble, extreme seasons, five moon roles, inner-moon glass grains + irregular swarm |
| v0.018 | Neptune: all 16 moons in the sky (+8), seasons from the IAU pole, winds drift, field wobble, Adams-ring arcs, Triton backwards, Nereid swell, grains |
| v0.019 | "sky" toggle for the orbital viewer (remembered); PLANETS page open by default |
| v0.020 ★ MILESTONE (saved as -MILESTONE.html) | Pluto: Charon barycentric wobble, sunlit atmosphere, small-moon chord grains, pole seasons, Neptune 3:2 readout; nine cards fit at 1920 |
| v0.021 | Uniform read-only planet cards (orbit now · orbit · spin · body · rings · named · unnamed moons); controls and unique assignments stripped for the matrix |
| v0.022 | Keybed dots and ticks show the planet modules: note + Osc 2, in planet colours, brightness from each VCA |
| v0.023 | names / moon names moved under the PANELS toggles in the top bar |
| v0.024 | Planet orbits drawn in their card colours (brighter when the module is on) |
| v0.025 | Pitch colour retired; planet dots and names wear their card colours |
| v0.026 | "orbit · now" caption removed from the planet cards |
| v0.027 | Spin as first patch point: a blip per degree of rotation per planet; spin gauge on cards; boot rate 5 min/sec |
| v0.028 | Spin blips pitched on nine Cs by distance: Pluto C1 … Mercury C9 |
| v0.029 | Sun beam, sun menu and orbital geometry buttons removed from the viewer |
| v0.030 | Padlock removed; viewer caption describes the spin blips |
| v0.031 | SPIN rows: degree, arcminute, arcsecond, each with a gauge |
| v0.032 | Degree/arcminute/arcsecond gauges moved to the live rows; old spin row removed |
| v0.033 | Spin rings around each planet in the sky: arcsecond, arcminute, degree |
| v0.034 | Spin rings redesigned: dot = arcsecond pie, then arcminute and degree rings |
| v0.035 | Pitch ribbon hidden |
| v0.036 | Tracks toggle and track list removed |
| v0.037 | Planets drawn as three spin rings only; arcsecond is the tiny inner ring |
| v0.038 | Starfield dimmed 50% |
| v0.039 | Cards show moon counts (named, unnamed, total) instead of name lists |
| v0.040 | Default delay mix 25% |
| v0.041 | Cards show ring count instead of ring names |
| v0.042 | Day counter (full rotations since the page opened) above degree |
| v0.043 | Planet beams in the sky; spin, gauges, blips and day count measured from the Sun (solar day) |
| v0.044 | Day row gauge: sweeps once per orbit (place in the year from perihelion) |
| v0.045 | sync button: every beam to the Sun, day counters to 0, orbits untouched |
| v0.046 | Opens synced: every beam on the Sun at load |
| v0.047 | Old mod matrix retired: button, page, M key and pins removed |
| v0.048 | All presets, patches, the old mod matrix and LFOs deleted; one Default boot state |
| v0.049 | Old sequencer control row (mode, pitch ratio, timing, pitch, system, strike, tutorial) removed from the header |
| v0.050 | TRIGGERS toggles: days, degrees, arcmin, arcsec fire the spin blips |
| v0.051 | Hour-angle triggers (hours, minutes, seconds of rotation); Earth runs on real clock time |
| v0.052 | Rate slider boots at 1:1 real time |
| v0.053 | Nine-hand rotators under each trigger toggle |
| v0.054 | Years (one orbit) and months (30° zodiac signs) triggers, on the real orbits |
| v0.055 | Trigger bar split into ORBIT (years, months) and SPIN (days … arcsec) |
| v0.056 | Fix: clicking the rate thumb at 1:1 halted the sky; 1:1 detent added |
| v0.057 | Opens on real spins (IAU prime meridians, Earth on Greenwich); now resets to real; sync stays the downbeat |
| v0.058 | Panels toggles beside the rack buttons; triggers far right |
| v0.059 | Spin rings removed from the planets in the sky; dots return |
| v0.060 | Sun placeholder card removed from the deck |
| v0.061 | Header in two rows: view buttons under the logo and transport |
| v0.062 | Reverse button and date picker removed |
| v0.063 | SKY rack button beside PLANETS; the two take turns |
| v0.064 | Header back to one row: view buttons right after the transport |
| v0.065 | Header tidied: captions and dividers for every group, even button heights |
| v0.066 | Header groups top-aligned with the triggers |
| v0.067 | Logo level with the header button row |
| v0.068 | Apsidal precession: perihelia turn at JPL rates (Saturn, Neptune, Pluto backwards); "to scale" toggle back in SHOW |
| v0.069 | Cards: live "perihelion at" row (ϖ° and rate, ↺ backwards); seasons and Pluto 3:2 follow the turning perihelia |
| v0.070 | Perihelion dial on the cards (points as in the sky); rate on its own "precession" row |
| v0.071 | Precession trigger (slowest ORBIT clock: perihelion crossing 0°); every card carries the ten trigger rotators |
| v0.072 | Card clock strip removed; precession, year, month, hour, minute, second join the card listing with their wheels |
| v0.073 | Orbits drawn at their true tilt to the ecliptic; ascending nodes turn at JPL rates (nodal precession) |
| v0.074 | Constellation odometer on every card: the real constellation behind the planet (13, IAU boundaries), rolling |
| v0.075 | Zodiac band in the sky: 13 real constellations as stick figures, IAU boundary ticks, lit in the colour of the planet inside; "zodiac" toggle |
| v0.076 | Dials and readouts update every frame (were 20 fps, jerky at slow rates); halt removed: the slider bottoms out at 1:1 |
| v0.077 | Cards fold: fixed data (ORBIT down to the source line) hidden behind a +/− at each card's top right |
| v0.078 | Planet beams hidden by default; "beams" toggle in SHOW |
| v0.079 | Orbits shaded: bright and thicker at perihelion, fading toward aphelion |
| v0.080 | Orbit shading gentler and brighter; a dot at perihelion and aphelion with a break in the line |
| v0.081 | Apsis dots removed: perihelion and aphelion marked by a small break in the orbit line only |
| v0.082 | Apsis breaks narrowed to a hairline (~4 px) |
| v0.083 | Moons hidden in the sky by default; "moons" toggle in SHOW |
| v0.084 | SHOW moved under the title: two rows on the left (logo/title, then SHOW in one row) |
| v0.085 | SHOW buttons compact under the title (v0.084 made them full-size and bloated the left column) |
| v0.086 | Transport back beside the logo; SHOW in one compact row beneath both |
| v0.087 | Vintage instrument cards for all nine planets: brass plate, odometer counters, constellation drum, season meter, ten round gauges |
| v0.088 | Instrument cards smooth: needles on their own layers (no dial repaints); each needle points at its own value (no strobing) |
| v0.089 | Each instrument module enamelled in its planet's colour |
| v0.090 | Planet emblems in a brass porthole beside ARCSEC on every module |
| v0.091 | Smooth stop: dragging left of 1:1 eases the sky down to a halt; "stop" mark at the far left |
| v0.092 | Fix: dragging the rate slider back to the left no longer sticks near 1:1 |
| v0.093 | Fix: the sky no longer freezes at slow rates after a run far into the future (compensated time step) |
| v0.094 | Nameplate lamps flash on each triggered note |
| v0.095 | Milliseconds: "ms" trigger with rotator, and a MILLISEC gauge on every module |
| v0.096 | Captions clear of the bezels: DIST/SPEED/SUN under the counters, CONSTELLATION under its screen |
| v0.097 | Needles trigger only at the top; SYNC puts every needle (orbit and spin) at the top and sounds every planet |
| v0.098 | Orbit needles blur when fast; the rate slider becomes a brass throttle, always directly under the voice bar |
| v0.099 | Zodiac hidden by default; the top bar restyled as an instrument control panel |
| v0.100 | Keys, dots and voice meter in the instrument style: jewel lamps, lamp rail, bakelite keys, brass rail |
| v0.101 | Moons orbit inside each planet's emblem porthole, passing in front of and behind the planet |
| v0.102 | Planet sheet: click the porthole → full-deck machine with blank synth panels and a MOON BAY of named moons by family (unpatched jacks) |
| v0.103 | Planet sheet sits in the workspace below the throttle (replaces the card row) instead of a popup |
| v0.104 | The rate slider is engraved THROTTLE |
| v0.105 | THROTTLE centred on an engraved brass nameplate |
| v0.106 | THROTTLE plate removed; "throttle" toggle in SHOW hides/shows it |
| v0.107 | MOON BAY as a mixing console: a channel strip per moon, a group master per family |
| v0.108 | Moon console families open by default; planet selector centred as clicky bakelite keys |
| v0.109 | Clicking the porthole in the expanded sheet returns to the PLANETS view |
| v0.110 | SHOW row aligned under TRANSPORT |
| v0.111 | Planet keys moulded in their planet colours (jewel dots removed) |
| v0.112 | Navigator (SUN + nine planet keys) drives deck and viewport; ORBITAL view: ten phosphor CRT scopes, 2×5 |
| v0.113 | Navigator uses the sheet's keys, on its own centred header row |
| v0.114 | Scopes: no glow or strobing (fast motion fades out); a single planet fills the viewport |
| v0.115 | More space between the navigator and the voice bar |
| v0.116 | Navigator well ringed in brass like the throttle |
| v0.117 | TRANSPORT moved below the logo |
| v0.118 | VIEW button PLANETS renamed SEQUENCER |
| v0.119 | Mercury/Venus drone on C1; triggers per planet on each card (header bar retired); sheet panels wired as each planet's synth |
| v0.120 | Venus drone moves to C2 (Mercury stays C1) |
| v0.121 | On SYNTH the navigator shows each planet's synth (SUN = the original master SYNTH page) |
| v0.122 | Navigator keys to the top row; VIEW buttons to the centred row below |
| v0.123 | TRANSPORT left of VIEW, SHOW right of it, in one centred row |
| v0.124 | Navigator in its own panel under the throttle; header back to one row |
| v0.125 | Spacing and dividers between TRANSPORT, VIEW and SHOW |
| v0.126 | Triggers move from the cards to the sheet's top bar; singular moon/family counts |
| v0.127 | Trigger keys spelled out in full |
| v0.128 | ORBITAL scopes in square, screwed-down instrument mounts with brass nameplates |
| v0.129 | Scope phosphor tinted per planet colour |
| v0.130 | Sun scope in a black, brass-trimmed mount with engraved rays |
| v0.131 | Each card's nameplate lamp is its voice's mute |
| v0.132 | A lamp burns bright and breathes while its voice is sounding. |
| v0.133 | Mercury drone C-1 (8.18 Hz), Venus C0; spin blips two octaves lower; pitch floor 20 → 4 Hz. |
| v0.134 | Mercury C-1 · Venus C0 · Earth C1 · Mars C2 · Jupiter C3 · Saturn C4 · Uranus C5 · Neptune C6 · Pluto C7 |
| v0.135 | Lit lamps flicker like a filament: slow breath, jitter, rare dips. |
| v0.136 | The sounding note is engraved on the brass nameplate (held for drones, ~0.7 s after a blip). |
| v0.137 | A trigger strikes the planet's own synth instead of a shared sine blip. |
| v0.138 | Every planet armed on SECONDS (degrees took minutes to fire at 1:1); saved trigger settings reset. |
| v0.139 | Click picks one trigger (others off; click the lit one again = off); shift-click stacks. |
| v0.140 | Spin carried as whole turns + exact fraction (fmod + the v0.093 carry): dials, triggers, day count, sync and now stay exact after runs hundreds of millions of years out. |
| v0.141 | MILLISEC trigger, gauge and old header button removed |
| v0.142 | Each hand named for what it counts and turning once per the next unit up (seconds hand once a minute). |
| v0.143 | Cards: ORBIT · LOCAL SOLAR TIME (hours, minutes, seconds) · SPIN (degrees, arcmin, arcsec), then a DAYS counter. |
| v0.144–v0.146 | LCD, then nixie tubes, then red bubble LED — all rejected |
| v0.147 | Back to odometer wheels, eight of them. |
| v0.148 | A multiplier window beside the day wheels steps ×1 → ×10³ → … ×10¹⁵ when the wheels fill: no ceiling. |
| v0.149 | Every named moon in the MOON BAY drawn on its scope (irregular swarms and small inner moons joined). |
| v0.150 | Every named moon labelled in the single-planet scope view. |
| v0.151 | Mercury gets its own SKY scene (it had none: no moons): sodium tail, heat, magnetosphere, Sun stall. |
| v0.152 | Mercury scene rebuilt equatorial: Sun at centre, Mercury on its real ellipse. |
| v0.153 | Perihelion/aphelion diamonds with distances; shift-click a lamp to solo a planet. |
| v0.154 | Mercury's scene seen from straight above (true ellipse undistorted), flat range grid. |
| v0.155 | Venus–Pluto boot muted. |
| v0.156 | The navigator opens on MERCURY. |
| v0.157 | Top-left readout of the live oscillators, filter and state in the Mercury view. |
| v0.158 | Cutoff from true distance: 18 Hz at aphelion → 4 kHz at perihelion. |
| v0.159 | Removed from Mercury's scene |
| v0.160 | The Sun-stall caption removed; ring and readout row stay. |
| v0.161 | The scene and the breath generalised; Venus: cloud disc, evenly hot night, blue ion tail |
| v0.162 | FX delay and reverb mix 0 by default (were 25 % and 100 %). |
| v0.163 | Range rings run to the view's corners at any zoom (1-2-5 steps, labelled) |
| v0.164 | Mercury and Venus built from 32 sine partials (partial 1 = sine sub); the orbit opens them like drawbars toward perihelion |
| v0.165 | Mercury alone again. |
| v0.166 | Partials up to ~32 Hz stay open at aphelion (C-1 alone was silent on speakers). |
| v0.167 | The keybed plays the navigator's selected planet synth (held, mono; a drone takes the key while held). |
| v0.168 | The meter counts oscillators running (and buffer sources) against a 256 budget, red past 75 % |
| v0.169 | Non-finite canvas values drawn safely and logged; the main draw guarded. |
| v0.170 | The tail's 0/0 on a zero-size view (the cause of the dead throttle) fixed. |
| v0.171 | Each planet's noon beam on the Sun's tube. |
| v0.172 | VIEW button ORBITAL renamed SCOPE. |
| v0.173 | Mercury, Venus, Earth, Mars tubes: Sun at centre, true ellipse with apsides, trail, noon beam; Earth's and Mars's moons scaled up around them. |
| v0.174 | Scope beams reach exactly to the Sun: they cross it at local noon (future triggers). |
| v0.175 | Moon rings drawn clear of the planet dot; fast moons stay as dim dots. |
| v0.176 | Daphnis, Aegaeon, Methone, Anthe, Pallene, Polydeuces added to the scope. |
| v0.177 | SKY draws every named moon (swarms included, unnamed S/ left out), all labelled; drawing only. |
| v0.178 | Sun scope multi-coloured: each planet in its own phosphor |
| v0.200–v0.208 | Engine II — Claude's flagship-synth rebuild; abandoned (not carried forward) |
| v0.209 | Resynth step 1: the old Orrery engine voices the planets (Sun's beam, orbital-period pitch); navigator switches |
| v0.210 | MOON BAY strips live: mute, solo, level, strike glow |
| v0.211 ★ MILESTONE (saved as -MILESTONE.html) | STRIKE keys per planet: BEAM · RADAR · PERIAPSIS · HOLD |
| v0.212 | Datasheet on every planet's sheet: shared fields with rank bars, live column, what's unique |
| v0.213 | Scopes: labelled distance rings replace the unlabelled grid |
| v0.214 | Scopes: true-distance geometry (Nereid fixed); orbits brighter, ornaments dimmer |
| v0.215 | Voice bar: one LED per sounding body, Sun → Pluto |
| v0.216 | LED strip centred, label removed |
| v0.217 | Keybed dots in the sounding planet's colour |
| v0.218 | Sun view: calculator name readouts (replaced) |
| v0.219 | High bells ring shorter (linear per semitone, 100 % → 15 %) |
| v0.220 | BELLS preset button (an earlier v0.220 header move was rejected and deleted) |
| v0.221 | FIRST: one note per planet's system per sweep |
| v0.222 | PRESETS panel left of the navigator keys; singing bodies glow on the scopes |
| v0.223 | The Sun's beam in SKY; SHOW › sunbeam |
| v0.224 | Stereo WIDTH slider (mono · orbit · wide) |
| v0.225 | BELLS pulses at startup |
| v0.226 | Sun view: singing ring round each scope (DYMO labels tried) |
| v0.227–v0.228 | Bezel window, then bezel engraving — tried, rejected |
| v0.229 | Thin engraved brass plate under each scope |
| v0.230 | REVERSE: pitch mirrored about the keybed's centre |
| v0.231 | REVERSE → INVERT; presets row: bells · invert · first |
| v0.232 | Throttle labels 30 min · 3 hr; eccentric moon trails smoothed |
| v0.233 | Scopes: eccentric moons as true ellipses |
| v0.234 | BELLS latches |
| v0.235 | 3D view (Three.js) with brass joystick |
| v0.236 | Zodiac on the 3D sky sphere |
| v0.237 | Gentler joystick |
| v0.238 | DRONE |
| v0.239 | DRONE pitch rides the throttle |
| v0.240 | Presets: bells · first · drone; INVERT on the right |
| v0.241 | Saturn's rings in SKY, Kepler particles |
| v0.242 | Ring particles dimmed |
| v0.243 | DRONE its own group |
| v0.244 | Saturn in 3D at true scale (untested in a browser) |
| v0.245 | Shimmer interval −24…+24, double-click 0 |
| v0.246 | Throttle invites a pull after BELLS/DRONE |
| v0.247 | Plain on/off flashes; indent click stops it |
| v0.248 | CLOCK: gauges strike the planets; card keys un-wired from fixed notes |
| v0.249 | One ping per dial turn |
| v0.250 | Dials as oscillators (rate × 8192) |
| v0.251 | CLOCK runs dry (delay 0) |
| v0.252 | Arcsec clicks every arcsecond again |
| v0.253 | Nine-clock ladder; slowest coinciding tick wins |
| v0.254 | Each clock pitched by its own tick rate (× 128); MIDI on faces |
| v0.255 | Smoother throttle (dial faces on own layers, throttled readouts) |
| v0.256 | Strike glow replaces MIDI windows |
| v0.257 | BELLS opens SKY with moons |
| v0.258 | Bezel lights on strike; rainbow pitch lamp in each dial |
| v0.259 | WIDTH moved to the OUT section |
| v0.260 | Fixed Cs |
| v0.261 | Planetary seconds |
| v0.262 | Blips |
| v0.263 | Moon pulled in |
| v0.264 | CLOCK reverb centred |
| v0.265 | DRONE throttle (superseded by v0.266) |
| v0.266 | DRONE on the hourglass |
| v0.267 | One preset bank |
| v0.268 | DRONE opens SCOPE |
| v0.269 | BELLS off stops |
| v0.270 | Barn-find weathering |
| v0.271 | Darker case |
| v0.272 | SYNTH / FX into SHOW |
| v0.273 | First-release simplification |
| v0.274 | Keys are switches |
| v0.275 | Weathering tune |
| v0.276 | SUN toggles all |
| v0.277 | Keys are mutes |
| v0.278 | INVERT the scopes |
| v0.279 | Phosphor negative |
| v0.280 | Navigator row layout |
| v0.281 | Quiet unmute |
| v0.282 | ZODIAC pulled |
| v0.283 | System balance |
| v0.284 | 1 s fade-in |
| v0.285 | Throttle captions |
| v0.286 | Shift-click solo |
| v0.287 | START → DRONE |
| v0.288 | No pulsing |
| v0.289 | START → BELLS |
| v0.290 | Sun logo on SHOW |
| v0.291 | Top row spread |
| v0.292 | SEQUENCER → CLOCK view |
| v0.293 | (superseded) |
| v0.294 | One-line header |
| v0.295 | VIEW beside TRANSPORT |
| v0.296 | Title divider |
| v0.297 | CLOCK view doesn't auto-start |
| v0.298 | MAJOR / MINOR MOONS |
| v0.299 | Moon keys are clicky keys |
| v0.300 | Cards open, toggle gone ★ FIRST RELEASE CANDIDATE |
