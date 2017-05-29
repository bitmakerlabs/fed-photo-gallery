# Gallery

## HTML/CSS:

1. Lineup all of the `.photo` elements in the `/img` folder so they are displayed as part of a .gallery
2. Write `@media` queries to ensure the images lineup 1, 2, 3, 4 in a row, depending on the viewport width
3. Create a `.popover` (or "modal") that covers the entire screen with a single un-src'd image in it
4. Center the imagine within the `.popover` as best you can
5. Add a `.close` button (or just an X) in the top right corner of the `.popover`

## jQuery/Javascript:

1. Using jQuery, detect when an image is clicked. Store the `src` url of the image that was clicked (only the one image!)
2. Using HTML and CSS, prototype an overlay with a single larger image in it
Set the url of the clicked image to the src of the large image
3. Make any clicked .photo the .current element
4. When someone clicks the `.mainimg`:
  1. Figure out which element is `next()` from the `$('.current')`
  2. Move the `.current` class over to the `.next()` `.photo`
  3. Set the src `.attr()` for the `.mainimg` to match the `.next()` `.photo`
5. If someone does a `click()` on the `.close`, remove the `.popover`
    1. Make sure to remove the `.current` marker so that we don't accumulate false markers
6. If the `.current` `.is()` the `:last-child` of the `.gallery`, make sure the `.current` is moved to the `:first-child`
7. Using jQuery, figure out how to calculate the position of the `img` to center dynamically sized images in all directions
