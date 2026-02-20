# Walk Alarm

An alarm clock that forces you to physically walk 100 meters to dismiss it. No snoozing — you have to get up and move.

## How It Works

1. **Set the alarm** on your computer (computer.html)
2. When the alarm goes off, a **QR code** appears with a pairing code
3. **Scan the QR code** or enter the code on your phone (index.html)
4. **Walk 100 meters** — GPS tracks your distance in real-time
5. Once you hit the target, the alarm dismisses on both devices

The computer and phone communicate in real-time through Firebase.

## Features

- **GPS distance tracking** with accuracy indicator
- **5 alarm sounds**: Gentle Chime, Soft Melody, Classic Ring, Harsh Beep, Escalating
- **Sound preview** before setting the alarm
- **QR code pairing** between computer and phone
- **Real-time sync** via Firebase Realtime Database
- **Visual progress ring** on the phone showing distance walked
- **Wake lock** to keep screens active

## Files

| File | Purpose |
|------|---------|
| computer.html | Desktop alarm — set time, choose sound, displays QR code when ringing |
| index.html | Phone companion — enter pairing code, tracks GPS distance walked |

## Usage

1. Open computer.html on your computer
2. Set your alarm time and choose a sound
3. When the alarm rings, open index.html on your phone
4. Enter the 4-digit pairing code (or scan the QR)
5. Start walking — the alarm dismisses at 100m

## Tech Stack

- Vanilla JavaScript
- Firebase Realtime Database
- Web Audio API (alarm sounds)
- Geolocation API (GPS tracking)
- QR Code generation
