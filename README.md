Hamza's Portfolio:

Links:

- Live site: https://hamzaalsamraaie.github.io/hamza-portfolio/ (not confirmed working yet)
- Repository: https://github.com/hamzaalsamraaie/hamza-portfolio.git

Current Progress:

- Home page complete
- About Me page complete (photo and introduction video added)
- Projects page complete (five projects)
- Contact Me page complete
- Shared, laptop, tablet and mobile stylesheets complete
- GitHub Pages deployment pending, live site not confirmed working yet

Files:

- index.html
- about.html
- projects.html
- contact.html
- css/style.css
- css/laptop.css
- css/tablet.css
- css/mobile.css
- IMG_4533.jpeg: my photo
- poster.png: image shown before the video plays
- media/introduction.mp4: my introduction video, recorded by me

Viewports:

- laptop.css: min width 960px. Nav floats on the left, content on the right, two boxes per row
- tablet.css: 481px to 959px. Nav stacks above the content as a two by two block of buttons, two boxes per row
- mobile.css: max width 480px. Everything in one column, large stacked buttons, one box per row
- These sizes come from the Week 3 lecture, which lists phones as 480px or narrower, tablets as 481px to 960px and laptops as 960px or wider
- Tablet ends at 959px so only one stylesheet applies at any width
- Widths are percentages so the layout stretches and shrinks with the screen. No Flexbox is used, only floats and clear

Gradients:

- Direction based: #banner in style.css, to bottom, #14365B to #1F6F8B
- Angle based: #footer in style.css, 45deg, #14365B to #1F6F8B

Colours:

I used the Complementary harmony rule in Adobe Color, with navy and teal blues as the main colours and an amber accent, since blue and orange sit opposite each other on the colour wheel. Blue suits a security portfolio and gives strong contrast with white text.

Adobe Color theme: PASTE YOUR LINK HERE

- #14365B: Navy, header and footer gradients, current page button, photo caption, form buttons
- #1F6F8B: Teal, links, nav buttons, end of both gradients
- #99C4D8: Steel blue, box borders and photo frame
- #E8A33D: Amber, button hover
- #DCE8EE: Page background
- #F2F6F8: Background inside the wrapper
- #1A1A1C: Main text colour

Contact Form:

- Name, Email, Cell Number and Comments are all required
- Email uses type email so the browser checks the format
- Cell Number must be exactly 10 digits, for example 9055550123
- Every label is connected to its field with matching for and id values
- The form uses a mailto action from the Week 2 lecture. Pressing Send opens the visitor's own email app with the form data filled in, and the visitor still has to send that email
- This only works if the visitor has an email app set up on their device. A note on the Contact page explains this
- GitHub Pages only hosts static files and cannot run a server script, so the form cannot send messages automatically

Deployment (pending):

- The project is pushed to the public GitHub repository with git
- To publish: in the repository, go to Settings, then Pages, choose Deploy from a branch, select main and the root folder, then save
- The live site has not been confirmed working yet

Testing:

- W3C Nu HTML Checker, October 9, 2026:
  - index.html: no errors or warnings
  - projects.html: no errors or warnings
  - contact.html: no errors or warnings
  - about.html: two errors found
    - The video source was src="Intro video.mp4". The space in the file name is not allowed in a URL. Fixed by moving the video to media/introduction.mp4 and updating the source
    - The photo caption used an h5 heading right after an h2, which skips heading levels. Fixed by replacing it with plain caption text
    - Revalidated about.html on October 9, 2026: no errors or warnings
  - Result: all four HTML pages checked with no errors or warnings
- W3C CSS Validation Service, October 9, 2026, CSS level 3 + SVG profile:
  - css/style.css: no errors found
  - css/laptop.css: no errors found
  - css/tablet.css: no errors found
  - css/mobile.css: no errors found
- W3C Link Checker, live site: pending
- WAVE accessibility, all four live pages: pending
- Spelling check: pending
- Form test, empty fields, bad email, letters or wrong length in the phone number, valid submit: pending
- Screen sizes 320, 375, 480, 481, 768, 959, 960 and 1366px in Chrome device tools: pending

Sources:

- Week 1 lecture: page template, wrapper, floats, box class, clear class, gradient syntax
- Week 2 lecture, semantic markup: header, nav, article, section, footer, address, figure and figcaption elements
- Week 2 lecture, native video: video element with controls, poster and fallback text
- Week 2 lecture, forms: mailto form, labels, required, email type, submit and reset buttons
- Week 3 lecture, responsive design: viewport meta tag, media queries, fluid widths, button class, separate viewport stylesheets
- Week 4 lecture: hover transitions on the buttons, text-align center
- MDN Web Docs, input pattern attribute (developer.mozilla.org): pattern="[0-9]{10}" on the phone field. This is the only HTML or CSS feature not taught in the lectures
- Claude (Anthropic), AI assistant: helped me adapt the lecture code to my layout, suggested the page structure and CSS, and explained how each part works. The code is based on the lecture examples but some of it was written with Claude's help. I reviewed and edited all of it
