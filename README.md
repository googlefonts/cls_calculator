# cls_calculator
Computes a set of CSS values suitable for use in a CLS fallback face. Basically https://www.industrialempathy.com/perfect-ish-font-fallback/?font=Montserrat adjusted to fit my specific needs.

At time of writing page requires Chrome Canary, see:

1. https://caniuse.com/mdn-css_at-rules_font-face_size-adjust
1. https://caniuse.com/mdn-css_at-rules_font-face_ascent-override

Scaling will be quite poor unless both are supported.

## Try it

1. Clone repo
1. Start an http server in the directory, e.g. `python3 -m http.server 8010`
1. Using Chrome Canary, load http://localhost:8011/offset_sizing.html?web=Lato&local=Roboto
    * You need Chrome 92+
    * local should be something that local() will match; we do NOT confirm this
    * Use a Mac, currently haven't filled out any data for non-Mac
1. In Chrome Console, copy the textproto using something like `copy($$('.snippet').map(e => e.innerText).join('\n'))`
    * https://developer.chrome.com/docs/devtools/remote-debugging/ can be used to snapshot Android values

## Family Matching Notes

On Mac Impact only has Regular.

On Mac Open Sans weights don't quite match Avenir Next weights.

## References

* https://web.dev/cls/
* https://www.industrialempathy.com/posts/high-performance-web-font-loading/#tool%3A-perfect-ish-font-fallbacks
