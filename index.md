# Manoa Rest Stop

## A UH Manoa bathroom locator and community review site

* [Overview](#overview)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)
* [Example Enhancements](#example-enhancements)
* [Deployment](#deployment)
* [Team](#team)

## Overview

Manoa Rest Stop is a website that helps UH Manoa students find and compare campus bathrooms. Students can search for a bathroom, view its location and details, read reviews, and submit updates about its current condition.

The project addresses a simple problem: students often do not know whether a bathroom is clean, crowded, missing supplies, or accessible before they use it.

The planned system includes:

* A bathroom directory with locations, restroom types, stall counts, renovation dates, and accessibility information.
* Community ratings for cleanliness, odor, and overall experience.
* Recent reports for conditions such as missing soap, missing toilet paper, high odor, or long lines.
* Search, filters, an interactive map, favorites, and an administrator review queue.

The project source is available in the [Manoa Bathroom Finder repository](https://github.com/manoa-bathroom-finder/manoa-bathroom-finder).

## User Guide

### Bathroom Directory

The directory lets students search by building, floor, or room number. Filters can be used to find highly rated, accessible, renovated, or recently reported bathrooms.

### Interactive Map

The map displays restroom locations across campus. Selecting a location shows its details and allows the student to inspect or report its condition.

### Bathroom Details

The details view shows the restroom type, stall count, renovation date, accessibility information, favorites, ratings, and recent community reports.

### Reviews

Students can submit an overall star rating, cleanliness score, odor score, supply checks, tags, and a written comment. The review prototype also includes a preview of the post before it is submitted.

### Quick Reports

Students can quickly report that a restroom was freshly sanitized, out of paper or soap, high odor, or crowded. They can also add a short note.

### Administration

Administrators will be able to review bathroom requests, data corrections, reviews, and condition reports before approving or rejecting them.

## Community Feedback

The project is intended to make it easier for students to find useful and current information about campus bathrooms. Feedback will help us decide which details are most useful, how reports should be moderated, and which filters students use most often.

## Developer Guide

The current version is a front-end prototype made with HTML, CSS, and JavaScript. It uses Tailwind CSS, Font Awesome, Google Fonts, and Leaflet through CDNs.

The main prototype files are:

* `loolocator_campus.html` — bathroom directory, map, bathroom details, favorites, and admin queue.
* `campus_bathroom_rating_reviews.html` — ratings, reviews, quick reports, and the community feed.

The current mockup uses sample data in the browser. A production version will need a shared database, authentication, authorization, and permanent moderation.

## Development History

The project began as a proposal for a UH Manoa bathroom locator and tier list. The first prototypes focused on the main directory and map. Later work added detailed reviews, live condition reports, supply checks, community-feed filters, and administrator workflows.

The next major step is connecting the prototype to persistent application data so that students can see the same reviews and reports across devices.

## Example Enhancements

* Add directions and building hours.
* Add notifications for favorited bathrooms.
* Add charts showing cleanliness and odor over time.
* Add a transparent bathroom tier list.
* Add moderation history and community guidelines.
* Allow facilities staff to respond to reports.

## Deployment

The Bowfolio is deployed at [manoa-bathroom-finder.github.io](https://manoa-bathroom-finder.github.io/).

## Team

* [Haoshen Zheng](https://haoshenz.github.io/)
* Kainalu Ishikawa
* Mina Girgis
* Junhong Xiong
