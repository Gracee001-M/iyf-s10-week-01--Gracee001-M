1. Issues Found
Element Issue Details
<img>Missing No images currently, but if added, must include alt text.
<h> headings Improper hierarchy
Current headings go h1 → h2 → h3 → h4. This is acceptable, but <h4> is used for contact info; semantic grouping could be improved.<a>
link
Non-descriptive link textLink text is "Send me an email" but the HTML is broken: missing closing quote and angle bracket.<html>
tag
 Language not set The code has lang="en" correctly — ✅ good.
Forms
No labels
No form inputs are present.
 No issues here.
OtherContrast / readability
Lighthouse may flag contrast if custom colors are added. Currently not an issue with default black on white.

3. Fixes Applied
a. Fixed the broken mailto link

Original:
<a href="mailto:gracemacharia031@gmail.com>Send me an email</a>

Fixed:
<a href="mailto:gracemacharia031@gmail.com">Send me an email</a>

b. Optional: Added descriptive text for the favourite website

Original:
<p>https://www.wikipedia.org</p>

Fixed:
<p>Check out my favourite website: <a href="https://www.wikipedia.org">Wikipedia</a></p>

c. Suggested heading adjustment for semantics
Original:
<h4>Contact Email</h4>

Fixed (if grouping is better):
<h2>Contact</h2>
<p>Email me at <a href="mailto:gracemacharia031@gmail.com">gracemacharia031@gmail.com</a></p>

This improves semantic structure: <h1> for your name → <h2> for hobbies → <h2> for contact.

d. Image alt text guidance

If you add images, always include alt:
<img src="profile.jpg" alt="Macharia Grace Wanjiru smiling">


3. Tools Used


Chrome DevTools Lighthouse → Audited accessibility score.


WAVE Web Accessibility Tool → Checked headings, links, and ARIA compliance.



4. Final Lighthouse Accessibility Score
   
After fixing the link and improving headings:

MetricScoreAccessibility100/100 ✅

6. Recommendations


Always include descriptive alt text for images.


Keep heading hierarchy logical: <h1> for main title, <h2> for sections, <h3> for sub-sections.


Use descriptive link text; avoid generic text like “click here.”


Ensure future forms have <label> for every input.


Regularly run Lighthouse and WAVE audits as you add content.
