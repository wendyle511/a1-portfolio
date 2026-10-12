--Readme document for Wendy Le, wle7@uci.edu--

A reminder on academic integrity, as described in the syllabus.

In general, the course staff expects that you will look at code and examples from many online resources as part of the assignments, particularly to resolve syntax and understand frameworks. We expect that you'll use other libraries you find, and will even require it in some assignments. These practices are often critical to the work of developers today. The best developers are adept at interpreting the examples they see, customizing them to their specific situation, and citing their sources so they can find them later. We expect you to do the same.

While learning from examples is encouraged, attempting to pass an existing project or example from the web as your own is not allowed. If you ever have a question about what is or is not appropriate, feel free to ask the course staff!

Talking to classmates about class material, assignment requirements, etc. is a great way to verify ideas and get feedback. But this distinctly does *not* permit attempting to pass off someone else's code as your own. Talking over ideas and approaches is allowed, but the work that you produce and submit must be your own.

1. How many assignment points do you believe you completed (replace the *'s with your numbers)?

10/10
- 1/1 Readme
- 2/2 Basic HTML content
- 1/1 Basic CSS styling
- 1/1 Advanced feature
- 2/2 Responsive layout
- 1/1 Passes validation checks
- 2/2 Embraces spirit of the assignment

2. What (a) basic features, (b) CSS features, and (c) advanced features did you include in your portfolio?

(a) Basic features
- An image with a descriptive alt attribute (my profile photo, images/wendy.jpeg, on the home page)
- Appropriate headings and paragraph text on all three pages
- Links to external pages (my GitHub repositories, GitHub profile, LinkedIn, and a mailto email link)
- Multiple pages with navigation between them (index.html, projects.html, contact.html)
- Semantic HTML tags (header, nav, main, section, article, footer)
- Custom icons (inline SVG icons for GitHub and email)

(b) CSS features
- Padding and margins to indent content and improve readability
- A blue and white color scheme defined with CSS variables
- Custom Google Fonts (Lora for headings, Nunito for body text) with fallback fonts (Georgia/serif and Segoe UI/Arial/sans-serif)

(c) Advanced features
- A data table of my skills that works with screen readers (caption, thead/tbody, scope, and id/headers attributes)
- A more complex page layout: a sticky navigation bar that marks the current page with aria-current, plus a skip-to-main-content link
- Nested selectors for the project cards (for example .project .tags li and .project ul.details li)
- A contact form using HTML forms with labels, required fields, and autocomplete
- A responsive layout using CSS grid, flexbox, and media queries (breakpoints at 800px and 520px). The hero stacks on small screens, the project cards become one column, and the skills table scrolls inside its own box so the page never scrolls sideways.

3. Did you ignore any of the warnings or errors presented by the accessibility checker? If so, why does this not seem like an accessibility concern? If it's useful, you can consolidate your thoughts on multiple warnings/errors if the rationale is similar.

AChecker reported 0 known problems and 0 likely problems on index.html, projects.html, and contact.html. It also listed potential problems (manual checks). I reviewed them and did not change anything because they do not apply or are already handled:
- Image checks (alt text, decorative image, long description, text in image): my photo has descriptive alt text, is not decorative, and contains no text.
- Text direction, language parts, and Unicode direction marks: all content is English and left-to-right, and each page sets lang="en".
- Visual lists and groups of links: the navigation, tags, and project details use real ul/li lists, and the main links are inside a nav element with an aria-label.
- Skip link, consistent navigation, and site map: every page has a skip link and the same nav bar in the same order. The site has only three pages, all linked from the nav, so a site map is not needed.
- Page titles, headings, and link text: each page has a unique descriptive title, the headings are used for structure in a logical order (h1, h2, h3) and not for styling, and the link text is meaningful in context.
- Table checks (summary, colgroup, and so on): the skills table is a real data table with a caption, proper header cells, and id/headers attributes. It is simple enough that a summary or colgroup would not add information.
- Sensory characteristics and blockquote: nothing relies on shape or position to be understood, and there are no long quotations.
- Contact form checks: every field has a visible label connected with for/id, placed directly above the field, and required fields use the required attribute so the browser reports empty ones. The form uses a mailto action, so there is no server-side submission or data deletion to handle.
- Use of color alone: fields are identified by labels and borders, not color alone, and keyboard focus is clearly outlined.

4. How long, in hours, did it take you to complete this assignment?

It took me approximately 8 hours to complete this assignment.

5. What online resources did you consult when completing this assignment? (list specific URLs, describe queries to Generative AI, or use of AI-based code completion)

Websites:
- https://fonts.google.com (to choose and load Lora and Nunito)
- https://validator.w3.org (HTML validation)
- https://jigsaw.w3.org/css-validator/ (CSS validation)
- https://achecker.ca (accessibility checking)

Generative AI (Claude, by Anthropic):
- I asked about page structure, how many pages the assignment allows, and which Google Font pairings pass the validators, and I asked for a visual comparison of font pairings before choosing Lora and Nunito.
- I pasted validator and AChecker error messages (a skipped heading level on the projects page and a table id/headers error on the home page) and asked it to fix them.
- I asked it to help organize the submission folder.

6. What classmates or other individuals did you consult as part of this assignment? What did you discuss?

None. I worked on this assignment on my own.

7. Is there anything special we need to know in order to run your code?

- Open index.html directly in a browser. No packages or installs are needed, and all file paths are relative.
- The Google Fonts load from the internet. Without a connection, the site falls back to Georgia and Arial and still looks fine.
- The contact form uses a mailto: action, so pressing "Send message" opens the visitor's email app instead of sending the message directly.
