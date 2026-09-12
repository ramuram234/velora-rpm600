# Velora RPM600

Local-first indoor bike app for the **FS-583ADC / JIANJIA JJ-BLE** (RPM600).

## Download APK

The installable Android package is **Velora 1.4** (`com.velora.rpm600`).

Chat-card downloads are often blocked by Android. Use the **Download** page in the live preview:

1. Open the Grok live preview in **Chrome** (open in new tab, not inside Grok).
2. Go to `/download.html` or `/get`
3. Tap **Download APK**
4. If Chrome says blocked → **Download anyway**
5. Settings → Security → Install unknown apps → Chrome → Allow

Source zip is on the same page: `velora-source.zip`.

## What’s in this repo

This GitHub repo is the landing page. Full TypeScript + Kotlin source is in the zip from the download page (`src/` UI + BLE + analytics, `android/app/src/` Health Connect / Gemini Nano / step counter).

## Bike BLE

- FTMS Indoor Bike Data `0x2AD2`
- Heart Rate `0x180D` / Measurement `0x2A37`
- Manual resistance knob (no electronic ERG)

No dummy ride history. Analytics stay empty until you finish a ride.
