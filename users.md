---
title: Users
---

## Logging In

We block logging in using Username, so users must always login using their Email. This is a security measure as user names are easy to guess if the name is displayed as an author on a post.

## New Users

Having a strong password should be good enough to protect against most hacking attempts, but to be extra careful you should also use an email address that isn't easy to obtain (which the `@southlacrosse.org.uk` addresses on the Contacts page are). See the existing users for examples.

You should also note that GMail ignores everything after a `+` sign in the email address, so you can also add a suffix to the address to make it even more secure, which is especially relevant for administrators. For example `actual.address+extra@gmail.com` will get delivered to `actual.address@gmail.com`.

## Roles

Apart from the standard WordPress roles, we have a `SEMLA Officer` role. This is the same as `Editor`, plus the user has access to the SEMLA Admin Menu, so they can do things like load the fixtures. Administrators have access to everything, including the SEMLA Admin Menu.

## Deleting Users

Deleting most users isn't a problem, but if you delete an author who has posts then WordPress will ask you to assign their posts to another user. In order to preserve the correct credit on the author's posts you should therefore **not delete authors**, but instead edit the user and set their Role to `— No role for this site —`. Users without a role won't be able to login, and can safely remain on the system.
