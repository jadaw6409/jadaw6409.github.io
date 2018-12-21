---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of Greece

## Describe your program
- In my I was able to create the flag of Greece with the help of my teacher. I believe I should at most receive the grade of a practitioner because I was able to create the code and assemble the flag with lots of time and effort put into this project as well.

## Current output
- my current 
* * *
![Flag](/images/http://flags.fmcdn.net/data/flags/w580/gr.png)
* * *

## Describe your process.
- In the beginning of the project I was having a hard time understanding and processing how to create the flag ratios. After creating the basic code,like height/width/size and other adjustments I was then able to make the actual shape like a stripes on the flag or one of the symbols needed to form the flag of Greece. Some strategies I used was working with my teacher Mr.Allata to first know what we were trying to solve and "break the big problems into smaller pieces". Later when I did the program my main focus was making the cross because it was what tied the flag itself together. Also after knowing what I needed to do and make it somewhat became easier to answer questions on what I had to change but I overall struggled with some basic concepts because I was unsure if I was taking the "right step".

## Explain your code.
- So as you can see this is a section of my program, 
```size=100 
height= size * 2
width= size * 3 

stripe-height= 2/18 * height
white-height= 8/18 * size 
blue-height= 10/18 * size
square-height= 10/18 * height

blue= rectangle(width , height, "solid","blue")
#br= place-image()
white= rectangle(width,stripe-height,"solid","white")

base=place-image(white, 1/2 * width, 1.5 * stripe-height, 
  place-image(white, 1/2 * width, 3.5 * stripe-height, 
    place-image(white, 1/2 * width, 5.5 * stripe-height, 
      place-image(white, 1/2 * width, 7.5 * stripe-height, blue))))

five-stripe = 5 * stripe-height
```
Within this section of 15 lines of the program you are able to know the size,width,height,stripe-height and much more about my flag. The first thing needed to make the flag was the size because without a scaled size the stripes and symbols would not be aligned. We created a segment called Stripe-height,blue-height,white-height,square-height because on the flag of Greece there are stripes that contain a particular width and height. So using measurements given to me I was able to know that the stripes take up about 2/18 of the flag. So each stripe is 2/18 (height) of the flag, we also know that everything in that area associated with height is creating a height put. For example white-height that is making a height of the white cross used in the flag, blue-height creates the height of the square. But the lower half is were I put the pieces together, I had to make the stripes by overlapping the white rectangles over the blue rectangle, then increase the height so the blue would still be visable. Independently the section where it tells you the heights they count as numbers, so if they are not placed together it would give you just a decimal in return. 

* * *

```size=100 
height= size * 2
width= size * 3 

stripe-height= 2/18 * height
white-height= 8/18 * size 
blue-height= 10/18 * size
square-height= 10/18 * height

blue= rectangle(width , height, "solid","blue")
#br= place-image()
white= rectangle(width,stripe-height,"solid","white")

base=place-image(white, 1/2 * width, 1.5 * stripe-height, 
  place-image(white, 1/2 * width, 3.5 * stripe-height, 
    place-image(white, 1/2 * width, 5.5 * stripe-height, 
      place-image(white, 1/2 * width, 7.5 * stripe-height, blue))))

five-stripe = 5 * stripe-height

blue-square = square(five-stripe,"solid","blue")

horizontal-cross = rectangle(five-stripe,stripe-height,"solid","white")

vertical-cross = rectangle(20,100,"solid","white")

cross = overlay(horizontal-cross, vertical-cross)

blue-cross = overlay(cross, blue-square)

piece = overlay(cross,blue-cross)

flag = overlay(piece,base)

place-image(piece,50,55,base)
```
* * *
- The flag I created was Greece in this flag it had 9 lines of stripes and I learned that the blue square with the cross took up 5 stripes/lines of the flag itself in the top left corner. In the program I had to use the width of each stripe and create the height of the square so the placement was at most perfect. In addition I also had to create a defintion and funtion called ```vertical-cross and horizontal-cross``` so that the rectangles which make the cross align in the center to actually make the cross. 

## Program code
```
size=100 
height= size * 2
width= size * 3 

stripe-height= 2/18 * height
white-height= 8/18 * size 
blue-height= 10/18 * size
square-height= 10/18 * height

blue= rectangle(width , height, "solid","blue")
#br= place-image()
white= rectangle(width,stripe-height,"solid","white")

base=place-image(white, 1/2 * width, 1.5 * stripe-height, 
  place-image(white, 1/2 * width, 3.5 * stripe-height, 
    place-image(white, 1/2 * width, 5.5 * stripe-height, 
      place-image(white, 1/2 * width, 7.5 * stripe-height, blue))))

five-stripe = 5 * stripe-height

blue-square = square(five-stripe,"solid","blue")

horizontal-cross = rectangle(five-stripe,stripe-height,"solid","white")

vertical-cross = rectangle(20,100,"solid","white")

cross = overlay(horizontal-cross, vertical-cross)

blue-cross = overlay(cross, blue-square)

piece = overlay(cross,blue-cross)

flag = overlay(piece,base)

place-image(piece,50,55,base)
```
