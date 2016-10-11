# Bob Ross

![](http://i.imgur.com/9EI2q3P.jpg)

> We don't make mistakes, just happy little accidents. -[Bob Ross](https://en.wikipedia.org/wiki/Bob_Ross)

Bob Ross has a twitch.tv channel and it's incredible. You can check that out [here](https://www.twitch.tv/bobross). Bob Ross passed away in 1995 but his TV Show still inspires people today which is evident of the popularity that this Twitch Channel generated over the past year.

### Bob Ross Video

[![](http://img.youtube.com/vi/YLO7tCdBVrA/0.jpg)](https://www.youtube.com/watch?v=YLO7tCdBVrA "Bob Ross")

# Instructions

Lets treat Interface Builder like our empty canvas.  

![](http://i.imgur.com/87Kf685.png?1)

Let the painting begin.

Drag onto the canvas, a `UIImageView` and position it towards the bottom of the scene.The `UIImage` that we're going to place within this `UIImageView` is a .png file I was able to find on the internet. The size of this image is 1280 (w) x 800 (h). Ultimately, we want to stick to this aspect ratio in Interface Builder. We don't want our `UIImageView` object to have a `width` of 1280 and a `height` of 800. With all of the different iPhone/iPad screen sizes, this would look different on every single device if we supplied it with explicit constraints like this.

Add an Aspect Ratio constraint to this `UIImageView`. After selecting this constraint--open the Attributes Inspector to be able to view details on this specific constraint. The ratio should be 1280:800 or 8:5 (broken down by the greatest common devisor). By adding this constraint, we are insuring that this aspect ratio sticks, if the width of this `UIImageView` is ever set to 8, then in turn the height will be 5. If one grows, so does the other staying in line with that aspect ratio (which is awesome).

Now you should constrain this `UIImageView` to the `View`. The bottom, leading and trailing edges of the `UIImageView` should equal the `View`.

Through those three constraints, the `width` of this `UIImageView` and considering our `height` and `width` work with each other (because of setting the Aspect Ratio) we've technically set the `height` on this `UIImageView` already!

Select the `UIImageView`. In the attributes inspector, set its image to `Grass`. Run your app, it should look like the following screenshot:

![](http://i.imgur.com/EWzyZhf.png?1)

Add another `UIImageView` to your canvas. Place it near the upper right corner. This will be our Sun. Feel free to select the `UIImageView` and set its image to Sun.

The following constraints should be added to this new `UIImageView`: 
* The height and width should be the same. Hint: Aspect Ratio.
* The width should be 0.25 of the View's width.
* The top and trailing edges should equal the Views top and trailing edge.

Run your app, it should look like this:

![](http://i.imgur.com/9oad9uT.png?1)

Add another `UIImageView` to the canvas. This will represent out SmallTree image (so feel free to set the image of this new `UIImageView` to SmallTree.)

The following constraints should be added to this new `UIImageView`:
* `139:230` should be the aspect ratio of this `UIImageView`.
* The width should be 0.3 of the View's width.
* The Small Tree `UIImageView` bottom should equal the top of the Grass `UIImageView` with a multiplier of 1.25. 
* The leading edge should equal the Views leading edge.

It should now look like this when you run the app:

![](http://i.imgur.com/x0ojPSn.png?1)




<a href='https://learn.co/lessons/BobRossLab' data-visibility='hidden'>View this lesson on Learn.co</a>
