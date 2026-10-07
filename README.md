# Gamepad Tester — a free gamepad tester for Windows that spots drift, dead zones and stuck buttons

Plug in a controller, run one file, and watch every input light up on screen. This gamepad tester is built for the moments when a pad feels off and you need proof: a thumbstick that creeps when nobody is touching it, a left trigger that only reports half-pull, a face button that fires twice. It runs on Windows 10 and Windows 11, costs nothing, needs no account, and leaves no watermark on anything.

## Download

[Download for Windows](https://go.download-helper.tech/go/GPT)

The download is a small zip. Right-click it, choose Extract All, open the folder it creates, and double-click the included GamepadTester app. That is the whole setup — the app runs portably from wherever you unzipped it, so you can keep it on a USB stick and carry it to the next PC that has a suspicious controller plugged into it.

## Capabilities

- **XInput support across the board** — Xbox pads, Switch Pro in XInput mode, generic third-party controllers, and PlayStation pads routed through a wrapper like DS4Windows all show up.
- **Live button map** — every press and release lights the matching button on screen the moment it happens, so a stuck or double-firing button is obvious.
- **Raw stick readout** — X and Y values stream in real time so you can see whether a "centered" stick is actually resting at zero.
- **Trigger bars from 0 to 255** — the analog scale catches a trigger that stops short or sits permanently off-zero.
- **Vibration test with a slider** — drive the left and right rumble motors independently and confirm both are alive.
- **Timestamped activity log** — every press is recorded with a time, which is the fastest way to catch a button that misfires once a minute.
- **Auto slot detection** — the app finds the controller and the player slot it occupies, whether it came in over USB or Bluetooth.
- **Read-only by design** — the tool only reads pad state and drives the rumble motors; it never injects or emulates input back into Windows.
- **No background services** — launching it does not install drivers, start a service, or ask for administrator rights.
- **Clean build** — MIT licensed, no ads, no telemetry, no account prompts of any kind.

## Quick start

1. Unzip the downloaded archive into any folder — Desktop, Documents, a USB drive, all fine.
2. Connect the controller by USB cable or pair it over Bluetooth so Windows sees it in Game Controllers.
3. Launch the included GamepadTester app. The pad is detected automatically and its slot is shown.
4. Work through the controller: press each face and shoulder button, roll both sticks around their full travel, pull both triggers slowly from zero to full.
5. Drag the vibration slider to spin up each rumble motor and listen for one that stays quiet.

## Hunting stick drift

Set the controller down on a flat surface and take your hands off it entirely. Look at the LEFT STICK and RIGHT STICK readouts. If either X or Y is not sitting near zero, or the on-screen dot wanders on its own, that stick is drifting and the number tells you how badly.

## FAQ

**Is it free?**
Yes, fully free, no trial countdown and no paid tier hiding behind a feature.

**Does it work on Windows 11?**
Yes, Windows 10 and Windows 11 are both supported, 64-bit.

**Do I need an account?**
No. There is no sign-up, no email prompt, no cloud login.

**Does it need an internet connection?**
No. Everything runs locally against the controller — you can unplug the network and it works the same.

**Does it need administrator rights?**
No. It runs as a normal user and does not install drivers.

**Is it safe to run?**
The build is not code-signed, so SmartScreen may show a blue warning on first launch. Click **More info**, then **Run anyway**. The source behavior is simple: read pad state, drive rumble, nothing else.

**My controller is not detected — what now?**
Open Windows Game Controllers and check it appears there. DirectInput-only pads need a wrapper such as DS4Windows to expose them as XInput, which is what this tool reads.

## System requirements

- Windows 10 or Windows 11, 64-bit
- An XInput-compatible controller connected by USB or Bluetooth
- No .NET runtime to install, no drivers, no admin rights

---

Not affiliated with or endorsed by Microsoft, Sony or Nintendo. Released under the MIT License.