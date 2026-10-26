# DevTools Verification Note

I inspected the following elements in the browser DevTools and made adjustments based on the box model and layout findings:

1. **Box Model Inspection (`.about-section`):** I verified that the `border-radius` and `box-shadow` were applying correctly. I ensured the absolute `.badge` was positioned using top/right without overflowing the box.
2. **Overflow Inspection (`.long-text-example`):** I tested the text overflow. The box model showed the content exceeding the width, so I applied `text-overflow: ellipsis` and `overflow: hidden` to truncate it cleanly.
3. **Float Layout (`.container`):** Inspected the `#skills` and `#education` floats. Ensured the container cleared them properly, preventing the footer from overlapping.
4. **Table Layout (`table`):** Verified the `border-collapse: collapse` was applied. Checked the `:nth-child(even)` selector to confirm alternating row colors were calculating correctly in the DOM.
5. **Sticky Nav (`.navigation`):** Inspected the `.navigation` element. Verified that `z-index: 100` keeps it above the scrolling page content and that `scroll-padding-top` prevents the nav from hiding anchor headings.