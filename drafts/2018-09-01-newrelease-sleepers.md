---
layout: eventdate
title:  New Video From Exploded View! 'Sleepers'
description: New track 'Sleepers', latest to be released from forthcoming record, 'Obey' out on Sacred Bones on 28th Sept 2018.  
date:   2018-09-13 13:00:23 +0200
categories: newrelease news
event:
  title: New Video From Exploded View! 'Sleepers'
  description: New Exploded View track 'Sleepers', latest to be released from forthcoming record, 'Obey' out on Sacred Bones on 28th Sept 2018.
  date: 2018-09-01
  url: "https://www.youtube.com/watch?v=C6SXE9R67Wg"
  imageurl: https://i.ytimg.com/vi/C6SXE9R67Wg/maxresdefault.jpg
  Listen on Spotify:
  spotifyurl: "https://open.spotify.com/track/3jP5t43ucbpaQGh2sETaqc"
---
  <!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/C6SXE9R67Wg" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> -->

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
