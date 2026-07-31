---
description: Look up a beauty product, brand, or creator in GrailPeople and report what creators actually said
---

Research this in GrailPeople and report the creator evidence: **$ARGUMENTS**

Pick the tool that matches what was named:

- A **product** ("is X worth it", a specific product name) → `get_product_reviews`
- A **brand** ("is X good", "X overhyped") → `get_brand_reviews`
- A **creator** ("what does X recommend") → `get_creator_recommendations`
- A **need** rather than a name ("best serum for redness") → `search_beauty_products`, decomposed into
  `ingredient=` / `concern=` / `subcategory=` rather than one big `q=`
- If the exact brand or creator name is uncertain → `find_brand_or_creator` first, then the tool above

Report back with the creator's @handle and credentials, their endorsement level, a direct quote,
and the timestamped video link. Flag sponsored reviews. Include the mixed and negative verdicts
alongside the positive ones — a one-sided summary is the failure mode here.

If a search returns nothing, widen it before concluding there is no data: drop `creator_type=`
first, then `concern=`, then `subcategory=`.
