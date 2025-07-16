### Semantic HTML Review

## Importance of Semantic HTML
- <b>Structural hierarchy for heading elements: </b> It is important to use the correct heading element to maintain the structural hierarchy of the content. The `h1` element is the highest level of heading and the `h6` element is the lowest level of heading.

- <b>Presentational HTML elements:</b> Elements that define the appearance of content. Ex. the deprecated center, big and font elements.

- <b>Semantic HTML elements:</b> Elements that hold meaning and structure. Ex. header, nav, figure.

## Semantic HTML Elements
- <b>Header element:</b> used to define the header of a document or section.
- <b>Main element:</b> used to contain the main content of the web page.
- <b>Section element:</b> used to divide up content into smaller sections.
- <b>Navigation Section (nav) element:</b> represents a section with navigation links.
- <b>Figure element:</b> used to contain illustrations and diagrams.
- <b>Emphasis (em) element:</b> marks text that has stress emphasis.

Example Code
```html
<p>
  Never give up on <em>your</em> dreams.
</p>
```

- <b>Idiomatic Text (i) element:</b> used for highlighting alternative voice or mood, idiomatic terms from another language, technical terms, and thoughts.

Example Code
```html
<p>
  There is a certain <i lang="fr">je ne sais quoi</i> in the air.
</p>
```

The `lang` attribute inside the open `i` tag is used to specify the language of the content. In this case, the language would be French. The `i` element does not indicate if the text is important or not, it only shows that it's somehow different from the surrounding text.

- <b>Strong Importance (strong) element:</b> marks text that has strong importance.

Example Code
```html
<p>
  <strong>Warning:</strong> This product may cause allergic reactions.
</p>
```

- <b>Bring Attention To (b) element:</b> used to bring attention to text that is not important for the meaning of the content. It's commonly used to highlight keywords in summaries or product names in reviews.

Example Code
```html
<p>
  We tested several products, including the <b>SuperSound 3000</b> for audio quality, the <b>QuickCharge Pro</b> for fast charging, and the <b>Ecoclean Vacuum</b> for cleaning. The first two performed well, but the <b>Ecoclean Vacuum</b> did not meet expectations.
</p>
```

- <b>Description List (dl) element:</b> used to represent a list of term-description groupings.
- <b>Description Term (dt) element:</b> used to represent the term being defined.
- <b>Description Details (dd) element:</b> used to represent the description of the term.

Example Code
```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```

- <b>Block Quotation (blockquote) element:</b> used to represent a section that is quoted from another source. This element has a cite attribute. The value of the cite attribute is the URL of the source.

Example Code
```html
<blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
  "Can you imagine what it would be like to be a successful developer? To have built software systems that people rely upon?"
</blockquote>
```

- <b>Citation (cite) element:</b> used to attribute the source of the referenced work visually. Marks up the title of the reference.

Example Code
```html
<div>
  <blockquote cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    "Can you imagine what it would be like to be a successful developer? To have built software systems that people rely upon?"
  </blockquote>
  <p>
    -Quincy Larson, <cite>How to learn to Code and Get a Developer Job [Full Book].</cite>
  </p>
</div>
```

- <b>Inline Quotation (q) element:</b> used to represent a short inline quotation.

Example Code
```html
<p>
  As Quincy Larson said,
  <q cite="https://www.freecodecamp.org/news/learn-to-code-book/">
    Momentum is everything.
  </q>
</p>
```

- <b>Abbreviation (abbr) element:</b> used to represent an abbreviation or acronym. To help users understand what the abbreviation or acronym is, you can show its full form, a human readable description, with the title attribute.

Example Code
```html
<p>
  <abbr title="HyperText Markup Language">HTML</abbr> is the foundation of the web.
</p>
```

- <b>Contact Address (address) element:</b> used to represent the contact information.
- <b>(Date) Time (time) element:</b> used to represent a date and/or time. The datetime attribute is used to translate dates and times into a machine-readable format.

Example Code
```html
<p>
  The reservations are for the <time datetime="20:00">20:00 </time>
</p>
```

- <b>ISO 8601 Date (datetime) attribute:</b> used to represent dates and times in a machine-readable format. The standard format is `YYYY-MM-DDThh:mm:ss`, with the capital `T` being a separator between the date and time.

- <b>Superscript (sup) element:</b> used to represent superscript text. Common use cases for the `sup` element would include exponents, superior lettering and ordinal numbers.
Example Code
```html
<p>
  2<sup>2</sup> (2 squared) is 4.
</p>
```

- <b>Subscript (sub) element:<b> used to represent subscript text. Common use cases for the subscript element include chemical formulas, footnotes, and variable subscripts.

Example Code
```html
<p>
  CO<sub>2</sub>
</p>
```

- <b>Inline Code (code) element:</b> used to represent a fragment of computer code.

- <b>Preformatted Text (pre) element:</b> represents preformatted text

Example Code
```html
<pre>
  <code>
    body {
      color: red;
    }
  </code>
</pre>
```

- **Unarticulated Annotation (u) element:** used to represent a span of inline text which should be rendered in a way that indicates that it has a non-textual annotation.

Example Code
```html
<p>
  You can use the unarticulated annotation element to highlight
  <u>inccccort</u> <u>spling</u> <u>issses</u>.
</p>
```

- **Ruby Annotation (ruby) element:** used for annotating text with pronunciation or meaning explanations. An example usage is for East Asian typography.
- **Ruby fallback parenthesis (rp) element:** used as a fallback for browsers lacking support for displaying ruby annotations.
- **Ruby text (rt) element:** used to indicate text for the ruby annotation. Usually used for pronunciation, or translation details in East Asian typography.

Example Code
```html
<ruby>
  明日 <rp>(</rp><rt>Ashita</rt><rp>)</rp>
</ruby>
```

- **Strikethrough (s) element:** used to represent content that is no longer accurate or relevant.

Example Code
```html
<p>
  <s>Tomorrow's hike will be meeting at noon.</s>
</p>
<p>
  Due to unforeseen weather conditions, the hike has been canceled.
</p>
```

