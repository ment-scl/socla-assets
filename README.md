# SoCLA Conference Website Assets

Master stylesheets for the Society of Construction Law Australia (SoCLA) National Conference websites, built on EventsAir.

Website: https://www.soclaconference.com.au/

## Files

| File | Conference | Status |
| --- | --- | --- |
| `NC27-socla-EventsAir-global.css` | 2027 National Conference, Perth, 9 to 11 June 2027 | Current |
| `NC26-socla-EventsAir-global.css` | 2026 National Conference, Sydney, 6 to 8 May 2026 | Archived. Do not edit or delete. |

Each year gets its own file. Start a new year by copying the previous file and renaming it, so past conference pages keep working exactly as they were.

## How to use it in EventsAir

Add one link to the "Pre </HEAD> Code" section of the site. Use the jsDelivr address, not raw.githubusercontent.com. GitHub's raw address serves files as plain text, so browsers will not apply it as a stylesheet.

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/ment-scl/socla-assets@nc27-v1.0/NC27-socla-EventsAir-global.css">
```

`@nc27-v1.0` is a release tag. Pinning to a tag means changes only go live when a new tag is published and the link is updated. Using `@main` instead is fine for testing, but jsDelivr can cache it for up to 12 hours.

Load the stylesheet once only.

## What is in the stylesheet

• CSS variables (colours, fonts, sizes, spacing, radii, shadows, transitions)
• Typography, navigation and hamburger menu
• Buttons, portal buttons and overlays
• Cards (tickets, rooms, sponsors), modals and FAQ accordions
• Countdown and registration containers
• Mobile breakpoints and fixes for EventsAir builder classes

### 2027 brand colours (variables)

| Variable | Value |
| --- | --- |
| `--nc27-navy` | `#173b5d` |
| `--nc27-orange` | `#f7652d` |
| `--nc27-cream` | `#e2dfd6` |
| `--nc27-gold` | `#c9a84c` |
| `--nc27-pale-blue` | `#cce0ff` |

`--primary-blue` and `--accent-orange` are mapped to the navy and orange above.

## Updating the stylesheet

1. Edit the file in this repository.
2. Test the change on a draft EventsAir page first.
3. Commit the change.
4. Publish a new release tag (for example `nc27-v1.1`).
5. Update the tag in the link in the EventsAir "Pre </HEAD> Code" section.

## Version history

• NC27 v1.0: started from the NC26 file. Header updated for 2027. 2027 brand colour variables added.
• NC26 v1.0 (February 2026): initial release for the 2026 website.

## Notes

• Page-level styles for the 2027 hero, intro and banner currently sit in the EventsAir page code. They can be moved into the stylesheet once the remaining pages are built.
• This stylesheet and its assets belong to the Society of Construction Law Australia and are for use on official SoCLA conference websites only.
