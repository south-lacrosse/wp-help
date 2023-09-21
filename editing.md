---
title: General Editing Help
---

## Content Width

By default the content width is limited to 720px. This is because text is difficult to read if the lines are too wide. There is also a wide alignment of 1024px, and you can use this for blocks which support this (Image, Table, Media & Text, Column, .etc), however keep in mind the readability of the page.

![Align Toolbar](assets/img/align-toolbar.png)

Some blocks also support full width, but this should be used extremely sparingly.

## Links

### Link URL

When adding links you should make sure you remove any extraneous parts of the URL, which usually means part, if not all, of the query string (the bit after the `?`). For example the following query strings can be safely removed:

* `https://www.facebook.com/cardifflacrosse/?locale=en_GB` - locales are rarely needed.
* `https://southernboxlacrosse.org/f/b-oxfest-2023?fbclid=IwAR2XDqH4H-kILDLXca8k5eTlWYx4u05Wdff5ujX-TxS4iUlUprkdgw9CaGM` - Facebook and other sites often add query strings to links from their site so that the target site knows where the link came from. These should always be removed.

Note that some URLs need the information in the query string, e.g. our own fixtures page uses it for the club or team name, e.g. `https://www.southlacrosse.org.uk/fixtures?team=Bath`, so do be careful.

You should also remove the trailing slash if possible. Facebook and Twitter should have no trailing slash, and Instagram should have one. You shouldn't remove a trailing slash from the site root, so `https://www.example.com/` should be left as is, but you may be able to remove it from `https://www.example.com/folder/`. Try the link without a trailing slash in your browser, and if it needs the trailing slash it will either not work, or the page will be redirected so that address includes the slash.

Before adding the link you should test it in your browser to make sure that it still goes to the correct page, and also make sure the link isn't redirecting by using the DevTools in your browser or an online redirect checker.

### Telephone Number Links

To link to telephone numbers just add `tel:` to the beginning of the URL, and make sure there are no spaces in the number, so `tel:07123456789`, and not `tel: 07123 456789`. You can use the international number format and hyphens for separators, so `tel:+44-7123-456789` is valid. On mobile devices a `tel:` link will dial the number when a user clicks it, and desktop browsers may offer to make a call from their phone.

You should also nicely format the link text so it is easier to read. For most numbers that means grouping 5-6, 020 numbers 3-4-4, and if the number has an international dialing code then that should be a separate group and the first group size reduced by 1.

| Number | Formatted |
| ------ | --------- |
| `07123456789` | `07123 456789` |
| `+447123456789` | `+44 7123 456789` |
| `02012345679` | `020 1234 5679` |

## Post Author

You should be aware that posts (not pages or clubs) will display the author name and modified date on the front end, so if you create a post from an account for your role such as "SEMLA Webmaster" it will display that name. If you want the post to display your actual name then you should create the post from a personal account (or see below to create a post as a different user). Note in the above example this doesn't mean setting the "SEMLA Webmaster" name to your name, as when someone else takes over that role the name will be changed, and all the posts that user has authored will have the author name changed too! If you need a personal account then you should ask the Webmaster or another administrator to create one for you.

### Creating Posts As A Different User

If you user account has the Editor or SEMLA Officer roles (and they most likely do) you can assign posts to a different author, either while editing it from the Post Settings, or you can change existing posts from the Posts list screen using Quick Edit or Bulk actions.

## Custom Block Styling

To style a block you can usually use the styling options in the block Settings. You can also add custom styles provided by the theme to any block using the Additional CSS Classes feature (CSS is Cascading Style Sheets, the language used to style web pages).

To add an additional CSS class to a block, click on the block you are editing. Then, check the block settings on the right for the Advanced setting.

If you don't see the block settings on the right, click the settings icon in the top right corner to open the settings. This icon looks like a square with two uneven columns.

Classes provided by our theme are:

* `no-print` - omit from printed page. If a user prints a page our default styles will remove the header, footer, sidebars, and navigation. Use this class if you don't want the current block to be printed.
* `callout callout-info` etc. - see [the Callout page](callout.md) for how to style callouts.
