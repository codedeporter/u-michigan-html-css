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
#### span, cite, abbr(shows the full word on hover), time, code, sub, sup

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

### Tag attributes
#### img has src, alt, title, class
#### class, id, accesskey, tabindex, 

# Special Entities
&lt;, &gt;, &copy;, &nbsp;(blank space), &cent;, &amp;, 

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
#### Needs a hyper-reference and content
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

# Hosting a site
#### Need a domain name - bought for a few years at a time, most common is .com but others exist
#### Need a hosting service - need a registered IP address to connect domain name to internet, 
#### https://byethost.com



