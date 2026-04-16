CCDI Web Applications SEO, LLMO SOP


# Purpose

This SOP outlines the procedures and best practices for implementing SEO (Search Engine Optimization) improvements to enhance the visibility, ranking, and organic traffic of a website. The goal is to ensure consistent and effective optimization across all web pages.


# Roles & Responsibilities

- SEO Specialist: Oversees implementation and audits.
- Content Creators: Ensure all content follows SEO guidelines.
- Web Developers: Address technical SEO requirements.
- TPM and Fed Lead: Define target audience and review performance metrics.



# Procedure

## SEO Development Cycle (Repeatable)

Use this cycle for every monthly/quarterly SEO iteration:

0. **Benchmark first (required)**
   - Capture baseline metrics before any optimization work:
     - Organic traffic
     - Keyword rankings
     - Impressions and CTR
     - Conversions
     - Core Web Vitals / page speed
     - Indexed pages and crawl issues
1. **Research audience and search behavior**
2. **Implement metadata and content updates**
3. **Improve page speed and UX**
4. **Build external authority (backlinks)**
5. **Refresh and expand content**
6. **Monitor, report, and optimize again**

**Benchmark cadence:**
- Initial benchmark: before starting a new SEO cycle
- Checkpoints: 30/60/90 days after major updates
- Ongoing: compare monthly results against baseline

## Step 0: Benchmark Current Performance

**Frequency:** At cycle start and before major releases

**Why this step matters:**

Without a baseline, you cannot confirm whether SEO updates are working. Benchmarking gives your team a clear before-and-after view.

**What to do:**

- Capture current metrics:
  - Organic traffic
  - Keyword rankings for priority terms
  - Impressions and click-through rate (CTR)
  - Conversion rate from organic traffic
  - Indexed pages and crawl issues
  - Core Web Vitals and page speed
- Document baseline values in a shared tracker.
- Define 30/60/90-day targets for the cycle.

**Tools and how they help:**

- **[Google Search Console](https://search.google.com/search-console/about)** `Free` - Baseline for impressions, clicks, CTR, indexing, and crawl alerts
- **[Google Analytics](https://analytics.google.com/)** `Free` - Baseline for traffic quality and conversions
- **[PageSpeed Insights](https://pagespeed.web.dev/)** `Free` - Baseline for speed and Core Web Vitals

**Output:**

- Approved baseline snapshot for this cycle
- 30/60/90-day target metrics recorded

## Step 1: Identify Your Main Audience and Their Search Behavior

**Why this step matters:**

Before choosing keywords, first understand who you are trying to help and how they ask for help online. Good SEO starts with audience questions, not just keyword lists.

**What to do:**

- Define your top audience groups (for example: researchers, clinicians, patients, caregivers, policy staff).
- List what each audience group is trying to do (learn, compare, apply, find a resource, contact support).
- Write 5-10 real search-style questions each audience might type.
  - Example: "How do I find pediatric cancer data by year?"
  - Example: "What is CCDI and who can use it?"
- Convert those questions into keyword intent groups:
  - Primary keyword: main topic of the page
  - Secondary keywords: common variations and related phrases
  - Search intent: informational, navigational, or action-oriented

**Tools and how they help:**

- **[Google Search Console](https://search.google.com/search-console/about)** `Free`
  - Helps you see what users already search before landing on your site.
  - Use it to find real queries with high impressions but low click-through rate (CTR).
- **[Google Keyword Planner](https://ads.google.com/home/tools/keyword-planner/)** `Free`
  - Helps estimate search demand and discover related terms.
  - Use it to validate whether your audience phrases are commonly searched.
- **[SEMrush](https://www.semrush.com/)** `Paid (trial available)`
  - Helps compare your topics with other websites and uncover missed terms.
  - Use it for deeper research when planning major content updates.


**Output:**

For each page, create a short "Audience and Search Intent" note including:

- Primary audience
- Top user questions
- Primary keyword
- Secondary keywords
- Search intent
- Recommended page angle (what answer the page should provide first)


## Step 2: Prepare Page Metadata and Content

**Frequency:** For every new or updated page

**Why this step matters:**

Now that you have the keyword and audience-intent list from Step 1, prepare both the technical metadata layer and the page content together. Page headers (HTML `<head>`) contain metadata tags that don't appear on the page but help search engines, AI tools, and social media understand and display your content correctly. The visible page content must answer user questions clearly and be easy to read. Together, metadata + content ensure the page is search-ready, AI-ready, and social-media-ready.

**What to do:**

**A. Set up page header metadata tags:**

- **Open Graph (OG) tags** - for social media preview (Facebook, LinkedIn, etc.)
  - `og:title`, `og:description`, `og:image`, `og:url`, `og:type`
- **Twitter Card tags** - for Twitter/X sharing
  - `twitter:card`, `twitter:title`, `twitter:description`, `twitter:image`
- **Dublin Core Terms** - for trust, authority, and academic/government context
  - `dc:creator` (author), `dc:date`, `dc:publisher`, `dc:subject`, `dc:issued`
- **CGDP domain metadata** - for government/NIH website compliance
  - `cgdp:domain`, `cgdp:keywords`, `cgdp:category`
- **Author and publication metadata** - for trust signals
  - author name/email, publication date, last modified date
- **Schema markup (JSON-LD)** - for AI/LLMO understanding
  - Article schema, BreadcrumbList, Organization schema

**B. Build the page structure and write content:**

- Build the page structure:
  - H1: includes the primary keyword and matches user intent.
  - H2/H3: based on top user questions from Step 1.
  - FAQ block: 3-5 common user questions in plain language.
- Place keywords naturally:
  - Primary keyword in title tag, meta description, and H1.
  - Secondary keywords in subheadings and body content.
- Keep the content easy to read for non-technical audiences:
  - short paragraphs
  - plain language
  - clear action-oriented headings
- Improve trust and navigation:
  - add 2-5 relevant internal links
  - add external links to authoritative sources when needed
  - optimize images with descriptive alt text and compressed size

**C. Update XML Sitemap:**

- Ensure XML sitemap file (sitemap.xml) includes all new/updated pages
- Submit updated sitemap to Google via [Google Search Console](https://search.google.com/search-console/about)
- Submit to Bing via [Bing Webmaster Tools](https://www.bing.com/webmasters)

**D. Configure Robots.txt:**

- Ensure robots.txt file is correctly configured at the root of your website
- Allow search engine crawlers to access important pages
- Block sensitive pages or duplicate content if needed
- Verify robots.txt configuration in [Google Search Console](https://search.google.com/search-console/about)

**Example XML Sitemap snippet (save as `/sitemap.xml`):**

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url>
    <loc>https://example.com/page1</loc>
    <lastmod>2026-04-15</lastmod>
    <changefreq>weekly</changefreq>
    <priority>0.8</priority>
  </url>
  <url>
    <loc>https://example.com/page2</loc>
    <lastmod>2026-04-15</lastmod>
    <changefreq>monthly</changefreq>
    <priority>0.6</priority>
  </url>
</urlset>
```

**Example Robots.txt snippet (save as `/robots.txt`):**

```text
# Allow all search engines to crawl the site
User-agent: *
Allow: /

# Block specific low-value pages
Disallow: /admin/
Disallow: /login/
Disallow: /search/
Disallow: /*?*  # Block URLs with query parameters (duplicates)

# Sitemap location
Sitemap: https://example.com/sitemap.xml

# Respect crawl delay (optional)
Crawl-delay: 2
```

**Tools and how they help:**

- **[Meta Tags](https://metatags.io/)** `Free` - Preview and generate OG/Twitter card tags
- **[Schema.org validator](https://validator.schema.org/)** `Free` - Validate schema markup
- **[Google SERP Snippet Preview tools](https://mangools.com/free-seo-tools/serp-simulator)** `Free/Freemium` - Preview how title and meta description may appear in search results
- **[Hemingway Editor](https://hemingwayapp.com/)** `Free/Freemium` or **[Grammarly](https://www.grammarly.com/)** `Freemium` - Simplify language for non-technical readers
- **[Google Search Console](https://search.google.com/search-console/about)** `Free` - Confirm if pages improve CTR and query relevance over time
- **[XML Sitemap Generator](https://www.xml-sitemaps.com/)** `Free/Freemium` - Auto-generate sitemap.xml from your website
- **[Robots.txt Tester](https://www.google.com/webmasters/tools/robots-testing-tool)** `Free` - Test and validate robots.txt rules in Google Search Console
- **[Bing Webmaster Tools](https://www.bing.com/webmasters)** `Free` - Submit and monitor sitemap in Bing

**Example metadata snippet (add to page `<head>`):**

```html
<!-- Open Graph -->
<meta property="og:title" content="Page Title Here" />
<meta property="og:description" content="Short description for social sharing" />
<meta property="og:image" content="https://example.com/image.jpg" />
<meta property="og:url" content="https://example.com/page" />

<!-- Twitter Card -->
<meta name="twitter:card" content="summary_large_image" />
<meta name="twitter:title" content="Page Title Here" />
<meta name="twitter:image" content="https://example.com/image.jpg" />

<!-- Dublin Core -->
<meta name="dc:creator" content="Author Name" />
<meta name="dc:publisher" content="CCDI" />
<meta name="dc:date" content="2026-04-15" />

<!-- CGDP (Government) -->
<meta name="cgdp:domain" content="nih.gov" />
<meta name="cgdp:category" content="Health/Data" />
```

**Output checklist:**

- OG and Twitter card tags added/updated
- Dublin Core creator, publisher, and date fields set
- CGDP domain tags included (if applicable to NIH/government site)
- Schema.org JSON-LD markup added
- Final page title tag and meta description
- H1 and H2/H3 outline
- FAQ questions added
- Internal/external links added
- Image alt text updated
- Publish date and owner
- Tested in [Meta Tags](https://metatags.io/) tool

## Step 3: Page Speed Optimization

**Frequency:** Quarterly or after major updates

**Why this step matters:**

Search engines and visitors both prefer fast-loading pages. A slow website hurts user experience, increases bounce rate, and lowers your search rankings. Page speed is also a ranking factor for both desktop and mobile. Fast pages also improve AI/LLMO crawling efficiency, making your content easier to index and cite.

**What to do:**

**A. Measure current page speed:**

- Run [PageSpeed Insights](https://pagespeed.web.dev/) `Free` on each key page (desktop and mobile).
- Record scores for:
  - Largest Contentful Paint (LCP) - target: under 2.5 seconds
  - First Input Delay (FID) - target: under 100 milliseconds
  - Cumulative Layout Shift (CLS) - target: under 0.1
- Note which pages need optimization.

**B. Optimize images:**

- Compress all images to reduce file size without losing quality.
- Convert images to modern formats (WebP instead of JPG/PNG where possible).
- Use responsive images that scale for mobile, tablet, and desktop.
- Add lazy loading so images load only when visible on screen.

**C. Reduce JavaScript and CSS:**

- Minify (compress) JavaScript and CSS files.
- Remove unused code and third-party scripts.
- Load critical CSS inline instead of external files.
- Defer non-critical JavaScript to load after page content.

**D. Enable browser caching:**

- Set up cache headers so browsers store static assets (images, CSS, JS) locally.
- Enable server-side caching for frequently accessed content.
- Use Content Delivery Networks (CDN) to serve content from servers closer to users.


**Tools and how they help:**

- **[PageSpeed Insights](https://pagespeed.web.dev/)** `Free` - Measures page speed and provides specific optimization suggestions
- **[GTmetrix](https://gtmetrix.com/)** `Free/Freemium` - Detailed performance reports with waterfall charts
- **[Google Lighthouse](https://developers.google.com/web/tools/lighthouse)** `Free` - Built-in browser tool (Chrome DevTools) for auditing performance
- **[WebP Converter](https://cloudconvert.com/webp)** `Free/Freemium` - Convert images to modern formats
- **[Cloudflare](https://www.cloudflare.com/)** `Freemium` - CDN and caching layer to speed up content delivery
- **[Google Search Console](https://search.google.com/search-console/about)** `Free` - Monitor Core Web Vitals for your entire site

**Example optimization quick-start:**

```
Step 1: Check current speed with PageSpeed Insights
Step 2: Identify top 3 slowest pages
Step 3: Compress images (biggest impact usually)
Step 4: Enable caching in server settings
Step 5: Re-test to confirm improvement
Step 6: Aim for Core Web Vitals passing score
```

**Output checklist:**

- Baseline page speed scores recorded (desktop and mobile)
- Images compressed and converted to modern format
- JavaScript and CSS minified
- Browser caching enabled
- CDN deployed (if applicable)
- Mobile responsiveness verified
- Core Web Vitals passing
- Re-test scores documented and compared to baseline
- Page speed improvement target achieved (e.g., 10% faster)

## Step 4: Build External Links and Authority

**Frequency:** Monthly

**Why this step matters:**

Search engines view external links pointing to your site (backlinks) as "votes of confidence." High-quality backlinks from authoritative websites improve your domain authority, boost rankings, and help AI tools recognize your content as trustworthy. Building backlinks takes time and relationship-building, not shortcuts.

**What to do:**

**A. Identify backlink opportunities:**

- Find websites in your industry or related fields that mention topics relevant to your content.
- Look for:
  - Industry directories and resource lists
  - Partner organizations and collaborators
  - Health/government sites that could reference your data
  - News outlets and research blogs
  - Academic or professional associations

**B. Develop a link-building strategy:**

- **Partnerships:** Reach out to partner organizations to add mutual links.
- **Guest posting:** Write articles for reputable industry blogs with a link back to your site.
- **Outreach:** Politely contact relevant websites and offer value (resource, data, collaboration).
- **Resource pages:** Ask to be added to "best resources" or "helpful links" pages.
- **Press releases:** Announce major updates or new datasets to news outlets.

**C. Monitor and track backlinks:**

- Use backlink tracking tools to see which sites link to you.
- Check domain authority of linking sites (quality > quantity).
- Record new backlinks monthly.
- Remove or disavow low-quality or spam links.

**D. Create link-worthy content:**

- Regular research, datasets, or tools that others want to share.
- Infographics and visual content that attract citations.
- Whitepapers and case studies.
- Comprehensive guides and frameworks.

**Tools and how they help:**

- **[Ahrefs](https://ahrefs.com/)** `Paid` - Detailed backlink analysis and competitor research
- **[SEMrush Backlink Tool](https://www.semrush.com/)** `Paid (trial available)` - Monitor and analyze backlinks
- **[Google Search Console](https://search.google.com/search-console/about)** `Free` - See backlinks discovered by Google
- **[Moz Link Explorer](https://moz.com/link-explorer)** `Freemium` - Analyze link profile and domain authority
- **[BuzzSumo](https://buzzsumo.com/)** `Freemium` - Find shareable content and linking opportunities

**Output checklist:**

- List of 10+ potential partner/backlink websites identified
- Guest posting opportunities targeted
- Outreach emails sent (record template and results)
- Monthly backlink count tracked
- Domain authority of linking sites monitored
- Low-quality backlinks identified and marked for removal
- New backlinks from high-authority sites documented
- Monthly report on backlink growth showing trend

## Step 5: Keep Content Fresh and Relevant

**Frequency:** Weekly (planning) / Monthly (execution)

**Why this step matters:**

Search engines reward fresh, updated content. Old pages with outdated information rank lower and may confuse users and AI tools. Regular content updates signal that your site is active and maintained. Updating existing pages is often more effective than creating entirely new pages because you're improving content that already has some authority.

**What to do:**

**A. Create a content calendar:**

- Plan new content aligned with audience questions (from Step 1).
- Assign creation to team members with clear deadlines.
- Mix new pages with updates to existing high-traffic pages.
- Balance frequency with quality (consistent but not rushed).

**B. Publish new content regularly:**

- Follow the SEO format from Steps 1-2 for each new page.
- Include keywords, headings, FAQ, internal links, and metadata.
- Ensure plain language for non-technical audiences.
- Add publication date and author bio.
- Schedule content releases to maintain steady flow.

**C. Update existing pages quarterly:**

- Review top 10 pages by traffic in [Google Search Console](https://search.google.com/search-console/about).
- Check for:
  - Outdated statistics or references
  - New developments or trends in the field
  - Broken links or outdated tool/product mentions
  - Opportunities to add new keywords or sections
- Add an "Updated [date]" note at the top or bottom.
- Republish to signal freshness to search engines.

**D. Maintain consistency:**

- Use the same tone, terminology, and style across all pages.
- Keep formatting consistent (headings, bullet points, font sizes).
- Update internal links when content changes.
- Archive old content rather than deleting (use redirect if necessary).

**E. Plan topic expansion:**

- Group related pages into topic clusters (main topic + supporting pages).
- Link them together with relevant anchor text.
- Update the main page when new supporting pages are published.
- Use keyword variations across the cluster.

**Tools and how they help:**

- **[Google Search Console](https://search.google.com/search-console/about)** `Free` - Identify top pages and their performance
- **[Content Calendar (Google Sheets or Asana)](https://asana.com/)** `Free/Freemium` - Plan and track content publication
- **[Yoast SEO](https://yoast.com/wordpress/plugins/seo/)** `Freemium` - Maintain SEO consistency across pages
- **[Google Analytics](https://analytics.google.com/)** `Free` - Track which content drives engagement
- **[Hemingway Editor](https://hemingwayapp.com/)** `Free/Freemium` - Keep writing clear and accessible

**Example content update checklist:**

```
QUARTERLY UPDATE PROCESS:
1. Export top 20 pages from Google Search Console
2. Review each page for outdated info
3. Update statistics, links, and examples
4. Add "Updated [date]" timestamp
5. Republish with updated slug/metadata if changed
6. Re-check page speed (Step 3)
7. Test all internal and external links
8. Monitor how changes affect CTR in 2-4 weeks
```

**Output checklist:**

- Content calendar created and approved by team
- New content published at planned frequency
- All new pages follow Steps 1-2 format
- Quarterly review of top 20 pages completed
- Outdated information updated with current data
- Publication/update dates visible on pages
- Consistency check: tone, terminology, style
- Internal links within topic clusters created
- Broken links identified and repaired
- Redirect rules set up for archived content
- Monthly publication and update count tracked

## Step 6: Monitor Performance and Report Results

**Frequency:** Weekly (quick check) / Monthly (full report)

**Why this step matters:**

You cannot improve what you don't measure. Regular monitoring shows whether your SEO efforts are working. Reports keep stakeholders informed, justify continued investment, and help identify problems early. Performance data guides what to do next (which strategies work, which need adjustment).

**What to do:**

**A. Set baseline metrics:**

- Record starting numbers for:
  - Organic traffic (sessions from search)
  - Keyword rankings (for 20-50 key terms)
  - Click-through rate (CTR) from search results
  - Pages indexed by Google
  - Average page speed
  - Bounce rate
  - Conversion rate (if applicable)

**B. Monitor weekly (quick check):**

- Check [Google Search Console](https://search.google.com/search-console/about) for:
  - New search queries driving clicks
  - Pages with high impressions but low CTR (improvement opportunity)
  - Crawl errors or indexing issues
  - Manual penalties or alerts
- Check [Google Analytics](https://analytics.google.com/) for:
  - Organic traffic trends
  - Top landing pages
  - Pages with high bounce rate
  - Device performance (mobile vs desktop)

**C. Monitor monthly (detailed review):**

- Update keyword ranking tracker (target keywords' positions in search results).
- Compare metrics month-over-month:
  - Traffic growth % (target: 5-15% monthly)
  - Ranking improvements (which keywords moved up/down)
  - CTR changes
  - Conversion rate changes
- Review which pages drive the most traffic and conversions.
- Identify pages that need improvement (high traffic but low conversion, or low traffic).

**D. Create monthly SEO report:**

- Include:
  - Executive summary (key wins, areas to improve)
  - Traffic overview (organic sessions, users, sessions per page)
  - Keyword rankings (top 20 keywords and their positions)
  - Page performance (top 10 pages by traffic)
  - Issues found and fixes applied
  - Technical issues (broken links, crawl errors, Core Web Vitals)
  - Backlinks added
  - Content published or updated
  - Recommendations for next month
- Store in shared drive (NIH SharePoint) for team access.

**E. Track progress toward goals:**

- Set quarterly or annual SEO goals:
  - Example: "Increase organic traffic by 50% in 6 months"
  - Example: "Rank 30+ keywords in top 3 positions"
  - Example: "Achieve 25% conversion rate from organic search"
- Review progress monthly and adjust tactics if needed.
- Celebrate wins and learn from underperforming initiatives.

**Tools and how they help:**

- **[Google Search Console](https://search.google.com/search-console/about)** `Free` - Track search impressions, clicks, CTR, and keywords
- **[Google Analytics](https://analytics.google.com/)** `Free` - Monitor organic traffic, user behavior, conversions
- **[Rank Tracker (SE Ranking or Semrush)](https://www.semrush.com/)** `Freemium/Paid` - Track keyword rankings over time
- **[Data Studio (Google Looker Studio)](https://datastudio.google.com/)** `Free` - Create automated visual reports
- **[Excel or Google Sheets](https://sheets.google.com/)** `Free` - Build custom tracking spreadsheets
- **[Slack integration](https://slack.com/)** `Free/Freemium` - Get weekly alerts on key metrics

**Example monthly report template:**

```
SEO PERFORMANCE REPORT - [Month]

EXECUTIVE SUMMARY:
- Organic traffic: X sessions (+Y% vs last month)
- Top performing page: [Page Name] - Z sessions
- New keywords ranking in top 10: [Count]

KEY METRICS:
- Organic Sessions: X
- Avg CTR: X%
- Avg Page Position: X
- Pages Indexed: X
- Core Web Vitals Status: [Good/Needs Work]

TOP 10 KEYWORDS & RANKINGS:
[Table with keyword, search volume, current position, target]

ACTIONS TAKEN:
- [Content update/new page/link built/speed optimization]
- [Issue fixed]

NEXT MONTH PRIORITIES:
- [Action item 1]
- [Action item 2]
```

**Output checklist:**

- Baseline metrics recorded at project start
- Weekly monitoring system set up
- Monthly reporting schedule established
- SEO report template created and shared
- Google Search Console configured and reviewed
- Google Analytics 4 set up with proper tracking
- Keyword rank tracker implemented
- Monthly reports completed and stored in shared drive
- Stakeholder meetings scheduled to review performance
- Goals set and progress tracked monthly
- Issues identified and action items assigned
- Improvement trends documented for reporting




# GEO, AEO & LLMO: Optimizing for AI-Driven Search

**What this means:**

Traditional SEO focuses on ranking in Google search results. But user behavior is shifting: more people use AI tools like ChatGPT, Claude, Perplexity, and Google's AI Overview to get direct answers without browsing web pages. This section covers how to optimize your content so AI tools cite, trust, and surface your information.

## What are GEO, AEO, and LLMO?

**LLMO (Large Language Model Optimization)**
- Goal: Make your content visible and citable to AI chatbots and language models
- Focus: Clear structure, authoritative tone, trustworthy sources
- Impact: AI tools cite your site when answering related questions

**GEO (Generative Engine Optimization)**
- Goal: Get your content cited by generative AI search engines
- Focus: Answer-ready format, structured data, E-E-A-T (Experience, Expertise, Authoritativeness, Trustworthiness)
- Tools: ChatGPT, Claude, Perplexity, Google's AI Overview

**AEO (Answer Engine Optimization)**
- Goal: Appear in featured snippets and voice search results
- Focus: Direct answers, conversational language, question-based targeting
- Tools: Google's "People Also Ask," voice assistants, featured snippets

---

## GEO (Generative Engine Optimization) Tactics

**Why this matters for CCDI:**

AI tools often cite healthcare and research data when users ask health questions. If your CCDI data is well-structured and trustworthy, AI tools will use it as a source—driving discovery and establishing authority.

**1. Write in "answer-ready" format**

Make content easy for AI to extract and understand:

- Use clear headings that mirror common questions:
  - "What is pediatric cancer data?"
  - "How do I access CCDI datasets?"
  - "Who can use CCDI resources?"
- Place the short answer summary at the very top (first 40-60 words)
- Then expand with details, examples, and caveats
- Use bullet points and numbered lists (easier for AI to parse)
- Avoid vague language; be specific and factual

**Example:**

**Poor (vague):** "CCDI has cancer data."

**Better (AI-friendly):** "The Cancer Moonshot Data Initiative (CCDI) provides standardized pediatric cancer datasets including patient outcomes, tumor genomics, and treatment records from participating research institutions, accessible to researchers and clinicians via secure portals."

**2. Add structured data (Schema markup)**

Tell search engines and AI explicitly what your content means:

- **FAQ Schema** — Mark FAQ sections so AI recognizes Q&A pairs
- **Article Schema** — Declare article title, author, publication date
- **Organization Schema** — Identify your organization (NIH, CCDI) with logo, mission, contact
- **Dataset Schema** — For data resources, describe dataset name, description, access instructions
- **BreadcrumbList Schema** — Help AI understand page hierarchy

*(Already covered in Step 2's metadata section)*

**3. Build E-E-A-T signals (Experience, Expertise, Authoritativeness, Trustworthiness)**

AI evaluates source credibility. Show you're trustworthy:

- **Experience:** Include real-world examples, case studies, and use cases
- **Expertise:** Cite author credentials, institutional affiliations (NIH, NCI, university)
- **Authoritativeness:** Reference peer-reviewed research, government frameworks, industry standards
- **Trustworthiness:** Cite sources, link to authoritative sites, be transparent about limitations

**Example:**

Include author bio: "Dr. Jane Smith, PhD in Oncology, National Cancer Institute, 15+ years cancer research"

**4. Create "citation-worthy" content**

AI tools prefer content that directly answers questions:

- **Definitions:** Clear explanations of complex terms
- **Statistics:** Recent, specific numbers with sources
- **Original insights:** Research findings, analysis, frameworks unique to your data
- **Curated resources:** Lists, comparisons, roadmaps

**Example:** Instead of writing "cancer data is important," include:
"Pediatric cancer mortality rates differ by tumor type: 5-year survival is 90% for acute lymphoblastic leukemia vs. 40% for high-grade gliomas (NCI SEER database, 2023)."

---

## AEO (Answer Engine Optimization) Tactics

**Why this matters for CCDI:**

People increasingly ask voice questions ("What's the survival rate for childhood leukemia?") or scroll "People Also Ask" boxes in Google. AEO gets your answers in front of these users.

**1. Target specific questions users actually ask**

Discover real questions:

- Check "People Also Ask" boxes on Google for your keywords
- Review your Google Search Console for query questions
- Monitor Reddit, forums, and social media for unmet questions
- Survey your actual users (researchers, clinicians)

**Example questions for CCDI:**
- "How do I find cancer data by age group?"
- "What clinical data does CCDI have?"
- "Is CCDI data downloadable?"

**2. Provide concise, direct answers**

Featured snippets and voice results show short answers:

- **40-60 word rule:** Lead with a single-sentence answer, then expand
- **Paragraph format:** Answer in 1-3 sentences at the top of the section
- **Bullet lists:** Optimal for comparison questions
- **Tables:** Best for structured data (e.g., dataset names, availability)

**Example structure for "What data does CCDI have?"**

```
[SNIPPET - 40-60 words]
CCDI provides standardized pediatric cancer datasets including 
tumor genomics, patient outcomes, and treatment records from 
National Cancer Institute partner institutions. Data is available 
through secure portals to eligible researchers and clinicians.

[DETAILED SECTION BELOW]
Types of data available:
- Genomic (mutation, copy number, gene expression)
- Clinical (demographics, treatment, outcomes)
- Imaging (radiology and pathology reports)

Data access requirements vary by dataset...
```

**3. Add FAQ sections with schema markup**

Structure Q&A clearly:

- Place FAQ sections near the end of long pages
- Use natural questions users ask
- Keep answers concise (2-3 sentences) with links for details
- Mark with FAQ schema (covered in Step 2)

**Example FAQ for data portal page:**

```
Q: How long does it take to get access?
A: Most requests are processed within 5 business days. 
   Institutional users may expedite access through 
   their IRB pre-approvals.

Q: Can I download data offline?
A: Yes, approved users can download datasets in 
   CSV or JSON formats for offline analysis.
```

**4. Optimize for voice search**

Voice queries are conversational and longer:

- Include natural phrases: "How do I...," "What's the best way to...," "Tell me about..."
- Answer with simple, clear language (no jargon-heavy definitions)
- Include location data if relevant (e.g., "CCDI data partner institutions in your region")
- Keep sentences short and direct

**Example voice-friendly content:**

**Poor:** "The Cancer Moonshot Data Initiative endeavors to synergize oncological genomic and clinical datasets."

**Better:** "CCDI brings together cancer datasets from research hospitals and universities so researchers can find what they need faster."

---

## LLMO (Large Language Model Optimization) Checklist

Use this checklist before publishing high-priority pages:

- Answer appears in the first section of the page.
- Headings are question-based and easy to scan.
- Facts and statistics include sources and dates.
- Author and organization credibility are visible.
- Schema and metadata are complete.
- Page loads fast and works well on mobile.
- Internal links connect related pages and datasets.
- Terminology is consistent across related content.

## How GEO, AEO, and LLMO Connect to the Main Procedure

- Step 1 discovers real user questions and intent.
- Step 2 structures metadata and answer-ready content.
- Step 3 improves speed and crawlability.
- Step 4 builds authority through trusted backlinks.
- Step 5 keeps information current and reliable.
- Step 6 validates impact and informs the next cycle.

Key takeaway:
If your team follows Steps 0-6 consistently, GEO/AEO/LLMO performance improves naturally over time.

# Review and Update

Review this SOP every 6 months, or sooner when significant search engine or AI platform changes occur. Incorporate feedback from stakeholders and performance reports to keep this SOP current and practical.

