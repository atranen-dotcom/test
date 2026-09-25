# Business Info Code for the Home Page (LocalBusiness Schema)

This code tells Google, ChatGPT, Perplexity and the other AI tools, in their own language, exactly who you are, where you work and how to book. It's invisible to visitors.

**Where it goes:** at the bottom of your **home page**, in a "Custom HTML" block. Some SEO plugins, like Rank Math and Yoast Local, have a "Local SEO" settings screen that does this for you. If your current SEO person set one up, check there first so you don't end up with two copies.

**Before pasting:** fill in the brackets, or delete any line you can't fill in (and the comma on the line above it if it becomes the last item). Everything else is already filled in from public info.

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "H. Williams Mobile Pet Spa",
  "description": "Mobile dog and cat grooming. Licensed and insured, one-on-one grooming in self-contained vans at your home, using all-natural products. Serving Greenwich, Stamford, Darien, New Canaan, CT and Rye, NY.",
  "url": "https://hwilliamsmobilepet.com/",
  "telephone": "+1-203-900-7704",
  "email": "[BUSINESS EMAIL]",
  "logo": "[URL OF YOUR LOGO IMAGE]",
  "image": "[URL OF A PHOTO OF YOUR VAN]",
  "priceRange": "$$$",
  "address": {
    "@type": "PostalAddress",
    "addressLocality": "Greenwich",
    "addressRegion": "CT",
    "postalCode": "[ZIP]",
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
    { "@type": "City", "name": "Rye, NY" }
  ],
  "openingHoursSpecification": [
    {
      "@type": "OpeningHoursSpecification",
      "dayOfWeek": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
      "opens": "[08:00]",
      "closes": "[17:00]"
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
    "[YOUR GOOGLE BUSINESS PROFILE LINK]"
  ]
}
</script>
```

**Notes**
- Add Scarsdale (and any other towns) to `areaServed` only once you actually serve them.
- `priceRange` is just a rough signal. Change it to `$$` if that fits better.
- To check your work, paste the code (or your live home page URL) into Google's free [Rich Results Test](https://search.google.com/test/rich-results). Green checkmarks = you're golden.
