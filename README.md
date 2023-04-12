# Deluge Synth Presets

** These synth presets are now hosted on [my Gumroad page](https://meatbeats.gumroad.com). This repo will not be updated with new sounds.**

A collection of synth presets for the Synthstrom Deluge. Only internal oscillators used - no samples. Each preset is a simple XML file.

## Presets
- Roland Juno-60 - Factory Bank A
- Roland TB-303 - 15 starter synths + demo song

## Installation
1. [Download this repository as a zip file](https://github.com/weavermedia/deluge-synths/archive/refs/heads/main.zip)
2. Unzip the contents
3. Optionally rename the required synth XML files (see below)
4. Copy the XML files to the SYNTHS folder on your Deluge SD card

**Note**: you do not have to copy entire folders of XML files. You can pick and choose any presets you like. This helps to keep your SD card SYNTHS folder light and preset browsing fast on the Deluge.

## Renaming XML files

To avoid possible conflicts with existing synths on your SD I recommend you rename the XML files before copying. I use a prefix before each name to allow for easy browsing and loading.

For example, `11-STRINGS1.XML` from 'Juno60-FactoryGroupA' becomes `J60A-11-STRINGS1.XML`

Use the naming system makes the most sense to you.

## Preset Notes

### Roland Juno 60 - Factory Group A
[Watch a 6-minute demo video of the presets on YouTube](https://www.youtube.com/watch?v=EcqYMWde5bI)

These presets were ported from the TAL U-NO-LX. Some are very close to the original (the simpler sounds) and others vary in accuracy. Feel free to tweak and send me improvements!
- Some presets are missing (71, 72, 73, 75, 76) due to them using filter self-oscillation.
- Some sound different because they use all 3 oscillator waveforms (Square/Saw/Sub).
- Presets that use the Juno chorus are ported pre-chorus then Deluge chorus/reverb added.

### Roland TB-303
[Watch a 1-minute video of the demo song on YouTube](https://www.youtube.com/watch?v=PWHVqo6Fu2k)

The Roland TB-303 has no presets so this is a collection of starting points to create your own. The essense of the 303 sound is movement, achieved by manipulating the filter and envelope controls.

Envelope 1 is used for amplitude with fast attack, full sustain and short release. Envelope 2 controls the low-pass filter cutoff with independent control over the decay time.

|303 Control|Deluge Parameter|Control|
|------|------------|---------|
|Waveform | Oscillator 1 Type (Square/Sawtooth)|Via menu or shortcut|
|Tuning | Oscillator 1 Transpose|Via menu or shortcut|
|Cut Off Freq | LPF Cutoff |Parameter 2 Upper (default)|
|Resonance | LPF Resonance |Parameter 2 Lower (default)|
|Env Mod | Envelope 2 -> LPF Cutoff |Parameter 7 Upper (custom)|
|Decay | Envelope 2 Decay |Parameter 7 Lower (custom)|
|Accent | Velocity -> LPF Cutoff |Parameter 8 Lower (custom)|

Assign these parameters to an external MIDI controller for maximum tweakage.

SLIDE: To get the characteristic slide effect extend the length of one note to the next. Be sure to slide between notes more than an octave apart to get the full effect. Legato (VOICE > POLY > LEGATO) and Portamento (VOICE > PORT > 10) are already assigned in the presets.

ACCENT: For accented notes set the velocity higher than regular notes. Then use the Velocity -> LPF Cutoff modulation (assigned to paramter 8 lower) to control the accent strength.

The demo song `ACID.XML` includes 12 famous acid lines, each using a different preset. The copyright in the clips remains with the original owners and are for educational purposes only.

**Note:** This is not an accuarate emulation of a real TB-303. The original has too many idiosyncrasies for that. But it does give you a very usable 303 sound, especially when automating the assigned parameters.

## Support

Everything here is supplied free of charge with no expectations but if you would like to support the creation of more sounds feel free to buy a track or two on my Bandcamp page: https://dannytaurus.bandcamp.com/

## Contribute

If you make improvements to the accuracy of these sounds I'm happy to merge them into this repo. Either submit a pull request or create an issue.

## Changelog

Oct 31st 2021 - Roland TB-303 presets and demo song added.

Oct 23rd 2021 - Roland Juno-60 Factory Group A added.
