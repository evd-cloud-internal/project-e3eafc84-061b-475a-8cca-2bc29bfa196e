---
name: Home
assetId: bc1c98b0-af83-490e-8ef5-e5590eb15382
type: page
---

{% dropdown
    id="category_filter"
    data="demo_daily_orders"
    value_column="category"
/%}

{% table
    data="demo_daily_orders"
%}
{% dimension
    value="category"
    link="concat('/category-detail?category_filter=',category)"
/%}
{% /table %}