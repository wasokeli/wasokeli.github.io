for scanning paper:

- go to your local library, maybe they have a scanner
- use a scanner phone app, such as Adobe Scan


# nasin #1 (requires guess-and-check, but good results)

for making colored lines darker, and monochrome lines lighter:

1. Krita > Filter > Adjust > Cross-channel adjustment curves...
2. Channel: Lightness
3. Driver Channel: Saturation
4. Input: 0  (start at 0, fiddle with it if needed)
5. Output: 0  (start at 0, fiddle with it if needed)
6. click "Create Filter Mask". this lets you adjust the Input and Output values after the fact


# nasin #2 (less work for you, but may look aliased)

for scanning colored marker/pen and ensuring it's dark enough:

1. Krita > Filter > Adjust > Threshold > move the slider until it looks good

optional for cleaning up a bunch of stray black pixels:

2. move the Threshold slider until it looks *really* good, *but* has a bunch of stray black pixels. we delete those automatically in the following steps!
3. Krita > Filter > Start G'MIC-Qt
4. search for Morphological Filter
5. set Action from "Erosion" to "Closing"
6. set Kernel from "Square" to "Circular"
7. set Size to 2, or like 5 maybe. bigger numbers delete bigger blobs of pixels, but also delete thin strokes

note that the Threshold filter removes antialiasing, making the resulting font look kinda pixelated. nasin #1 avoids this.
