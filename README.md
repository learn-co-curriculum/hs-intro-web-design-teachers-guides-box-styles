###SWBATS
+ CSS - include comments
+ CSS - understand how to use gradient and how to make it cross-browser friendly
+ CSS - Use background properties for box styling
+ CSS - understand how to use opacity and how to make it cross-browser friendly
+ CSS - understand and utilize border property for box styling, including border radius and box shadow
+ CSS - utilize text declarations
+ CSS - understand how to use scaling elements - px, em, % - and min and max

###Motivation
Let's pimp out your site with box styles, audio and video tags, and sprites! 

###Lesson Plan
+ We’ve covered changing the background color and adding a background image but here is a list of properties that you can give it:
  + `background-color: black | #fff | rgba(0,0,0,1);`
  + `background-image: url(myimage.jpg);`
  + `background-position: top left;`
  + `background-repeat: repeat | repeat-x | repeat-y | no-repeat;`
  + `background-scroll: fixed | scroll;`
  + `background-size: 100% | 1px | 1em | contain | cover;`
  + `background: white url(myimage.jpg) no-repeat;`
+ A few cool properties to point out:
  + `background-scroll` - if you set it to fixed you’ll have a fixed image background which can be nice
  + `background-size` - cover can be used to resize your image to cover the page
  + `background` - you can use this to apply the top 4 properties at once
+ We’ve mentioned borders but here is a review of how it works:
  + `border-size: 1% | 1px | 1em;`
  + `border-color: blue | #00f | rgba(0,0,255,1);`
  + `border-style: solid | dashed | dotted | double | groove | ridge | inset | outset;`
  + `border: 1px solid #000;` - combines size, style, and color
  + Notice there are lots of options for border-style and that there is a border property that can be used to set all properties at once.
+ We can also set how our corners look and round out their edges a bit with border-radius property.
+ Here are some examples of how you can modify the look of your divs with the border radius property:

<img src= "https://s3.amazonaws.com/after-school-assets/css-selector3.png">

+ Not all browsers support border radius so we use something called browser prefixes to make sure that out CSS is compatible across browsers:
  HTML:
  ```html
    <div></div>
  ```
  CSS:
  ```css
  div {
    -webkit-border-radius: 20px;
    -moz-border-radius: 20px;
    border-radius: 20px;
  }
  ```
+ We can also set box shadows on our divs like this:

<img src="https://s3.amazonaws.com/after-school-assets/css-selector4.png">

+ Explain each of the properties and emphasize the prefixes.
  + `box-shadow: horizontal-offset, vertical-offset, blur-radius, color`
+ We can also set the opacity of our div for effects like this:

<img src="https://s3.amazonaws.com/after-school-assets/css-selector5.png">

+ Here are the ways that you can do that for different browsers:
```css
  div {
    filter: alpha(opacity=50); /* IE*/
    -moz-opacity: 0.5; /* Older than Firefox 0.9 */
    -khtml-opacity: 0.5; /* Safari 1.x (pre WebKit!) */
    opacity: 0.5; /* Modern! */
  }
```
+ One last thing that we can do is set a gradient to the background of our divs. 
+ Here are some examples of how we would do that:
  Linear Gradient (top to bottom):
  ```css
  div {
    background: -webkit-linear-gradient(red, blue); /* For Safari 5.1 to 6.0 */
    background: -o-linear-gradient(red, blue); /* For Opera 11.1 to 12.0 */
    background: -moz-linear-gradient(red, blue); /* For Firefox 3.6 to 15 */
    background: linear-gradient(red, blue); /* Standard syntax */
}

  + Horizontal Gradient (right to left):
  ```css
  div {
    background: -webkit-linear-gradient(left, red , blue); /* For Safari 5.1 to 6.0 */
    background: -o-linear-gradient(right, red, blue); /* For Opera 11.1 to 12.0 */
    background: -moz-linear-gradient(right, red, blue); /* For Firefox 3.6 to 15 */
    background: linear-gradient(to right, red , blue); /* Standard syntax */
  }
  ```
+ It’s way easier to just use a gradient generator like this: http://www.colorzilla.com/gradient-editor/ 



##Conclusion / So What?

### Hints and Hurdles
<a href='https://learn.co/lessons/hs-intro-web-design-teachers-guides-box-styles' data-visibility='hidden'>View this lesson on Learn.co</a>
