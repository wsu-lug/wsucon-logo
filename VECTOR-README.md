# Recreating WSUCon logos in Inkscape

I think that we can all agree that in most cases, vector graphics are better than raster graphics. They are instantly scalable and modular. For this guide, you'll need the free vector graphics program [Inkscape](www.inkscape.org).

Open an svg file in this repo. Before you get started, do yourself a favor and select View -> Display Mode -> Outline. Also, turn on snapping. There are a variety of snapping modes you can enable at the very right edge of the window. 

### Roman numerals
I used Comfortaa for the font. The size doesn't matter, since the perspective extension will auto scale it. 

When you have your roman numerals, select the text and select Path -> Object to Path. If you're in outline mode, the text will just be outlined, not filled in now.

I've already prepared the rectangles that the text will be put inside, but in case you need to recreate them, use the letters as a guide. Use the straight line tool to create a rectangle. Once you have the rectangle, you aren't done. Outline the rectangle with more straight lines *starting from the bottom* and going around *clockwise*. Once you've done that, delete the original rectangle. The new straight lines should be connected.

Your roman numerals should be joined, but if each letter has it's own bounding box, select them all by shift-clicking each one and then select Path -> Combine. 

Now the fun part. It's fun because it just works. *First*, select the roman numerals. *Then*, shift-click the large box where they will go. It is important that you select the numerals first, then the box. Now, select Extensions -> Modify Path -> Perspective. You should be presented with a window that says "Perspective is working". For me, it appeared for about 6 seconds -- enough to cause some minor panic. But don't worry. The window will close and your roman numerals will be beautifully perspectivized. 

### Year

The steps are the same for the year, but use the small box above the C instead. We used "Carlito" for the year.

## Colors
Now that you have everything layed out, you might want to edit the colors. If you switch your Display Mode to Normal, you should see the roman numerals and year filled in. 

You should see a rainbow of colors at the bottom of the screen. To change the color of an object (or multiple objects), select the object(s). Then right click on the color you want and select "Set Stroke". 

If you want to use the exact color as another element in the graphic, you can use the color picker, which looks like an eye dropper. With the color picker tool selected, click the object who's color you want. The color is then selected. This method is recommended so we maintain the same color red across different years of WSUCon. 

For the dark logo, you'll need to do something kind of tricky to cut out the roman numerals from the rectangle. Make sure all the roman numerals are set to a transparent fill. You have to select each letter inidividually by Ctl-clicking on the letter. Then shift-click to select the outer rectangle. Then select Path -> Difference. Do this with each letter. 