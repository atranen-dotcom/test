# H. Williams Mobile Pet Spa: Website Content Drafts

Drafts of new pages for hwilliamsmobilepet.com, written to help with regular Google search (SEO) and with AI search in ChatGPT, Claude, Perplexity and Google AI Overviews (GEO).

## What's in here

| File | Page | Suggested URL |
|---|---|---|
| `faq.md` | Mobile Grooming FAQ | `/mobile-dog-grooming-faq/` |
| `greenwich-ct.md` | Greenwich town page | `/mobile-dog-grooming-greenwich-ct/` |
| `darien-ct.md` | Darien town page | `/mobile-dog-grooming-darien-ct/` |
| `new-canaan-ct.md` | New Canaan town page | `/mobile-dog-grooming-new-canaan-ct/` |
| `scarsdale-ny.md` | Scarsdale town page | `/mobile-dog-grooming-scarsdale-ny/` |
| `schema-local-business.md` | Code for the home page that tells Google and AI tools who you are | (paste into the home page) |

The URL pattern matches your existing Rye page (`/mobile-dog-grooming-in-rye-ny/`). You can use either style, as long as you stick with one.

## Before anything goes live: fill in the [BRACKETS]

I only used facts that are already public about the business: your phone number, the 60–90 minute grooms, all-natural products, one-on-one care in a self-contained van, licensed and insured, and dogs and cats. Anything I couldn't confirm is in **[BRACKETS]**, such as prices, hours, what's in each package, and when you started. Please don't publish a bracket. Google won't mind, but your customers will giggle.

**About Scarsdale:** your site doesn't list Scarsdale as a service area yet. Publish that page only if a van actually goes there (or will soon, with van #6). If not, use the same template for Harrison or Larchmont instead.

## How to post each page in WordPress

1. **Pages → Add New.** Paste the "Page Content" section.
2. Set the **URL slug** to the one listed at the top of each file.
3. In your SEO plugin (Yoast or Rank Math: look for the box under the editor), paste the **SEO Title** and **Meta Description**.
4. Add 2–4 **real photos**: the van parked in that town, a before/after, a happy dog. Name the files something like `mobile-dog-grooming-darien-ct.jpg` and fill in the image "alt text" with a plain description.
5. On the town pages, paste the FAQ schema code block into a "Custom HTML" block at the bottom of the page. On the FAQ page, do the same with its code block.
6. **Link the pages together.** Add links to the town pages from the home page (a "Towns We Serve" section) and from the footer. Link the FAQ from the main menu.
7. After publishing, open **Google Search Console → URL Inspection**, paste each new URL, and click **Request Indexing**.

## Quick cleanup items (from the search check)

- **"Coming Soon" page** (`/coming-soon/`): delete it or set it to "noindex" in your SEO plugin. It's currently showing up in Google.
- **"Uncategorized" blog category**: give the blog posts real categories (e.g. "Grooming Tips", "Senior & Anxious Dogs") and set category archives to noindex, or at least rename "Uncategorized."
- **Google Business Profile**: make sure the service-area towns there match the towns on the website exactly.
