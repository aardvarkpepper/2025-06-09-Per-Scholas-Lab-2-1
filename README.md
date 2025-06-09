# Reflection Questions (and Answers)

1.  What accessibility enhancements were the most challenging to implement, and why?
2.  How do ARIA attributes improve the experience for users relying on assistive technologies?
3.  What tools did you use to check color contrast, and how did they help?

1.  Text to background contrast was one of the more challenging accessibility features for me to implement, as significant changes compromising intent of a feature may be required.  E.g. placeholder text on a white background is by default light gray as opposed to black, making it clear the text is placeholder text.  But accessibility requires high contrast between text and background, so placeholder text is made darker.  Making the placeholder text darker, though, makes it harder to distinguish between placeholder and entered text, which is contrary to the reason for making the placeholder text light gray in the first place.
2.  Semantic HTML elements such as button, a (hyperlink), nav, header, footer, main, and so forth, provide structural elements to screen readers.  Some elements, though, are not readily understood by screen readers, such as toggle switches, sliders, or unique input elements; for such elements, ARIA attributes may be assigned to help screen readers navigate.
3.  I used [WebAIM](https://webaim.org/resources/contrastchecker/) to check color contrast.  It's useful to have such tools to provide specific numbers on color contrast, so the desired 7:1 contrast difference is achieved.