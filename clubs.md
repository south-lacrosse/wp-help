---
title: Clubs
---

Clubs are added using their own post type, and can be found on the main WordPress Admin Dashboard menu. They are edited in the same way as regular pages and posts, though there are specific blocks that you should use.

The simplest option to create a new club page is to add the Club Layout pattern (see [Block Patterns](patterns.md)). Note that you can modify this pattern for future use, or create additional patterns. Alternatively edit another club and copy the content from there.

You can easily delete any unwanted blocks by using the Document Overview.

![Document Overview](/assets/img/overview.png)

If the Club has a logo then it should start with a **Club Title** block. This will replace the normal page title (the club name) on the front end as long as it contains a **Post Title** inner block, which it does by default (unfortunately we can't hide the standard title in the editor, so you will see the club name twice).

If you have entered the club name then a Club Title block with the club name above it will look like:

![Empty Club Title](assets/img/club-title-empty.png)

You need to set the Club's featured image to the logo. In the settings on the right select the Club tab rather than Block, and locate the **Featured Image** section. If you don't see the settings area, you may need to click on the settings icon in the top right corner to make it appear. Once you have uploaded or selected a featured image it will appear in the Club Title.

Inside the Club Title block you can also have a **Website** block, which is used to determine the club's website in other pages such as the Clubs List, and also a standard **Social Links** block for links to Facebook, Instagram etc.. Please make sure you use correct [link URLs](editing.md#link-url).

Once completed it should look something like:

![Completed Club Title](assets/img/club-title-filled.jpg)

The club's location should be added using a [Location Block](location.md), as that will correctly format the Google Map, and make sure the club is placed correctly on the Clubs Map etc.

You should also use the [Attribute Value Block](attribute-value.md) to correctly format things like contacts, club colours etc., and take a look at the help page as it details a quickest way to enter attribute/values as paragraphs, and then transforming them.

If you know the Club's founded date then you should add it to the page under Club Information, unless the logo contains the founded date in which case it can be omitted, though you should make sure it's added to the [SEMLA Club Founded Dates Google Sheet](https://docs.google.com/spreadsheets/d/1_FFVi4FSQ5mW2Ory7X4gIRy-0JHlQEC3Zx6KJfQyusw/edit?usp=sharing)

Finally, at the bottom you should always add the **Club Footer** [synced pattern](patterns.md#synced-patterns).

You should check out the other Clubs to see what is possible.

## Clubs List

Information from the Club page is also used for the Clubs List [SEMLA Data block](semla-data.md), so you need to make sure you create the Club in the correct format.

Most, if not all, clubs should use the **Club Title** block. Its inner **Website** block is then used to populate the website link on the Clubs List. If there is no Website block then the Clubs List will use the first link on the page with the link text of "Website" or "Club Website" (case doesn't matter).

The other links are populated from the first **Social Icons** block on the page, usually the one in the Club Title block.
