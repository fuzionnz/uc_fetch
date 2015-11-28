# Fetch for Ubercart

Fetch is an implementation of Flo2Cash's Web2Pay service provided by Kiwibank in NZ.

## Download

The official code is available from www.fetchpayments.co.nz

* Download [UC Fetch from Fetch Payments NZ](https://www.fetchpayments.co.nz/help/supported-shopping-carts-for-fetch-web-payments/)
* [Merchant implementation docs](https://www.fetchpayments.co.nz/yk-files/501ccf687c122dcb3a39dd69630d0da3/Fetch%20Web%20Payments%20Integration%20Guide_July2015.pdf)
* [Github repo for uc_fetch](https://github.com/fuzionnz/uc_fetch) (this is an *unofficial* fork)

## Known issues

* Web2Pay doesn't accept negative or zero value items, no go for line items such as discounts.
* Fetch is not visible at `admin/store/settings/payment`?
* Page at `cart/checkout/review` feels a bit surplus to requirements.
* Should use `drupal_http_request()` not `curl_*()`.
* `_uc_fetch_callAPI()` says "Invalid URL" regardless of what triggers the exception.
* Get project onto Drupal.org so it has an issue queue and security updates.
* Maybe merge with existing Web2Pay methods instead of duplicating?
