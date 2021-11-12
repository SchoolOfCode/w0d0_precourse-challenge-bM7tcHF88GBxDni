# School Of Code fCC Tribute Page
As part of the School Of Code's pre-course pre-requisites we were asked to create a tribute page from the foundational HTML and CSS skills we picked up while completing freeCodeCamp's [Responsive Web Design](https://www.freecodecamp.org/learn/responsive-web-design/) module. 

## Development
I decided to apply some of the new flexbox and CSS3 visual design I'd picked up from fCC and also came across naturally while building the website and debugging issues. I chose the subject of Star Trek Deep Space Nine because it's a great show that remains unbeaten.

### Notable Feature:
- Some nice CSS3 tricks allow the header text to have a parallax texture, although I was unsure how I could make this compatible in Firefox- it has an unintended but otherwise nice effect too. Thought I'd note another very amusing issue where Firefox will stop rendering this section if it is hidden by scrolling down for some time.
- Flexbox is used in an unordered list to show off most of the TV shows main cast
- The header text cannot be highlighted but it's not an image! This is to prevent an issue with Firefox where highlighting header text then scrolling would break it's position until a page refresh.
- The header and flexbox elements also require several media width queries to prevent overlapping text. This could be better implement with CSS variable or calculations.

## Failing the fCC Tribute Page tests
This project actually partially failed a test:
1. The <img> element should responsively resize, relative to the width of its parent element, without exceeding its original size. [FAIL]

`Use the "display" style property with a value of "block" for responsive images.: expected 'inline' to equal 'block'...`

2. The <img> element should be centered within its parent element. [PASS]

However, I believe my `#image` element *is* responsive. Adding `display: block;` to `#image` does not change behaviour but passes the test so I've done that.
