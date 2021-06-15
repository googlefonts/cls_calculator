# cls_calculator
Computes a set of CSS values suitable for use in a CLS fallback face. Basically https://www.industrialempathy.com/perfect-ish-font-fallback/?font=Montserrat adjusted to fit my specific needs.

At time of writing page requires Chrome Canary, see:

1. https://caniuse.com/mdn-css_at-rules_font-face_size-adjust
1. https://caniuse.com/mdn-css_at-rules_font-face_ascent-override

Scaling will be quite poor unless both are supported.

## Try it

1. Clone repo
1. Start an http server in the directory, e.g. `python3 -m http.server 8010`
1. Using Chrome Canary, load http://localhost:8010/offset_sizing.html (assuming server started as above)

## Family Matching Notes

On Mac Impact only has Regular.

On Mac Open Sans weights don't quite match Avenir Next weights.
