# DevTools Layout Verification

I used browser DevTools to inspect the box model and layout behavior of the page:

1. **Box Model Panel:** Inspected `.content-box-example` to verify that with `box-sizing: content-box`, the 300px width does not include the 20px padding and 5px border (total computed width is 350px).
2. **Computed Styles:** Checked `.profile-header` to confirm `position: relative` is active and calculating correctly.
3. **Element Dimensions:** Verified `.container` max-width of 900px is respected on large screens and scales to 90% on smaller screens.
4. **Overflow Inspection:** Tested the `.long-text-example` to ensure `text-overflow: ellipsis` truncates the long word properly.
5. **Positioning:** Verified `.scroll-top-btn` uses `position: fixed` and stays at the bottom-right corner during scrolling.
