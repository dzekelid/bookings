---
name: Bookeo
x-slug: bookeo
description: Bookeo provides a leading online booking and scheduling system for tours,
  classes, and appointments, to help you save money and time. Click to learn more!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
x-kinRank: "7"
x-alexaRank: "23042"
tags: Bookings
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/apis.md
specificationVersion: "0.14"
apis:
- name: Bookeo - Retrieve bookings
  x-api-slug: bookings-get
  description: |-
    Retrieve existing bookings
     The result is limited by the permissions of the apiKey.
     <p/>
     It is possible to filter by time booked and/or time of the last change.
     To filter by time booked, the parameters startTime and endTime are required.
     To filter by last time changed, the parameters lastUpdatedStartTime and lastUpdatedEndTime are required.
     It is possible to filter by both at the same time. At least one of the two filters must be used.
     <p/>
     It is further possible to filter by product id.
     <p/>
     Do not use this method to periodically poll for new/changed bookings. Use webhooks (see API general documentation) instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookings-get-openapi.md
- name: Bookeo - Create a new booking
  x-api-slug: bookings-post
  description: |-
    When creating a booking for a product of type "fixed" or "fixedCourse", the eventId is required. eventIds are obtained by calling /availability/slots or /availability/matchingSlots .
     When creating a booking for a product of type "flexibleTime", you can either specify the eventId or the startTime (in which case you can optionally specify the endTime. If no endTime is specified, Bookeo will automatically calculate the duration based on the options chosen)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookings-post-openapi.md
- name: Bookeo - Retrieve a booking
  x-api-slug: bookingsbookingnumber-get
  description: Retrieve a booking by its booking number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-get-openapi.md
- name: Bookeo - Update an existing booking
  x-api-slug: bookingsbookingnumber-put
  description: Update an existing booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-put-openapi.md
- name: Bookeo - Cancel a booking
  x-api-slug: bookingsbookingnumber-delete
  description: Cancel a booking. Cancelled bookings remain in the system, but no longer
    show up in the calendar or take up seats.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-delete-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Get the payments received for a booking
  x-api-slug: bookingsbookingnumberpayments-get
  description: Get a list of all payments received for a booking. Only payments for
    which the apiKey has at least read permission will be included
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-get-openapi.md
- name: Bookeo - Add a payment to a booking
  x-api-slug: bookingsbookingnumberpayments-post
  description: Create a payment record associated with a booking
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-post-openapi.md
- name: Bookeo - Retrieve a customer's bookings
  x-api-slug: customersidbookings-get
  description: Retrieve a customer's bookings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/customersidbookings-get-openapi.md
- name: Bookeo - Retrieve a booking
  x-api-slug: bookingsbookingnumber-get
  description: Retrieve a booking by its booking number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-get-openapi.md
- name: Bookeo - Update an existing booking
  x-api-slug: bookingsbookingnumber-put
  description: Update an existing booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-put-openapi.md
- name: Bookeo - Cancel a booking
  x-api-slug: bookingsbookingnumber-delete
  description: Cancel a booking. Cancelled bookings remain in the system, but no longer
    show up in the calendar or take up seats.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-delete-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Get the payments received for a booking
  x-api-slug: bookingsbookingnumberpayments-get
  description: Get a list of all payments received for a booking. Only payments for
    which the apiKey has at least read permission will be included
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-get-openapi.md
- name: Bookeo - Add a payment to a booking
  x-api-slug: bookingsbookingnumberpayments-post
  description: Create a payment record associated with a booking
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-post-openapi.md
- name: Bookeo - Retrieve a booking
  x-api-slug: bookingsbookingnumber-get
  description: Retrieve a booking by its booking number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-get-openapi.md
- name: Bookeo - Update an existing booking
  x-api-slug: bookingsbookingnumber-put
  description: Update an existing booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-put-openapi.md
- name: Bookeo - Cancel a booking
  x-api-slug: bookingsbookingnumber-delete
  description: Cancel a booking. Cancelled bookings remain in the system, but no longer
    show up in the calendar or take up seats.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-delete-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Get the payments received for a booking
  x-api-slug: bookingsbookingnumberpayments-get
  description: Get a list of all payments received for a booking. Only payments for
    which the apiKey has at least read permission will be included
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-get-openapi.md
- name: Bookeo - Add a payment to a booking
  x-api-slug: bookingsbookingnumberpayments-post
  description: Create a payment record associated with a booking
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-post-openapi.md
- name: Bookeo - Add a payment to a booking
  x-api-slug: bookingsbookingnumberpayments-post
  description: Create a payment record associated with a booking
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-post-openapi.md
- name: Bookeo - Add a payment to a booking
  x-api-slug: bookingsbookingnumberpayments-post
  description: Create a payment record associated with a booking
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-post-openapi.md
- name: Bookeo - Get the payments received for a booking
  x-api-slug: bookingsbookingnumberpayments-get
  description: Get a list of all payments received for a booking. Only payments for
    which the apiKey has at least read permission will be included
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-get-openapi.md
- name: Bookeo - Get the payments received for a booking
  x-api-slug: bookingsbookingnumberpayments-get
  description: Get a list of all payments received for a booking. Only payments for
    which the apiKey has at least read permission will be included
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumberpayments-get-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Retrieve the customer associated with a booking
  x-api-slug: bookingsbookingnumbercustomer-get
  description: Retrieve the customer associated with a booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumbercustomer-get-openapi.md
- name: Bookeo - Cancel a booking
  x-api-slug: bookingsbookingnumber-delete
  description: Cancel a booking. Cancelled bookings remain in the system, but no longer
    show up in the calendar or take up seats.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-delete-openapi.md
- name: Bookeo - Cancel a booking
  x-api-slug: bookingsbookingnumber-delete
  description: Cancel a booking. Cancelled bookings remain in the system, but no longer
    show up in the calendar or take up seats.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-delete-openapi.md
- name: Bookeo - Update an existing booking
  x-api-slug: bookingsbookingnumber-put
  description: Update an existing booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-put-openapi.md
- name: Bookeo - Update an existing booking
  x-api-slug: bookingsbookingnumber-put
  description: Update an existing booking.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-put-openapi.md
- name: Bookeo - Retrieve a booking
  x-api-slug: bookingsbookingnumber-get
  description: Retrieve a booking by its booking number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-get-openapi.md
- name: Bookeo - Retrieve a booking
  x-api-slug: bookingsbookingnumber-get
  description: Retrieve a booking by its booking number
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28769-www-bookeo-com.jpg
  humanURL: https://www.bookeo.com
  baseURL: https://api.bookeo.com//v2
  tags: Bookings, Schedules, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/bookings/master/_listings/bookeo/bookingsbookingnumber-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bmc.software.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bookeo.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bookeo
- type: x-developer
  url: https://www.bookeo.com/api/
- type: x-documentation
  url: https://www.bookeo.com/apiref/index.html
- type: x-partners
  url: https://www.bookeo.com/affiliate/
- type: x-privacy-policy
  url: https://www.bookeo.com/privacy/
- type: x-terms-of-service
  url: https://www.bookeo.com/termsofservice/
- type: x-twitter
  url: https://twitter.com/bookeo
- type: x-webhook
  url: https://www.bookeo.com/api/webhooks/
- type: x-website
  url: https://www.bookeo.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---