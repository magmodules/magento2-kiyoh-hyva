# Changelog

All notable changes to the Kiyoh Hyvä compatibility module will be documented in this file.

## [1.2.0]

**Features:**
* Builds with Hyvä 1.5 and later, whose Tailwind 4 reads `module.css` instead of `tailwind.config.js`; the config file stays for earlier Hyvä versions.

**Improvements:**
* The stars in the Full, Small and Plain review widgets and in the three sliders show the score. The width was calculated for a five-point scale, so every score above 5 showed five full stars.
* The overview widget counts the same reviews in "based on" as in the star distribution below it.
* The filter modal on the review page closes once the filters are applied.
* The floating widget gets a position when none is configured.

**Compatibility:**
* Magento 2.4.x
* Hyvä 1.x, including the Tailwind 4 builds of 1.5 and later
* Requires Kiyoh 1.12.0 or later.

## [1.1.0]

**Features:**
* Seven new widgets, matching the ones Kiyoh 1.7.0 added: overview, textual, badge, carousel, sidebar, floating and plain.

**Compatibility:**
* Requires Kiyoh 1.7.0 or later.

## [1.0.0]

**Features:**
* Tailwind templates for the Kiyoh review page and the Full and Small review widgets and the three sliders.
