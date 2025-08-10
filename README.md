# Retro Neon Digital Clock

![Retro Neon Digital Clock](path/to/generated-clock-image.png) <!-- Placeholder for the generated image -->

## Overview

This project recreates a retro-futuristic neon digital clock inspired by vintage designs, implemented using CSS for web display. The clock features glowing neon effects, metallic textures, and a moody atmosphere. It includes a main time display, subtle animations (implied as flickers and glows), and extensions for an event display panel showing national and religious festivals, plus a rotating camera that links to a GitHub profile.

The design is highly detailed, with photorealistic elements like shadows, gradients, and noise overlays. This README provides detailed prompts for generating identical visuals using AI image tools (e.g., DALL-E, Midjourney, or Stable Diffusion). The prompts ensure 100% fidelity to the described CSS structure.

### Key Features
- **Core Clock**: Tall pipe enclosure with neon digital display showing time (e.g., "12:34 AM").
- **Event Display**: Right-side panel listing upcoming and past events/festivals (Indian national, Muslim, Hindu, Christian, Sikh, and others).
- **Rotating Camera**: Top-mounted scanning camera with interactive link implication.
- **Name Integration**: "Tahir" engraved in neon style.
- **Aesthetics**: Retro-futuristic with orange-yellow neon glows, metallic reflections, and film grain overlay.
- **Interactivity**: Camera "clickable" (implied in web version) to open [https://github.com/imtahirnaseer](https://github.com/imtahirnaseer).

## Installation and Usage

1. **Clone the Repository**:
   ```
   git clone https://github.com/imtahirnaseer/Nixie-Tube-Clock.git
   cd Nixie-Tube-Clock
   ```

2. **Open in Browser**:
   Open `index.html` in a modern browser to view the CSS-based clock.

3. **Generate Visuals**:
   Use the prompts below with an AI image generator to create static renderings. For the web version, apply the CSS directly.

## Detailed Prompt for AI Image Generation

Use this combined prompt to generate a single photorealistic image of the extended retro neon digital clock. It merges the core design with extensions, ensuring no elements are missed or altered. The image should be high-resolution, square or portrait aspect ratio, centered on a dark gradient background with noise overlay.

### Combined Prompt

Create a highly detailed, photorealistic digital artwork or rendering of a retro-futuristic neon digital clock, exactly matching the visual style and elements defined in the following CSS code description, extended with a right-side event display and top-mounted rotating camera. The image should represent the clock in its "on" state, with all glow effects, shadows, animations implied as static glows or flickers (e.g., subtle electric sparks or blooming light), and precise color gradients, textures, and positioning. Ensure nothing is missed or altered—replicate 100% accurately based on the structure, colors, dimensions, and effects described. The clock is a standalone object centered in the frame, on a dark gradient background, with a noise texture overlay for a vintage, grainy feel. Assume a displayed time like "12:34" in large digits and small secondary display for "AM" or date, using an LCD/digital font style (e.g., segmented digital display like old calculators or clocks). The overall aspect ratio should be square or portrait to fit the tall pipe structure, with the clock occupying most of the frame.

Integrate the name "Tahir" aesthetically in a fitting location for visual appeal (e.g., engraved on the top-tube). Make the top camera appear clickable (with visual cues like a glow halo) to imply linking to "https://github.com/imtahirnaseer". The event display shows upcoming and past national and religious events/festivals, including all major Indian ones: Independence Day, Republic Day, Gandhi Jayanti, Eid al-Fitr, Eid al-Adha, Muharram, Milad un-Nabi, Diwali, Holi, Navratri, Durga Puja, Raksha Bandhan, Janmashtami, Ganesh Chaturthi, Dussehra, Christmas, Easter, Good Friday, Guru Nanak Jayanti, Vaisakhi, Guru Gobind Singh Jayanti, New Year, Labor Day, Teacher’s Day, Children’s Day, Pongal, Onam, Baisakhi, Makar Sankranti, Shivratri, Lohri, Ugadi, Vishu. Ensure no event is missed; show 2-3 per section with implied scrolling.

**Background and Overall Setup:**

The background is a linear gradient from #040909 (deep black) at the top (covering about 60vh) to #312c2a (dark brown) at the bottom (starting at 80vh), creating a moody, dimly lit room or surface effect. Overlay the entire image with a subtle noise texture (like old film grain or static), at 12% opacity, covering 100% width and height, using an SVG or procedural noise pattern for a pointer-events-none z-index 100 effect. The clock is positioned centrally, with flex display for perfect centering in row wrap, no margins, overflow hidden on body. Font family stack: "LCD", "LCD2", "LCDMono2", "LCDMono", "Digitalism" (use a pixelated, segmented digital font for the display digits to match).

**Color variables to use exactly:**

--_refl: #f3eeef (reflection white)  
--_bloom: #fcfbf9 (blooming white glow)  
--_y1: #fae8a5 (yellow glow 1)  
--_y2: #fbd608 (yellow glow 2)  
--_o1: #ff8f0c (orange glow 1)  
--_o2: #e74702 (orange glow 2)  
--_o3: #b32801 (orange glow 3, darker red-orange)  
--mw1: #d0d5d7 (metallic white 1)  
--m1: #fdea09 (metallic yellow 1)  
--m2: #e46703 (metallic orange 2)  
--m3: #ac2a04 (metallic red-orange 3)

**Size scaling:** --_factor: min(600px, 80vh); --_size: min(--_factor, 80vw). Use this for proportional sizing in the image. Include a subtle user-select: none and transition effects implied as smooth glows.

**Shadow Element:**

Positioned absolutely at bottom:0, top:0, margin auto, width 100%, height 0em, translated 0 45em. Box shadow: 0 0 3em 2em #040909, 0 0 8em 3em --_o3, 0 0 10em 4em --_o2, 0 0 10em 5em --_o1, at 0.6 opacity. Before pseudo-element: height 20em, width 0, centered, box shadow 0 0 8em 4em --_y1, 0 0 8em 6em --_y2, 0 0 8em 8em --_o1, 0 0 8em 10em --_o2, 0 0 8em 12em --_o3. After pseudo-element: z-index -1, opacity 0.5, border-radius 50%, height/width 10em, border 2px solid red, transformed rotateX(70deg), box shadow 0 0em 12em 40em --_o1, 0 0em 12em 60em --_o2, 0 0em 12em 80em --_o3. This creates a glowing orange-red shadow pool under the clock, spreading elliptically on the surface, with yellow highlights.

**Outer Pipe:**

Position absolute, z-index 2, width calc(--_size * (8/15)), height --_size, border-radius 20%/10%, overflow hidden, opacity 1. Clip-path: polygon(0 0, 100% 0, 100% 85.8%, 0 85.8%) for bottom clip. Represents the main tall, rounded rectangular enclosure for the clock, dark and tubular.

**Inner Pipe:**

Width/height 100%, scale 0.84 0.91, border-radius 15%/7%. Box shadow: 0em 104em 16em 20em #040909, 0em 1.2em 1em 0.2em --m3, 0em 1.2em 1em 0.5em --m2, 0em 1.2em 0.5em 1.2em --m1, 0em 1.2em 1.2em 1.5em --m2, 0em 1.2em 2em 2em --m3, 0em 90em 16em 20em #040909, -1em 1em 2em 3.7em #040909, 0.5em 0em 2em 3.7em #040909, 0em 0em 0em 4.6em --mw1, 0em 0em 0.5em 5em --mw1, 0em 0em 0em 20em #040909. Creates internal depth, natural light reflections, and glowing orange metallic effects inside the pipe.

**Pipe Accents:**

Width calc(--_size * (8/15)), height --_size, position absolute. Top-tube: top 3%, centered, width 16%, height 6%, background linear-gradient(120deg, rgba(60,62,62,1) 0%, rgba(4,9,0,1) 60%), box-shadow inset -0.2em 1.1em 1.4em -0.4em --mw1, inset 0em -1.2em 0.5em -1.1em --m1, inset 0em -1.2em 1em -0.8em --m2, inset 0em -1.2em 1em -0.2em --m3, border-radius 20%. Tube-holders: width 26em, height 70em, translate 0 -7em, centered. Each div is 3em x 3em circle, with conic-gradient metal colors (--_metal-1 #30241d, --_metal-2 #000000, --_metal-3 #5f5f5f), box-shadow inset 0 0 0.1em 0.1em #ffffff5d, inset glows. Positions: child1 top12% left -8% rotate -65deg, child2 top12% right -8% rotate 65deg, child3 top26% left -8% rotate -85deg, child4 top26% right -8% rotate 85deg, child5 top78.5% left -8% rotate -115deg, child6 top78.5% right -8% rotate 115deg. Top: top -0.7%, centered, width 22%, height 6%, similar background and shadow as top-tube. Topinset: top -1.7%, centered, width 14%, height 8%, similar, border-radius 50%. Before: 50% size circle, box-shadow inset 0 0 0em 0.1em #040909, 0 0 0.5em 0.1em --_bloom, inset glows with --_o3 to --_y1, animated flicker (imply as subtle varying intensity in image). Left and right accents: full width/height. Each has 3 divs, width 14%, height 2.4%, border-radius 0.7em, background #040909, positions and radii specific (e.g., left child1 top16% left -3%, border-top radii 50%, with before pseudo for extension). Shadows for metallic glow. Bottom-left: bottom 12%, left -6%, width 20%, height 2.4%, border-radius 40% with top 50%, shadows. Before: top -24%, 90% width 70% height, similar. Bottom-right: symmetric to bottom-left.

**Small Outer Pipe:**

Position absolute, translate 0 -5.6%, width calc(--_size * (1/2.7)), height calc(--_size * 0.87), border-radius 40%/10%, overflow hidden, clip-path bottom 96%, border-top 0.3em solid --mw1. Small inner pipe: 100%, scale 0.92 0.98, border-radius 35%/10%, box-shadow similar to inner pipe but adjusted values.

**Base Container:**

Position absolute, width calc(--_size * (8/15)), height --_size. Base div: bottom 4%, left -10%, width 120%, height 12%, border-radius 40%/30%, box-shadow 0 2em 2em -1.4em #000, inset -0.4em 0.1em 0.8em -0.2em --mw1. Before: 100% width 50% height, border-radius 100%, shadows including glow.

**Display:**

Color --_bloom, font-size 14em, line-height 0.8em, translate 0 -0.4em. Row: flex display. Small-row: font-size 0.3em, right -22%, top 10%, column flex, line-height 1.02em. Col: flex, relative. Child1 opacity 0.2 (dim layer), child2 absolute right0 z2, child3 absolute right0 with --_bloom color, text-shadow multiple --_bloom and --_o3 to --_o1 for glowing effect, sizes 0.1em to 0.6em.

**Glass Tube:**

Absolute, width 26em height 70em, translate 0 -7em, border-radius 1000px, box-shadow glows and insets for reflections. Before: left reflection, after: right reflection with blur.

**Hex Pattern:**

Absolute, width 17.7em height 70em, translate 0 -7em, border-radius 1000px, overflow hidden, z -1, opacity 0.7. Background: complex radial and linear gradients in hex pattern with --_hex-cl1 #040909, --_hex-cl2 --_o1, size 2.18em, repeating every 2x3. Overlay: white mix-blend-mode overlay, width 200%, left -40%, height 12%, rotate 40deg, implying electric animation (show as diagonal streak or spark).

**Tube Base Container:**

Absolute, width 34em height 30em, translate 0 24em. Tube base: bottom 4%, width 60% height 20%, border-radius 80%/40%, shadows. Before: 99% width 42% height, shadows. Tube btm: bottom 34%, width 40% height 10%, border-radius 20% 20% 100% 100%, shadows. Before: bottom -158%, width 60% height 40%, similar. Rods: bottom 14%, width 50% height 28%, clip bottom 80%. Left-rod: width 60% height 12% rotate 60deg bottom 40% left0, center-rod 30% rotate90deg, right-rod 60% rotate-60deg right0, all with shadows. Wires: full, z -1. Child1/2: width/height 18%, rotate 25deg/122deg, positions, shadows for curved wires.

**Button:**

Absolute, width/height 4em, border-radius 50%, translate 0 43em, centered, z100, background --_bloom, box-shadow orange halos and insets, filter blur(1px). Represents a power button with glow.

**Power Cord:**

Z -1, scale 1.4 0.9, absolute full width height 50em, centered, transform rotateX(55deg) rotateZ(-64deg). Child1: width 20em height 18em, translate 39.3em 0em, bottom 4%, border-bottom 6px #040909, border-right 4px #040909, border-radius 100% 30%/100% 0, shadow. Child2: width 20em height 12em, translate 58em 0.2em, bottom 40%, border-top 3px #04090977, border-left 4px #040909, similar radius and shadow.

**Right-Side Event Display:**

Position absolute, attached to the right side of the outer pipe (aligned with calc(--_size * (8/15)) width), extending outward like a connected panel. Width: calc(--_size * 0.3), height: calc(--_size * 0.7), positioned at top 15% of the main tube, z-index 3. Shape: Rounded rectangular with border-radius 15%/7%, clip-path polygon(0 0, 100% 0, 100% 90%, 0 90%). Material: Matches outer pipe (#040909 base with metallic sheen), with linear-gradient(120deg, rgba(60,62,62,1) 0%, rgba(4,9,0,1) 60%). Connection: A small bridge (width: 5em, height: 2em, background #040909, border-radius 50%) visually links the panel to the outer pipe, with box-shadow inset -0.2em 0.4em 0.6em -0.2em --mw1, inset glows (--m1, --m2, --m3).

Two sections: Upcoming Events (top 60%) and Past Events (bottom 40%), separated by a horizontal divider (1em height, background --mw1, box-shadow inset 0em 0.2em 0.4em -0.2em --mw1). Font: Same LCD stack, color --_bloom, font-size 3em for event names, 1.5em for dates, line-height 1.2em. Upcoming Events: Show 2–3 events (e.g., "Independence Day - Aug 15", "Diwali - Oct 29"), scrolling vertically (imply as static list with topmost event brightest, fading slightly downward). Past Events: Show 2–3 events (e.g., "Gandhi Jayanti - Oct 2", "Eid al-Fitr - Apr 10"), dimmer (opacity 0.7), static. Glow: Text-shadow on event names matching display (.col > div:nth-child(3)): 0em 0em 0.04em --_bloom, multiple --_o3 to --_o1 (0.1em to 0.6em sizes). Box-shadow: Matches inner pipe, with added inset glows. Subtle flicker on upcoming events (varying intensity 0.8–1 opacity). Border: 0.2em solid --mw1 on left edge.

**Top Rotating Camera:**

Position absolute, centered above outer pipe (top -5%), width 10em, height 10em, z-index 4. Shape: Circular (border-radius 50%), with a smaller inner circle (60% size, centered) for the lens, background #040909, linear-gradient(120deg, rgba(60,62,62,1) 0%, rgba(4,9,0,1) 60%). Lens: Inner circle with box-shadow inset 0 0 0.5em 0.1em --_bloom, inset 0 0 1.3em 0.2em --_o3, inset 0 0 1.3em 0.4em --_o2, inset 0 0 1.3em 0.6em --_o1, inset 0 0 1.3em 2em --_y1. Animation: Imply 360-degree rotation (static as a tilted angle, e.g., 45deg, with a faint motion blur trail), with a red scanning beam (1em wide, --_o3 color, extending outward, fading to transparent). Visual cues for clickability: Slight brighter glow (0.1em --_bloom halo). Scanning Effect: Subtle hexagonal overlay fading outward, using --_hex-cl1 #040909, --_hex-cl2 --_o1, size 1em, opacity 0.5. Beam points toward right-side panel at 45deg angle. Box-shadow: Matches topinset, with outer halo 0em 0em 0.5em 0.1em --_bloom. Subtle flicker on lens (varying intensity 0.7–1 opacity).

**Name Integration ("Tahir"):**

Placement: Engrave or display "Tahir" on the top-tube or topinset of pipe-accents, centered. Style: Font matches LCD stack, size 2em, color --_bloom, with text-shadow 0em 0em 0.04em --_bloom, 0em 0em 0.1em --_o1, 0em 0em 0.2em --_o2, 0em 0em 0.3em --_o3 for neon glow. Effect: Subtle engraving (inset box-shadow 0em 0.1em 0.2em --mw1) blended into metallic surface.

**Additional Effects:**

Flicker animation: Subtle varying opacity in glowing parts (0.4 to 1). Electric animation: Diagonal white overlay streak implying motion. Ensure all elements are layered correctly (z-indices), with photorealistic metallic textures, reflections, and neon blooms. No additional elements; match 100% to this description for exact replication. High resolution, sharp details, no distortions. Do not apply off state; keep all glows active.

## Contributing

Contributions are welcome! Fork the repo and submit a pull request. For issues, open a ticket on GitHub.

## License

MIT License. See [LICENSE](LICENSE) for details.

## Credits

Design inspired by retro electronics. Created by [Tahir](https://github.com/imtahirnaseer).
