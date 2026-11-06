<img width="1917" height="1078" alt="Captura de tela 2026-11-06 004548" src="https://github.com/user-attachments/assets/65cf4cc7-f2d0-47ad-bc5e-c4f576a6d113" />

# Beginnings-OpNER
Beginnings OpNER, by Edzito, is an emulator specifically for EarthBound Beginnings Remake, a ROM hack by EBBR Team and PK Hack. Available for Windows, Linux, macOS and Android, with fullscreen play, keyboard, mouse, gamepad and touch controls, CRT filters, save states and quality-of-life features. Independent project. No ROM included.

A dedicated emulator frontend for the EarthBound Beginnings Remake (EBBR) SNES ROM hack. This independent project is not affiliated with the EBBR team, Nintendo, or SHIGESATO ITOI/HOBONICHI. Please see CREDITOS.md for the remake staff and acknowledgments.

This is still experimental, okay? Tweaks are needed.

## HIGHLIGHTS
- Fullscreen presentation with 1080p output.
- Expanded scenery and adjustable camera zoom.
- Keyboard, mouse and gamepad support.
- Click-to-move controls using the game’s normal collision rules.
- Save states organized into drawers, with screenshot previews.
- Quicksaves, quick loading and autosaves.
- Fast-forward and rewind.
- Customizable CRT filters with four personal presets.
- Mirrored psychedelic battle backgrounds and subtle enemy movement.
- Optional Double XP, Double Difficulty and Enemy Diversity modifiers.
- A manual “Where to go?” progression guide.
- A 60 FPS presentation target; actual performance depends on your hardware.

## Your own ROM is required

No ROM is included. Use your own EBBR SNES ROM; this application is designed for the remake, not the original NES game.

On Android, install `Beginnings OpNER Android 3.8.7.apk`. On first launch, select your ROM using the file picker. The app retains the imported ROM for later launches. Updates signed with the same key and using the same application ID can preserve existing app data.

On desktop, place your ROM in `Put your EBB rom here` and keep the distribution folders together. A single `.sfc` or `.smc` file can keep its own name. If multiple ROMs are present, name the intended one `EarthBound Beginnings (USA).sfc`. An explicit ROM path can also be supplied as `--rom "path/to/your ROM.sfc"`.

Desktop versions always start in borderless fullscreen with a 1080p presentation canvas. The display aspect ratio is preserved; F11 can switch to a window during the session.

## Platforms

- Windows x64: launch `Windows/Beginnings OpNER.exe`; keep SDL2.dll beside it.
- Linux x64: launch `Linux/earthbound-beginnings`; keep the bundled lib directory. Mark the executable as executable if your archive extractor does not preserve permissions.
- macOS Intel and Apple Silicon: open `macOS/Beginnings OpNER.app`. This locally built application is not notarized.
- Android ARM64: install the APK in the Android folder. No ROM is bundled.

## Controls

Keyboard: WASD or arrow keys to move; E, Space or Enter to confirm/interact; Esc, Q, Ctrl or Backspace to go back; Tab to toggle actions; Shift or C to run; + to fast-forward; - to rewind; F1 for options.

Character naming and final confirmation preserve the complete native frame, independent of map zoom. The direct mouse cursor-positioning change from 3.8.6 was reverted at the user's request.

Mouse: left-click the scene to move toward a point and interact; hold and move to update the destination. Movement follows the ROM's collision rules and does not find routes around obstacles. Right-click toggles actions or goes back in submenus. The wheel and middle button cycle battle directions/targets.

Touch: hold and drag to move. In menus, one deliberate swipe sends one arrow command; lift your finger before the next swipe. Tap the central confirmation area for OK and the lower area for Back. Name-entry keyboards use swipes and central OK, rather than direct letter selection. Pinch outward to zoom in and inward to zoom out. Landscape mode also provides OK, Back and Actions buttons. Optional virtual buttons are available in F1.

Gamepads: supported through SDL controller/joystick input. Face buttons provide confirm, back/actions, run and status functions; trigger inputs provide fast-forward and rewind; the right stick adjusts zoom. Physical layouts may differ between controller models.

On Linux, audio tries the default output, named outputs, and the PulseAudio/ALSA backends when needed. If audio is still unavailable, check `Saves/audio-status.txt` for the selected backend, error messages, and mute/volume settings.

## F1 options and saves

F1 provides video, audio, controls, touch, saves, guide, gameplay and CRT tabs. Menu language can be English or Portuguese; credits remain in English.

Save drawers contain manual slots and a quicksave slot. The black phone opens the save browser; the red phone opens the load browser. Select a slot and confirm the operation. Loading replaces the current running state. Autosaves are listed separately. Save/load feedback uses a flash and sound. Existing photographs retain the resolution at which they were originally captured.

Gameplay includes optional Double XP, Double Difficulty and Enemy Diversity modifiers, disabled by default. The God Menu requires deliberate activation and displays a warning because cheats can disrupt progression. The FAST / REWIND BUTTONS option hides both on-screen time controls and removes their touch areas; keyboard and gamepad shortcuts remain available.

CRT offers several filters, adjustable parameters and four personal presets. Sharp pixel sampling remains the base presentation mode. The guide is a manual campaign guide, not an automatic quest tracker.

## Presentation and performance

The frontend supports expanded scenery, manual zoom, full-screen output and a 60 FPS presentation target; Android also offers 30 FPS. Actual frame rate and audio continuity depend on the device. The underlying ROM artwork remains pixel art. Initial logos and notices are presented once, centered on their own background. Musical effects during gameplay use a separate background compositor.

This release includes English credits and documentation. Windows-based automated checks were run during development; physical Android testing and runtime testing on macOS are still needed. There is no guarantee of a constant 60 FPS on every device or of compatibility with every ROM revision or controller.

Updated source files are in Sources. Build scripts depend on the parent development workspace's SDL2, CMake, Ninja, Zig and Android tools. Binary toolchains, ROMs, personal saves, caches and private signing keys are excluded from this distribution.

So....

HAVE FUN!

THANKS EBBR TEAM AND PK HACK!




