# Chrono Squad — Vijay Time-Travel Game (v0.1 Design Doc)

**Working title:** *Chrono Squad: The Vijay Saga.* Alternates to consider — *Three Times Vijay*, *Vijay Across Time*, *The Vijay Continuum*, *Triple Thalapathy*.

**One-line pitch.** A celebratory top-down action-adventure where you command three Vijays — Young, Mid, and Current — pulled across time to restore his own fading timeline, hot-swapping between them to use each era's signature abilities.

---

## Core fantasy

The player isn't playing *as* Vijay. The player is *commanding the squad of Vijays* — three versions of the same man, working together across time to save themselves. Every level is a love letter to a chapter of his life as a performer, not a recreation of any specific film. The tone stays warm, joyful, and nostalgic throughout. Combat exists, but it's never grim — defeated enemies disperse into confetti and music notes rather than damage. The fantasy this game sells the fan is "all of Vijay, all at once, on your team."

## The three Vijays

**Young Vijay** is the scout. Late-90s look — leaner build, longer hair, the wide-eyed energy of a debutant. He moves the fastest, double-jumps, dashes through narrow gaps, and climbs ledges the others can't. His attacks are quick and rapid but light on damage. He's how you explore a zone, find shortcuts, and reach hidden collectibles.

**Mid Vijay** is the all-rounder and the heart of the squad. 2000s-2010s peak look — settled features, signature confident stance. His unique ability is the *Dance Pulse*: a short, AoE rhythm move that briefly stuns every enemy in a ring around him. It's a cheeky nod to his real-life dance reputation rather than any specific film move. Standard movement, balanced melee, mid-range projectile — he's the one you fight most encounters with, and his pulse is the answer to crowd moments.

**Current Vijay** is the heavy and the leader. Present-day look — full presence, gravitas. Slower movement, but a shield that blocks projectiles, a heavy strike that breaks barriers and large enemies, and a *Charisma Aura* that passively buffs the other two whenever they're near him. He's the only one who can smash certain walls, push heavy objects, and tank boss attacks.

The deliberate design constraint: each level needs all three. There is always a wall only Current can break, a gap only Young can reach, and a crowd that only Mid's pulse can defuse. That requirement is what makes the swap mechanic the actual game, not a costume change.

## The squad / swap mechanic

The player controls one Vijay at a time. The other two follow at a short distance as AI companions — they don't fight unless the active player initiates combat near them, in which case they assist with light attacks. Pressing **1, 2, or 3** (or tapping their portrait on touch) instantly swaps the active Vijay; the camera smoothly snaps to the new one, and the previous active becomes a follower. For puzzle moments, the active Vijay can be told to "hold position" (one button) so the player can move a different Vijay independently — this is what enables one-Vijay-on-the-switch, another-Vijay-through-the-door puzzles.

Health is per-Vijay, not shared. If one falls, you can still play with the other two; they revive at the next checkpoint. Losing all three is the only fail state.

## The villain and story spine

The antagonist is **The Eraser** — a faceless, ink-like time entity that's slowly blotting Vijay out of his own memories. The squad assembles because the act of erasing one Vijay tears him out of every era at once, and the only way to fight back is for all his selves to remember together. The villain is deliberately abstract and non-political — no real-world rivals, no industry references, no movie tie-ins. Three boss encounters, one at the end of each memory zone, each a stronger fragment of The Eraser. The final boss is The Eraser at full strength, and the climax requires all three Vijays' signature abilities chained together to defeat it.

## The three memory zones

Each zone is a vibe, not a movie. The visuals draw from the texture of his life as an entertainer at that era.

**Zone 1 — The Sunlit Street.** A bright Chennai neighbourhood at midday. Cycle-rickshaws, banana-leaf vendors, kids playing cricket, banners on the walls. Easy enemies (ink-blot minions). Tutorial zone where the player meets each Vijay and learns the swap. Boss: a crowd of ink-minions that only Mid's Dance Pulse can clear.

**Zone 2 — The Stage Lights.** A theatrical performance arena at dusk — neon signs, rigging, spotlights, a live audience that cheers when you fight well. Mid-difficulty enemies and the first real platforming demands. Boss: an Eraser fragment that splits into three; each Vijay must take down one simultaneously (forces the player to switch fast).

**Zone 3 — The Stadium of Years.** A vast open-air venue at night under fireworks — a celebration of his career condensed into one space. Hardest enemies, layered puzzles needing all three Vijays in different positions. Final boss: The Eraser itself.

## Core loop

Enter zone → explore with Young to find the path → fight encounters as Mid → break barriers and tank boss hits as Current → reach checkpoint → repeat with harder rooms → end-of-zone boss → cutscene of the squad recovering one of Vijay's memories → next zone. Total intended playtime for a v1 release is roughly 30–45 minutes — short, dense, replayable.

## Controls

WASD or arrow keys to move. **J** light attack, **K** signature ability (Young's dash, Mid's Dance Pulse, Current's heavy strike), **L** interact, **Space** jump, **Shift** hold-position toggle, **1/2/3** swap to Young/Mid/Current. On touch: virtual stick, three ability buttons, and three portrait taps for swap.

## Visual direction

Keep the "between 2D animation and realistic" direction from your earlier games — sprites stylised from real photos, chroma-keyed and treated, with hand-drawn outlines. The three Vijays must be instantly readable at a glance — silhouette, hair, and palette. Young leans warm-yellow accents, Mid leans red, Current leans deep blue. Memory zones use saturated, joyful palettes; The Eraser is the only ink-black element on screen, which makes it pop visually as the antagonist.

## Audio direction

A single original score motif that morphs across the three eras — sparser and more acoustic in Zone 1, fuller production in Zone 2, fully orchestrated and modern in Zone 3. The boss music is the same motif inverted into a minor key. SFX leans satisfying-arcade — a bright "ting" on swap, a percussive thump on Current's strike, a beat-drop on Mid's pulse. No real movie audio, no real songs.

## Scope for v1 (what we ship first)

One playable HTML file, mirroring your existing pattern. All three Vijays fully implemented with their kits. Zone 1 fully built and playable end to end with its boss. Zones 2 and 3 stubbed (level layout in, enemies and boss as placeholders) so the architecture is proven and we can fill them in iteratively. Save state via localStorage so the player can come back to it. No accounts, no leaderboard, no monetisation, no mobile-store packaging — same constraints as your other games.

## What I need from you next

Reference photos of Vijay across the three eras (one or two clean shots per era is enough — Young/late-90s, Mid/peak-2000s, Current). A working-title decision from the alternates above, or a fresh one. And your redline on this doc — kit changes, era choices, zone vibes, anything that doesn't feel right. Once those are in, I'll move to the vertical slice (Zone 1 playable, all three Vijays working, swap mechanic feeling good) before scaling up.
