# Google Sheets Formulas

## Schedule Reports

```=SCHEDULEREPORTS(frequency);```

**Frequencies**

* Daily
* Weekly
* Monthly
* Quarterly
* Yearly

## Get URL Information

```const rootDomain = GETROOTDOMAIN(URL);```

Use regular expression to extract root domain from various URL formats

* https://www.example.com
* https://example.com
* http://www.example.com
* http://example.com
* www.example.com
* example.com

```const preferredURL = GETPREFERREDURL(rootDomain, format);```

**Formats**

* Spliced URL (Separated into Columns by Components)
* Combined URL (All Components Combined into Single Cell)

**Components**

* Connection
* Protocol
* Subdomain
* Root Domain

```=GETSOCIALPROFILEURLS(preferredURL);```

**Social Profile Links**

* Facebook
* Twitter
* Google+
* Instagram
* YouTube
* LinkedIn
* Myspace
* Pinterest
* SoundCloud
* Tumblr

```=GETBUSINESSNAME(preferredURL);```

```=GETLOGOIMAGEURL(preferredURL);```

## Google Keyword Planner

```=GOOGLESEARCHCONTEXT(keyword, locations);```

```=GOOGLEAVERAGEMONTHLYSEARCHES(searchContext);```

```=GOOGLESUGGESTEDBID(searchContext);```

```=GOOGLECOMPETITION(searchContext);```

## Google My Business

```const businessListing = GOOGLEMYBUSINESSLISTING(businessName, address);```

**Output**

* Status
* Store code
* Business name
* Address line 1
* Address line 2
* Address line 3
* Address line 4
* Address line 5
* Sub-locality
* Locality
* Administrative area
* Country
* Postal code
* Primary phone
* Additional phones
* Website
* Primary category
* Additional categories
* Sunday hours
* Monday hours
* Tuesday hours
* Wednesday hours
* Thursday hours
* Friday hours
* Saturday hours
* Special hours
* Profile photo
* Logo photo
* Cover photo
* Other photos
* Preferred photo
* Labels
* AdWords location extensions phone
* Accessibility: Wheelchair accessible (is_wheelchair_accessible)
* Accessibility: Wheelchair accessible elevator (has_wheelchair_accessible_elevator)
* Accessibility: Wheelchair accessible entrance (has_wheelchair_accessible_entrance)
* Accessibility: Wheelchair accessible parking lot (has_wheelchair_accessible_parking)
* Accessibility: Wheelchair accessible restroom (has_wheelchair_accessible_restroom)
* Amenities: Gift wrapping (has_gift_wrapping)
* Amenities: Restroom (has_restroom)
* Amenities: Unisex restroom (has_restroom_unisex)
* Offerings: Appraisals (has_appraisals_for_items)
* Offerings: Installation service (has_service_installation)
* Offerings: Repair services (has_service_repair)
* Offerings: Same-day delivery (has_delivery_same_day)
* Payments: Cash-only (requires_cash_only)
* Payments: Checks (pay_check)
* Payments: Credit cards (pay_credit_card)
* Payments: Debit cards (pay_debit_card)
* Payments: NFC mobile payments (pay_mobile_nfc)
* Place page URLs: Appointment URL (url_appointment)
* Place page URLs: Menu URL (url_menu)
* Planning: LGBTQ-friendly (welcomes_lgbtq)

```=GOOGLEMYBUSINESSTOTALSEARCHES(businessListing);```

```=GOOGLEMYBUSINESSDIRECTSEARCHES(businessListing);```

```=GOOGLEMYBUSINESSTOTALVIEWS(businessListing);```

```=GOOGLEMYBUSINESSSEARCHVIEWS(businessListing);```

```=GOOGLEMYBUSINESSMAPVIEWS(businessListing);```

```=GOOGLEMYBUSINESSTOTALACTIONS(businessListing);```

```=GOOGLEMYBUSINESSWEBSITEACTIONS(businessListing);```

```=GOOGLEMYBUSINESSDIRECTIONSACTIONS(businessListing);```

```=GOOGLEMYBUSINESSPHONECALLS(businessListing);```

**Output**

* Calls by Days of the Week
* Calls by Hours of the Day

```=GOOGLEMYBUSINESSREVIEWS(businessListing);```

**Output**

* Average Ratings
* Count Reviews
* Count Responses
