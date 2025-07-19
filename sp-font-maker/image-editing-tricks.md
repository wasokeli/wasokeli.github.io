for scanning paper:
- go to your local library, maybe they have a scanner
- use a scanner phone app, such as Adobe Scan

for scanning colored marker/pen and ensuring it's dark enough:
1. Krita > Filter > Adjust > Desaturate > Min (for the darkest of the 3 color channels)
2. Krita > Filter > Adjust > Threshold > move the slider until it looks good

optional for cleaning up a bunch of stray black pixels:
2. move the Threshold slider until it looks *really* good, *but* has a bunch of stray black pixels
3. Krita > Filter > Start G'MIC-Qt
4. search for Morphological Filter
5. set Action from "Erosion" to "Closing"
6. set Kernel from "Square" to "Circular"
7. set Size to 2, or like 5 maybe. bigger numbers delete bigger blobs of pixels, but also delete thin strokes