# Haykal

Haykal is a local Adobe Illustrator CEP extension that turns selected vector
artwork into organized logo-construction graphics.

**Free beta version:** 0.3.0  
**Release date:** 2026-08-18

## Main functions

- Build structural guides, construction curves, nodes, handles, bounds, centre
  marks, clear-space guides, and outlines.
- Add overall dimensions, segment lengths, line and approximate arc angles, and
  proportional measurements.
- Generate uniform or directional clear space from a logo element, percentage,
  or custom value.
- Adjust colours, line weight, opacity, marker shapes, guide style, and
  measurement labels.

## Compatibility

The extension manifest accepts Adobe Illustrator versions **29.0 through
99.9**. Haykal has not been tested inside every version in that range, so test
its generated artwork before using it in an important client file.

The project provides CEP installation paths and behavior for **macOS and
Windows**. No specific operating-system release matrix has been verified.

## Install on macOS

1. Close Adobe Illustrator.
2. Extract `haykal-beta.zip`.
3. Copy the complete `com.haykal.tariqdesign` folder to:
   `~/Library/Application Support/Adobe/CEP/extensions/`
4. Because this beta is unsigned, open Terminal and enable unsigned CEP panels:

   ```sh
   for V in 11 12 13 14 15; do defaults write "com.adobe.CSXS.$V" PlayerDebugMode 1; done
   ```

5. Restart Illustrator completely.
6. Open **Window → Extensions → Haykal**.

An administrator may alternatively install the same extension folder in
`/Library/Application Support/Adobe/CEP/extensions/`.

## Install on Windows

1. Close Adobe Illustrator.
2. Extract `haykal-beta.zip`.
3. Copy the complete `com.haykal.tariqdesign` folder to:
   `%APPDATA%\Adobe\CEP\extensions\`
4. Because this beta is unsigned, open Command Prompt and enable unsigned CEP
   panels:

   ```bat
   for %V in (11 12 13 14 15) do reg add "HKCU\Software\Adobe\CSXS.%V" /v PlayerDebugMode /t REG_SZ /d 1 /f
   ```

5. Restart Illustrator completely.
6. Open **Window → Extensions → Haykal**.

An administrator may alternatively install the same extension folder in
`C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\`.

## Manual uninstall

The ZIP version must be uninstalled manually:

1. Close Illustrator.
2. Delete only the `com.haykal.tariqdesign` folder from the location where it was
   installed. Do not delete the complete CEP `extensions` directory.
3. Restart Illustrator.

Possible locations are:

- macOS user: `~/Library/Application Support/Adobe/CEP/extensions/com.haykal.tariqdesign`
- macOS system: `/Library/Application Support/Adobe/CEP/extensions/com.haykal.tariqdesign`
- Windows user: `%APPDATA%\Adobe\CEP\extensions\com.haykal.tariqdesign`
- Windows system: `C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\com.haykal.tariqdesign`

## Support and status

Haykal is provided as a free proprietary beta. Continuous technical support is
not currently provided. Construction-circle fitting, curved-angle labels, and
automatic annotation placement may require manual review.

Copyright © 2026 Tariq Yosef.  
Website: https://tariqdesign.com
