# Miss Anna S Way Station - website

The public website for Miss Anna S Way Station, a 501(c)(3) animal rescue in Little Rock, Arkansas.
EIN 41-3565519. Built as a plain static site and published with GitHub Pages.

## What is in here

    index.html      home page - intro, photo carousel, three ways to help
    about.html      who the organization is, what it does, how it is funded
    donate.html     the four ways to give, in order of usefulness
    contact.html    phone, email, follow links
    updates.html    the list of updates, newest first
    updates/        one file per update, plus _template.html to copy
    assets/style.css   the whole look - colours live at the top of this file
    assets/photos/     every photo used on the site

## The rule that matters most

**Donation links point OUT to the organization's own accounts.**
This site never collects money, never sees card details, and has no forms.
If you are editing a donation link, you are changing where a donor is sent - so
copy-paste, never retype, and test the link afterwards.

    PayPal     https://www.paypal.com/donate/?hosted_button_id=DY4ASRAAML26Q
    Chewy      https://www.chewy.com/g/miss-annas-way-station_b153605479
    Amazon     https://www.amazon.com/hz/wishlist/ls/1XON7PG287Z33?ref_=wl_share
    Cash App   https://cash.app/$Wayetsi

    Vet bill   Pallone Veterinary Hospital, Rose Bud AR, (501) 556-5355
               Callers ask to put a payment on Miss Anna's Way Station's account.
               No link to maintain - it is a phone number.

PayPal is the button in the header of every page. It is the one that takes cards
without an account, which is why it is the primary route.

## How to change a donation link

1. Open the file you need (`donate.html` for the list, or every page's header for
   the big button - the header is repeated in each of the five pages).
2. Find the existing link, swap the URL, save.
3. Check the old and new links both work before pushing.

## How to add an update

1. Copy `updates/_template.html`.
2. Rename it `YYYY-MM-DD-short-title.html` - hyphens, no spaces.
3. Edit the title, the date and the text.
4. In `updates.html`, copy an existing `<div class="post">` block and put the new
   one at the top, pointing at your new file.
5. Save, commit, push. Pages republishes in about a minute.

## Photos

Drop the file into `assets/photos/`, then reference it as
`assets/photos/name.jpg` (or `../assets/photos/name.jpg` from inside `updates/`).
Always write useful alt text - it is what a screen reader reads out, and what
Google reads too. Straight-from-camera files are best; anything downloaded from
Facebook is compressed and will look soft on a big screen.

## Who owns this

The repository, the domain and the donation accounts belong to Miss Anna S Way Station, not to
whoever builds or maintains the site. See MAINTAINERS.md for who has access and
what to do if the site breaks.

## Publishing

GitHub Pages, serving the `main` branch from the repository root. No build step,
no dependencies, no server - which also means no monthly hosting bill.
