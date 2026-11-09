# Manoa Rest Stop

## A UH Manoa bathroom locator and community review platform

* [Overview](#overview)
* [The problem](#the-problem)
* [The solution](#the-solution)
* [Current prototype](#current-prototype)
* [User guide](#user-guide)
* [Trust and privacy](#trust-and-privacy)
* [Development history](#development-history)
* [Future enhancements](#future-enhancements)
* [Deployment](#deployment)
* [Team](#team)

## Overview

Manoa Rest Stop helps UH Manoa students find a restroom that fits their needs before they make the trip across campus. The site combines a searchable bathroom directory, an interactive map, community ratings, and short-lived cleanliness reports in one place.

The project is designed around a simple question: **Which campus restroom should I use right now?** A student can compare locations, inspect details such as accessibility and supplies, read recent reports, and contribute an update after visiting.

* [Application source repository](https://github.com/manoa-bathroom-finder/manoa-bathroom-finder)
* [Manoa Bathroom Finder GitHub organization](https://github.com/manoa-bathroom-finder)

## The problem

Students often enter a UH Manoa bathroom without knowing whether it is clean, crowded, missing supplies, or unpleasant to use. Information is scattered, conditions change during the day, and there is no central community resource for comparing campus restrooms.

This creates several related problems:

* Students cannot easily find nearby restrooms that match their needs.
* Long-term quality and short-term conditions are mixed together.
* Important details such as accessibility, stall count, renovation history, and supplies are difficult to compare.
* Facilities staff and student users lack a focused channel for reporting problems or correcting location data.

## The solution

Manoa Rest Stop provides a campus-wide directory where each restroom can have:

* A location, building, floor, restroom type, stall count, accessibility information, and renovation history.
* An overall community rating with separate cleanliness and odor scores.
* Recent flash reports for conditions that may change quickly, such as missing paper, high odor, or long lines.
* Student comments, tags, helpfulness votes, and a way to flag a report.
* Favorites so students can quickly return to restrooms they trust.

The application separates overall ratings from real-time reports. A restroom can have a strong long-term rating while still having a temporary supply problem, and users should be able to see both facts.

## Current prototype

The project currently includes two front-end mockups:

* `loolocator_campus.html` demonstrates the main directory, search and filter controls, restroom cards, an interactive Leaflet map, bathroom details, favorites, a student/admin role switcher, and an admin request queue.
* `campus_bathroom_rating_reviews.html` demonstrates detailed reviews, quick flash reports, live review previews, rating controls, supply checks, tags, community-feed filters, helpfulness votes, and report flagging.

The prototype uses HTML, CSS, and JavaScript with Tailwind CSS, Font Awesome, Google Fonts, and Leaflet loaded from CDNs. It is intentionally focused on validating the user experience. Data is currently stored in the browser mockup, so authentication, a shared database, and permanent moderation are planned production work rather than completed features.

## User guide

### Find a restroom

The directory is the primary landing experience. Students can:

* Search by building, floor, or room number.
* Filter by rating, restroom type, accessibility, renovation status, or odor alerts.
* Compare summary cards showing ratings, supplies, favorites, and recent status.
* Open a restroom on the map or inspect its full details.

### Inspect restroom details

The detail view presents the information needed to make a quick decision, including renovation date, stall count, restroom type, accessibility, favorites, average ratings, and the latest community reports.

### Post a detailed review

After using a restroom, a student can submit:

* An overall star rating.
* Separate cleanliness and odor scores.
* Supply checks for toilet paper, soap, and hand dryers.
* Descriptive tags such as `#Clean`, `#FreshlyRenovated`, `#Quiet`, `#NoSoap`, `#OutOfOrder`, or `#Crowded`.
* A written comment with a live preview before posting.

### Send a quick flash report

When a condition needs immediate attention, a student can post a short status update using presets such as freshly sanitized, out of paper or soap, high odor, or long line. A note can add specific context, such as which stall is affected.

### Review the community feed

Students can sort reports by recency, helpfulness, or cleanliness and filter for five-star reviews, high odor, or missing supplies. Helpful and unhelpful votes surface useful reports, while flagging supports moderation.

### Manage the directory

Admins will be able to review bathroom additions, data corrections, reviews, and reports. The planned admin workflow separates pending, approved, and rejected requests so that directory information stays accountable and current.

## Trust and privacy

The design attributes reports to verified student email accounts to discourage spam and improve accountability. Production implementation should display only the minimum identity information needed by the community and should never expose a user's exact location.

Because bathroom conditions change, each report should show when it was created and the application should clearly distinguish current reports from historical averages. Moderation tools and community guidelines will help keep comments useful and respectful.

## Development history

The idea began with a project proposal focused on making restroom quality visible to the UH Manoa community. Early planning identified the core roles and use cases:

* Students browse, search, favorite, review, and report bathrooms.
* Admins approve or reject bathroom requests, data changes, reviews, and reports.
* Users can compare bathrooms by location, cleanliness, odor, supplies, and recent activity.

The current iteration turned those use cases into interactive HTML mockups. The next implementation milestone is to connect the directory and review flows to shared application data rather than browser-only sample data.

## Future enhancements

* Build the production application with a persistent database, authentication, and role-based authorization.
* Add directions, building hours, accessibility details, and campus map integration.
* Rank locations with a transparent tier list based on community ratings and recent reports.
* Notify users when a favorite restroom receives a new report or its rating changes.
* Add charts showing cleanliness and odor trends over time.
* Add moderation history, community guidelines, and facilities-maintenance escalation.
* Support organizations or campus groups that want to help maintain accurate location data.

## Deployment

This Bowfolio is published through GitHub Pages at [manoa-bathroom-finder.github.io](https://manoa-bathroom-finder.github.io/). The application mockups and source documentation are maintained in the [Manoa Rest Stop source repository](https://github.com/manoa-bathroom-finder/manoa-bathroom-finder).

## Team

* [Haoshen Zheng](https://haoshenz.github.io/)
* Kainalu Ishikawa
* Mina Girgis
* Junhong Xiong
