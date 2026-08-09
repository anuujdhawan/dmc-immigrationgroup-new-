# URLs NOT Present on the QATAR Website

Market site: **dm-consultant.qa**

Of the **61** legacy URLs listed in the QATAR sheet of `DMC_Legacy_URL_to_New_Menu_Mapping_WebsiteWise.xlsx`, the following **2** are **not present on the website** — they return **HTTP 404 (page not found)** when fetched directly.

> Verified live on 8 Aug 2026 with `curl -L` (following redirects). These are genuine 404 responses from WordPress, not extraction failures.

## Missing URLs

| # | Page Title | URL | HTTP Status | Sheet Details | Extract |
|---|------------|-----|-------------|---------------|---------|
| 1 | Residency By Investment | https://dm-consultant.qa/residency-by-investment/ | **404 Not Found** | New menu: Business & Investment > Residency — Canada · UK · USA | `pages/residency-by-investment.md` (stub) |
| 2 | Citizenship By Investment | https://dm-consultant.qa/citizenship-by-investment/ | **404 Not Found** | New menu: Business & Investment > Citizenship — St. Kitts · Vanuatu | `pages/citizenship-by-investment.md` (stub) |

## Details

### 1. Residency By Investment
- **URL:** https://dm-consultant.qa/residency-by-investment/
- **HTTP status:** 404 — the page does not exist on the Qatar site
- **Sheet mapping:** Business & Investment → submenu *Residency — Canada · UK · USA* (notes: "Matches new menu item")
- **Status:** A stub dataset file was created at `pages/residency-by-investment.md` so every sheet URL has a dataset, clearly marked as **not present on the live site**.

### 2. Citizenship By Investment
- **URL:** https://dm-consultant.qa/citizenship-by-investment/
- **HTTP status:** 404 — the page does not exist on the Qatar site
- **Sheet mapping:** Business & Investment → submenu *Citizenship — St. Kitts · Vanuatu* (notes: "Matches new menu item")
- **Status:** A stub dataset file was created at `pages/citizenship-by-investment.md` so every sheet URL has a dataset, clearly marked as **not present on the live site**.

## Notes

- All **59** other Qatar URLs returned **HTTP 200** and were extracted normally.
- These 2 URLs are also absent from the Qatar site's sitemap (see `URLS-NOT-IN-SITEMAP.md` for the full 9-URL sitemap comparison) — but note that 7 of those 9 URLs **do exist** on the site (they're just unlisted); only these 2 return 404.
- The stub files in `pages/` are marked with `> ⚠️ This page returns HTTP 404 on the live site` so they are never mistaken for real content.
