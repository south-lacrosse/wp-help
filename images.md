---
title: Images
---

Before you upload any images you should make sure you optimize them, as smaller images mean faster load times, and there are many tools that will allow you to reduce file size while maintaining quality.

You should also make sure you use sensible dimensions. The current theme (as of 2023) uses a layout with a default content width of **720px**, and a wide size of **1024px** (which you can use on certain blocks like Image, Table, or Media & Text). There is no point having images larger than the width they will be displayed at, so if your image will only be displayed in the standard content area it should be a **maximum** of **720px**, and **1024px** for wide alignment. If you are using the image as a logo, or in the Media & Text block, then you should resize it so it only takes up the space it needs.

**Club logos** should be square, and you should aim for **300x300px** as there shouldn't be a need to display anything larger, and a minimum of 150x150px as this size will be used in the Club Title.

The theme also allows full width so you can have larger images, though this should be used sparingly.

The simplest tool to use is Google's [Squoosh](https://squoosh.app/), which allows you to compress and resize your image. Just drop your image on the page, and follow the instructions. Even though it is a web app it does all the work locally.

Currently Squoosh has no cropping functionality, but you can use tools such as [Gimp](https://www.gimp.org/), Photoshop, or the online [Adobe Express](https://www.adobe.com/express/feature/image/crop), or you can crop the image in WordPress after you upload it.

See also [more compression tools](https://github.com/south-lacrosse/www-dev/blob/main/docs/developer-info.md#compression).

You should also note that WordPress creates several sizes for each image, with the original size, and then sizes fitting inside 1024x1024px (though as stated above you shouldn't have bigger than this), 300x300px, 150x150px, and 50x50px for club logos, omitting anything bigger than the original. If the browser can only display a smaller size, for example on mobile, then it will download the smaller image, therefore saving bandwidth and making the site faster.

## Aspect Ratio

You should try to use consistent aspect ratios, at least on the same page. You can use the tools suggested above for cropping. For most pictures you should use 16x9, or 9x16 for portrait, and Club logos should be square.

## Filenames

You might get images with weird names like `cid_A0E6CC18-EB02-43F2-B0DC-D33453D366A0.jpeg`, which won't be very useful if you need to search for the image in the Media Library, and are also bad for SEO. So before you upload files you should name them something sensible. You should use hyphens instead of spaces, have letters all lower case, no special characters, make the name descriptive, and use `.jpg` instead of `.jpeg`. So the example above, which is actually a club logo, would be much better as `bournemouth.jpg`.

## Lightbox Galleries

A lightbox is a modal image gallery, where you usually have a set of thumbnails and selecting one will pop up a larger image. You can then navigate through these larger images, or exit and select another thumbnail.

Our SEMLA plugin allows you to create these using the standard WordPress gallery block. What you need to do is:

1. Create a gallery block, and add your images.
1. If the block added captions then you probably want to delete them.
1. Open the block settings (if it's not showing then you can open it with the icon in the top right next to the 3 dots).
1. Uncheck `Crop images`.
1. Set `LINK` TO to Media File.
1. Set `IMAGE SIZE` to Thumbnail.
1. Open the styles tab and set the style to `Lightbox`. Once you do this the block will display as many thumbnail images as will fit on each line, and ignore the COLUMNS setting.
1. You can give each image a title by selecting an image, and in the Block Settings open up the Advanced panel, and enter the `TITLE`. This will appear over the thumbnail when you hover over it, and also below the image in the lightbox.

If you go to your page you can click on any of your thumbnails to open the lightbox.
