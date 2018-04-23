---
layout: eventdate
title:  "Exploded View at Britney Schauspiel Köln"
description: Confirmed: Exploded View Show at Schauspiel Köln
date:   2018-04-02 13:00:23 +0200
categories: eventdate news
event:
  title: Exploded View feat. Anika + Support Warm Graves
  description: Exploded View is playing in Cologne at Schauspiel Köln, supported by Warm Graves
  date: 2018-05-22
  url: "https://www.schauspiel.koeln/spielplan/monatsuebersicht/exploded-view/2700/"
  imageurl:
  venue:
    name: "Britney @Schauspiel Köln (Außenspielstätte Offenbachplatz)"
    url:  "https://www.schauspiel.koeln/haus/britney/"
    streetAddress: "Offenbachplatz"
    zipcode: "50667"
    city: "Köln"
    country: "Germany"
  ticketsurl: "https://www.schauspiel.koeln/spielplan/monatsuebersicht/exploded-view/2700/karten-kaufen/2700/"
---

<script type='application/ld+json'>
{
  "@context": "http://www.schema.org",
  "@type": "MusicEvent",
  "name": "{{ page.event.title }}",
  "url": "{{page.event.url}}",
  "description": "{{page.event.description}}",
  "startDate": "{{ page.event.date | date: "%m/%d/%Y"  }}",
  "endDate": "{{ page.event.date | date: "%m/%d/%Y"  }}",
  "location": {
    "@type": "Place",
    "name": "{{ page.event.venue.name }}",
    "sameAs": "{{ page.event.venue.url }}",
    "address": {
      "@type": "PostalAddress",
      "streetAddress": "{{ page.event.venue.streetAddress }}",
      "addressLocality": "{{ page.event.venue.city }}",
      "postalCode": "{{ page.event.venue.zipcode }}",
      "addressCountry": "{{ page.event.venue.country }}"
    }
  },
  "offers": {
    "@type": "Offer",
    "url": "{{ page.event.ticketsurl }}"
  },
  "performer": {
    "@type": "PerformingGroup",
    "name": "Exploded View"
  }
}
</script>
