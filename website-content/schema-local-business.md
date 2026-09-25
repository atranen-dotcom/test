# Business Info Code for the Home Page (LocalBusiness Schema)

This code tells Google, ChatGPT, Perplexity and the other AI tools, in their own language, exactly who you are, where you work and how to book. It's invisible to visitors.

**Where it goes:** at the bottom of your **home page**, in a "Custom HTML" block. Some SEO plugins, like Rank Math and Yoast Local, have a "Local SEO" settings screen that does this for you. If your current SEO person set one up, check there first so you don't end up with two copies.

**Before pasting:** it's ready to go as is. The logo and van photo lines are left out for now. See the note at the bottom for how to add them.

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "H. Williams Mobile Pet Spa",
  "description": "Mobile dog and cat grooming. Licensed and insured, one-on-one grooming in self-contained vans at your home, using all-natural products. Serving Greenwich, Stamford, Darien and New Canaan, CT, and Rye and Port Chester, NY.",
  "url": "https://hwilliamsmobilepet.com/",
  "telephone": "+1-203-900-7704",
  "email": "info@hwilliamsmobilepet.com",
  "priceRange": "$$",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "Greenwich",
    "addressRegion": "CT",
    "postalCode": "06830",
    "addressCountry": "US"
  },
  "areaServed": [
    { "@type": "City", "name": "Greenwich, CT" },
    { "@type": "Place", "name": "Old Greenwich, CT" },
    { "@type": "Place", "name": "Cos Cob, CT" },
    { "@type": "Place", "name": "Riverside, CT" },
    { "@type": "City", "name": "Stamford, CT" },
    { "@type": "City", "name": "Darien, CT" },
    { "@type": "City", "name": "New Canaan, CT" },
    { "@type": "City", "name": "Rye, NY" },
    { "@type": "City", "name": "Port Chester, NY" }
  ],
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
      "opens": "08:00",
      "closes": "17:00"
    }
  ],
  "potentialAction": {
    "@type": "ReserveAction",
    "target": "https://booking.moego.pet/go/?name=HWilliamsMobilePetSpa"
  },
  "sameAs": [
    "https://www.instagram.com/hwilliamsmobilepet/",
    "https://www.facebook.com/p/H-Williams-Mobile-Pet-Spa-100089757743195/",
    "https://www.yelp.com/biz/h-williams-mobile-pet-spa-greenwich",
    "https://nextdoor.com/pages/h-williams-mobile-pet-spa-greenwich-ct/",
    "https://share.google/GtbtB2AxtVTtfMsxE"
  ]
}
</script>
```

**Adding your logo and van photo (optional, 2 minutes)**
1. In WordPress, go to **Media → Library** and click your logo.
2. On the right, find **File URL** and click **Copy URL to clipboard**.
3. In the code above, add a new line right after the `"email"` line: `"logo": "PASTE-THE-LINK-HERE",`
4. Do the same with a van photo, using `"image": "PASTE-THE-LINK-HERE",`

**Notes**
- Add new towns to `areaServed` as you expand (Scarsdale when van #6 heads there, for example).
- The Google link is a share link. If Google's Rich Results Test complains about it, swap it for the full Google Maps link to your listing.
- To check your work, paste the code (or your live home page URL) into Google's free [Rich Results Test](https://search.google.com/test/rich-results). Green checkmarks = you're golden.
