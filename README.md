# brand-list
Brand list for macys.com


1.Get list of Categories: 
    https://api.macys.com/v4/catalog/category
    TODO: try limiting to top level only using Apollo

2. Find Brands by Categories for user to select and display on App or UI
    https://api.macys.com/v4/catalog/category/brandindex/3111?refcatid=118
    This is done a during initial setup and when modifications to brand List is required
    
3. Identify New product arrivals based on specific Brand choosen
    Search for Products
    https://api.macys.com/v4/catalog/search?searchphrase=coach&BRAND=COACH&CATEGORY=[women]
    TODO: Too much details. Try to filter only for <badge>
    Products have "New" badge for a month.
    TODO: Identify when this product was introduced and when last notification was sent to prevent repeaded push notifications for same product
