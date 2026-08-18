# Haykal

Haykal is a local Adobe Illustrator CEP extension that turns selected vector
artwork into organized logo-construction graphics.

**Free beta version:** 0.3.6  
**Release date:** 2026-08-18

## Main functions

- Build structural guides, construction curves, nodes, handles, bounds, centre
  marks, clear-space guides, and outlines.
- Add overall dimensions, segment lengths, line and approximate arc angles, and
  proportional measurements.
- Generate uniform or directional clear space from a logo element, percentage,
  or custom value.
- Present clear space with a cyan (`#00B7D6`) default, natural-size gray X
  references, a gray logo reference, outward arrows, and readable labels.
- Adjust colours, line weight, opacity, marker shapes, guide style, and
  measurement labels.
- Use compact Adobe-style up/down controls for every numeric field.

## Compatibility

The extension manifest accepts Adobe Illustrator versions **29.0 through
99.9**. Haykal has not been tested inside every version in that range, so test
its generated artwork before using it in an important client file.

The project provides CEP installation paths and behavior for **macOS and
Windows**. No specific operating-system release matrix has been verified.

## Install on macOS

1. Close Adobe Illustrator.
2. Extract `haykal-beta.zip`.
3. Keep `install mac.sh` beside the `com.haykal.tariqdesign` folder.
4. Open Terminal in the extracted directory and run:

   ```sh
   chmod +x "install mac.sh"
   ./"install mac.sh"
   ```

5. Restart Illustrator completely.
6. Open **Window → Extensions → Haykal**.

The installer uses the macOS user CEP location:
`~/Library/Application Support/Adobe/CEP/extensions/`.

## Install on Windows

1. Close Adobe Illustrator.
2. Extract `haykal-beta.zip`.
3. Keep `install windows.bat` beside the `com.haykal.tariqdesign` folder.
4. Double-click `install windows.bat`.
5. Restart Illustrator completely.
6. Open **Window → Extensions → Haykal**.

The installer uses the Windows user CEP location:
`%APPDATA%\Adobe\CEP\extensions\`.

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
