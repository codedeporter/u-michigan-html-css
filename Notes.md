# Notes on html/css

# Tags

#### eg. headings which have syntax(look) and semantics(meaning), paragraph which can only contain inline elements, divs which group related content, ordered lists, unordered lists, line breaks, image,

## Semantic Tags
#### header(nav goes inside) - is a block tag, nav - links to other parts of the site, footer, img, figure, header, footer

## Containers
#### article, aside, section, main

## Block Tags
#### Containers, hr, address, blockquote(has cite attribute), details(not implemented in firefox), summary

## Inline Tags
#### span, cite, abbr(shows the full word on hover), time, code, sub, sup, a

## More Tags
#### button, meter(attributes are min, max, value), progress, iframe, bdo(attribute dir, goes left to right or right to left), <map> with <area>, 

### Other new tags
#### Structural Elements: article, aside, main, menuitem, summary, section
#### Form Elements: datalist, keygen, output
#### Input Types: color, date, email, list
#### Graphics Elements: canvas, svg
#### Media Elements: audio, embed, source, track, video


# Attributes
### Display attributes:
#### block(can take width and height); newline is inserted before and after so takes up the whole width 
#### inline(can NOT take width and height) Only uses as much space as needed to contain the element
#### table, grid, flexbox

### Tag attributes
#### img has src, alt, title, class
#### class, id, accesskey, tabindex, 

# Special Entities
#### &lt;, &gt;, &copy;, &nbsp;(blank space), &cent;, &amp;, 

# Images
#### jpeg(.jpg and .jpeg), gif, png, svg, bmp(bitmap)
#### all require an http request
#### resize the image with width and/or height attributes on the image itself with pixels or percentages
#### resize the image using an editor with a downloaded file(preview software on mac)
#### Benefits of using percentages is that the picture will shrink/grow along with the browser size
#### font awesome images - class="fas fa-angry fa-xs" will change the size of the icon, xs, md, lg, 2x, 3x, 5x, 10x etc.  fas means font awesome
#### material icons
#### icons are not accessible!!
#### fab fa-twitter fa-tx; fab fa-pinterest fa-5x; fab fa-linkedin fa-5x; links will be blue  fas can stand alone while fab need to be in a link???????
#### WAVE validation tool for accessibility
#### aria-label is the accessible attribute for links similar to alt is the accessible attribute for img


# Links
#### Are inline elements!! Needs a hyper-reference and content
#### Types: Absolute(full url in the href), Relative(only the filename in the href maybe a folder also), (using the # eg. #history), Graphical, internal
#### links should never be specific to your computer!!
#### Can use an image for your content eg.
#### eg. <a href="http://www.redcross.org"><img src="imgs/#### redcross-logo.png" alt = "Red Cross Logo"/></a> 

# Embedded Links
#### Use an ID to link to specific parts of a page so users can jump around your page faster

# Targets
#### Anchor links can take a target attribute
#### _self is the default action
#### _blank opens a new tabl or window
#### _top and _parent 

# Audio & Video Elements
## Video - uses src or <source> tag.  Attributes are width, height, autoplay, loop, controls.  Add text to the attributes is best practice.
## Audio - Uses src to link to .mp3 or .wav.  Attributes include autoplay, controls, loop, buffered, muted, volume, 

# Tables
## Attributes: colspan, rowspan, border


## Linking captions to a table
#### Use the <caption> tag


#### The four predominant types of disabilities: Visual, hearing, motor, cognitive
#### The four principles: perceivable, operable, understandable, robust

# Validate for syntax - validator.w3.org checks the syntax of your code

# Validate for accessibility - wave.webaim.org

# Hosting a site(using Cpanel)
#### Need a domain name - bought for a few years at a time, most common is .com but others exist
#### Need a hosting service - need a registered IP address to connect domain name to internet, 
#### https://beythost.com


# Secure File Transfer Protocol(FTP, SFTP)
#### HTTP is a display protocol
#### FTP is a transfer protocol
#### Install FTP client fugu/cyberduck for mac, winscp for windows
#### Find the ftp address for your hosting service from the email they sent you

# CCS3

## Inline styling
#### <h1 style="color:blue">Styled Heading Inline</h1>
#### Takes precedence

## External StyleSheet
#### selector { property: value;}
#### h1 { color: blue;}
#### Will be used last as a choice of the three
#### If multiple of these exist, the last one linked has precedence

## Internal StyleSheet(used for one page only best practice)
#### <style>color: blue;<style>
#### Will be used after inline styling

# Comments
#### //This is how comments are done in html
#### /* This is how comments are done in css */

# Color Conventions
#### Avoid using color names
#### Hexadecimal colors 16 digits #0-9A-F, 6 or 9 digits
#### rgb(g, r, b)
#### rgba(g, r, b, transparency) - alpha channel
#### Use colors to convey meaning over style but don't use color ALONE to convey meaning. Use alternate text or a caption also

# Styling Text for Max Impact
#### font( family, style, variant, size, color), background, alignment, line-height
#### Use sans-serif fonts when possible

## Custon Fonts
#### @font-face{ font-family: mySpecialName; src: url("dee.ttf");}
#### h1{ font-family: mySpecialName;}

## Font-style
#### normal, italic, oblique

## Font-variant
#### normal or small-caps

## Font Size
#### px, %, 200%, 150% etc.

#### color, background-color, text-align, font-size, line-height(line spacing between lines), 


# Common Display Values
#### inline: sits next to each other taking up just enough width and height, accepts no height or width
#### block: forces a line break between elements
#### inline-block: accepts height and width
#### none: gets removed from page
#### table(used for table-like layout without table structure.  Use display:table along with display:table-cell for elements), grid, flex



# Complementary Display Properties
#### Float: Repositions elements to the right or left, and removes them from their position, as the other elements move in to fill the old space.  Float right flipped the order of the elements - elements won't overlap, values are either left or right
#### Clear: Used to keep floating elements away, values are left, right, or both
#### Browser by default places things upper left hand corner

# Element Overflow
#### What happens when you set a height/width and the content doesn't fit any longer?
#### User the overflow property: visible, hidden, scroll, auto

# Visibility
#### Seen by user or not?
#### options: visible, hidden, collapse(tables)

# Box Model
## Height and Width
#### The height and width of any inline element is the content itself!!!!

## Border
#### All elements can have borders - style, width, color, style is mandatory

## Margin 
#### outside the border Can be positive or negative

## Padding
#### between element and border

# Center Text
#### text-align: center;

# Centering an element
#### center horizontally: margin: 0 auto - the element must be display: block, must not float, must not have a fixed or absolute position, must have a numerical width

# Box Sizing
#### content-box: default additive
#### border-box: width takes content, padding, and border into consideration

# Measurements - setting height and width
#### Absolute - set to a specific size px, mm, cm, pt etc
#### Fluid - sets size relative to surrounding elements %, vw, vh, em(font) - 1em = current size, rem(font) - 1rem = 16px(size of root element)

# Styling Links
#### text-decoration
#### links have states: a:link, a:visited, a:hover(doen't work on touch, phones etc), a:focus(activated with keyboard tabs), a:active(being clicked - adds border while holding down)
#### Rules: a:hover MUST come after a:link, a:visited and a:active MUST come after a:hover

# Styling Lists
#### Properties - font, margin, list-style-type, list-style-image, list-style-position, list-style

# Advanced Selectors
## Descendant selectors (nav a) - style all the anchor links inside a nav tag
## Child selectors (nav > a) - the anchor element must be a direct child of the nav
## Adjacent sibling (hl + ol) - elements must be at same level










