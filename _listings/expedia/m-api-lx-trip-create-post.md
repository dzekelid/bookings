---
swagger: "2.0"
info:
  title: Expedia
  description: 'Expedia Mobile API Documentation. &lt;br&gt;&lt;font color=&quot;blue&quot;&gt;
    (Note: In case of authorization exception, just &lt;a href=&quot;/static/mobile/swaggerui/#!/User/signin-user&quot;&gt;Sign-In&lt;/a&gt;)&lt;/font&gt;'
  version: 0.0.1
host: apim.expedia.com
basePath: x/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /m/api/lx/trip/create:
    post:
      summary: Create A Trip
      description: Mobile API Lx Create Trip
      operationId: lx-create-trip
      parameters:
      - in: body
        name: body
        description: Lx Trip consisting of chosen item information and trip name
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - travel
      - trips
definitions:
  lxTickets:
    properties:
      count:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
      ticketId:
        description: This is a default description.
        type: get
  lxItem:
    properties:
      activityId:
        description: This is a default description.
        type: get
      activityItemId:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      activityDate:
        description: This is a default description.
        type: get
      allDayActivity:
        description: This is a default description.
        type: get
      regionId:
        description: This is a default description.
        type: get
      tickets:
        description: This is a default description.
        type: get
  lxTrip:
    properties:
      items:
        description: This is a default description.
        type: get
      tripName:
        description: This is a default description.
        type: get
  latLongDomain:
    properties:
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
  timeDomain:
    properties:
      raw:
        description: This is a default description.
        type: get
      localized:
        description: This is a default description.
        type: get
      epochSeconds:
        description: This is a default description.
        type: get
      timeZoneOffsetSeconds:
        description: This is a default description.
        type: get
      localizedShortDate:
        description: This is a default description.
        type: get
  hotelCheckoutV2:
    properties: []
  railsCheckout:
    properties:
      travelers:
        description: This is a default description.
        type: get
  hotelCheckoutFields:
    properties:
      checkInDate:
        description: This is a default description.
        type: get
      checkOutDate:
        description: This is a default description.
        type: get
      rooms:
        description: This is a default description.
        type: get
  jsonValueAdd:
    properties:
      id:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
  roomsDetails:
    properties:
      bedTypeId:
        description: This is a default description.
        type: get
      contactName:
        description: This is a default description.
        type: get
      smokingPreference:
        description: This is a default description.
        type: get
      specialRequests:
        description: This is a default description.
        type: get
      accessibilityOptionIds:
        description: This is a default description.
        type: get
  mainHotelTraveler:
    properties:
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
      phoneCountryCode:
        description: This is a default description.
        type: get
      phone:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      password:
        description: This is a default description.
        type: get
      expediaEmailOptIn:
        description: This is a default description.
        type: get
      bedTypeId:
        description: This is a default description.
        type: get
  checkoutFields:
    properties:
      tripId:
        description: This is a default description.
        type: get
      expectedTotalFare:
        description: This is a default description.
        type: get
      expectedFareCurrencyCode:
        description: This is a default description.
        type: get
      expectedCardFee:
        description: This is a default description.
        type: get
      expectedCardFeeCurrencyCode:
        description: This is a default description.
        type: get
      doIThinkImSignedIn:
        description: This is a default description.
        type: get
      tealeafTransactionId:
        description: This is a default description.
        type: get
      omniturePartnerId:
        description: This is a default description.
        type: get
      sendEmailConfirmation:
        description: This is a default description.
        type: get
      abacusUserGuid:
        description: This is a default description.
        type: get
  paymentFieldsRef:
    properties:
      streetAddress:
        description: This is a default description.
        type: get
      streetAddress2:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      postalCode:
        description: This is a default description.
        type: get
      creditCardNumber:
        description: This is a default description.
        type: get
      expirationDateYear:
        description: This is a default description.
        type: get
      expirationDateMonth:
        description: This is a default description.
        type: get
      cvv:
        description: This is a default description.
        type: get
      storedCreditCardId:
        description: This is a default description.
        type: get
  rewardsCheckoutFields:
    properties:
      membershipId:
        description: This is a default description.
        type: get
      programName:
        description: This is a default description.
        type: get
      paymentInstrumentId:
        description: This is a default description.
        type: get
      amountToChargeInVirtualCurrency:
        description: This is a default description.
        type: get
      amountToChargeInRealCurrency:
        description: This is a default description.
        type: get
      rateId:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
  utilityFields:
    properties:
      prettyPrint:
        description: This is a default description.
        type: get
      suppressFinalBooking:
        description: This is a default description.
        type: get
      clientId:
        description: This is a default description.
        type: get
      teaLeafTransactionId:
        description: This is a default description.
        type: get
  paymentInfoFields:
    properties:
      cards:
        description: This is a default description.
        type: get
      rewards:
        description: This is a default description.
        type: get
      deviceBlackBoxDetails:
        description: This is a default description.
        type: get
  applePayTokenFields:
    properties:
      nameOnCard:
        description: This is a default description.
        type: get
      postalCode:
        description: This is a default description.
        type: get
      cardType:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      amountOnCard:
        description: This is a default description.
        type: get
      token:
        description: This is a default description.
        type: get
  mobileError:
    properties:
      errorCode:
        description: This is a default description.
        type: get
      errorInfo:
        description: This is a default description.
        type: get
      diagnosticId:
        description: This is a default description.
        type: get
      diagnosticFullText:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
  jsonSurcharge:
    properties:
      amount:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  jsonPriceAdjustment:
    properties:
      type:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      formattedAmount:
        description: This is a default description.
        type: get
  jsonNightlyRates:
    properties:
      promo:
        description: This is a default description.
        type: get
      baseRate:
        description: This is a default description.
        type: get
      rate:
        description: This is a default description.
        type: get
  jsonMandatoryFees:
    properties:
      feeName:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
  jsonBaseRateInfo:
    properties:
      maxNightlyRate:
        description: This is a default description.
        type: get
      averageRate:
        description: This is a default description.
        type: get
      taxStatusType:
        description: This is a default description.
        type: get
      surchargeTotal:
        description: This is a default description.
        type: get
      surchargeTotalForEntireStay:
        description: This is a default description.
        type: get
      averageBaseRate:
        description: This is a default description.
        type: get
      nightlyRateTotal:
        description: This is a default description.
        type: get
      discountPercent:
        description: This is a default description.
        type: get
      total:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
  apiNewTripJson:
    properties:
      itineraryNumber:
        description: This is a default description.
        type: get
      travelRecordLocator:
        description: This is a default description.
        type: get
      tripId:
        description: This is a default description.
        type: get
  flightAggregatedResponse:
    properties:
      responseType:
        description: This is a default description.
        type: get
      flightsDetailResponse:
        description: This is a default description.
        type: get
  jsonAssociatedTraveler:
    properties:
      tuid:
        description: This is a default description.
        type: get
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
  jsonPhone:
    properties:
      number:
        description: This is a default description.
        type: get
      areaCode:
        description: This is a default description.
        type: get
      category:
        description: This is a default description.
        type: get
      countryCode:
        description: This is a default description.
        type: get
      extensionNumber:
        description: This is a default description.
        type: get
  jsonAddress:
    properties:
      firstAddressLine:
        description: This is a default description.
        type: get
      secondAddressLine:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      province:
        description: This is a default description.
        type: get
      postalCode:
        description: This is a default description.
        type: get
      countryAlpha3Code:
        description: This is a default description.
        type: get
      categoryCode:
        description: This is a default description.
        type: get
  loyaltyMembershipInfo:
    properties:
      loyaltyMembershipNumber:
        description: This is a default description.
        type: get
      loyaltyMembershipActive:
        description: This is a default description.
        type: get
      loyaltyPointsAvailable:
        description: This is a default description.
        type: get
      loyaltyPointsPending:
        description: This is a default description.
        type: get
      loyaltyAmountAvailable:
        description: This is a default description.
        type: get
      bookingCurrency:
        description: This is a default description.
        type: get
      isAllowedToShopWithPoints:
        description: This is a default description.
        type: get
      pointsRemainingTillPurchase:
        description: This is a default description.
        type: get
      loyaltyMembershipName:
        description: This is a default description.
        type: get
      membershipTierName:
        description: This is a default description.
        type: get
  jsonUserCreditCardInformation:
    properties:
      description:
        description: This is a default description.
        type: get
      paymentsInstrumentsId:
        description: This is a default description.
        type: get
      creditCardType:
        description: This is a default description.
        type: get
      nameOnCard:
        description: This is a default description.
        type: get
      expired:
        description: This is a default description.
        type: get
      expirationDate:
        description: This is a default description.
        type: get
  jsonFrequentGuestMembership:
    properties:
      frequentGuestMembershipID:
        description: This is a default description.
        type: get
      frequentGuestMembershipCode:
        description: This is a default description.
        type: get
      hotelMembershipNumber:
        description: This is a default description.
        type: get
  jsonPassport:
    properties:
      countryCode:
        description: This is a default description.
        type: get
  jsonTsaDetails:
    properties:
      gender:
        description: This is a default description.
        type: get
      dateOfBirth:
        description: This is a default description.
        type: get
      redressNumber:
        description: This is a default description.
        type: get
  jsonFrequentFlyerMembership:
    properties:
      membershipNumber:
        description: This is a default description.
        type: get
      planCode:
        description: This is a default description.
        type: get
      airlineCode:
        description: This is a default description.
        type: get
  jsonEmergencyContact:
    properties:
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
  jsonHotel:
    properties:
      sortIndex:
        description: This is a default description.
        type: get
      hotelId:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      localizedName:
        description: This is a default description.
        type: get
      nonLocalizedName:
        description: This is a default description.
        type: get
      address:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      stateProvinceCode:
        description: This is a default description.
        type: get
      countryCode:
        description: This is a default description.
        type: get
      postalCode:
        description: This is a default description.
        type: get
  jsonOpaqueNeighborhood:
    properties:
      opaqueHoodId:
        description: This is a default description.
        type: get
      opaqueHoodName:
        description: This is a default description.
        type: get
      opaqueHoodDescription:
        description: This is a default description.
        type: get
      cityName:
        description: This is a default description.
        type: get
      provinceName:
        description: This is a default description.
        type: get
      opaqueHoodShape:
        description: This is a default description.
        type: get
  jsonAmbiguousCityMatch:
    properties:
      regionId:
        description: This is a default description.
        type: get
      cityName:
        description: This is a default description.
        type: get
      cityUrl:
        description: This is a default description.
        type: get
  jsonOpaqueHotel:
    properties:
      sortIndex:
        description: This is a default description.
        type: get
      hotelName:
        description: This is a default description.
        type: get
      hotelStarRating:
        description: This is a default description.
        type: get
      opaqueHoodId:
        description: This is a default description.
        type: get
      opaqueSearchResultId:
        description: This is a default description.
        type: get
      productKey:
        description: This is a default description.
        type: get
      hotelAmenities:
        description: This is a default description.
        type: get
  flightSegmentJson:
    properties:
      departureTime:
        description: This is a default description.
        type: get
      departureTimeEpochSeconds:
        description: This is a default description.
        type: get
      departureTimeRaw:
        description: This is a default description.
        type: get
      departureTimeZoneOffsetSeconds:
        description: This is a default description.
        type: get
      arrivalTime:
        description: This is a default description.
        type: get
      arrivalTimeEpochSeconds:
        description: This is a default description.
        type: get
      arrivalTimeRaw:
        description: This is a default description.
        type: get
      arrivalTimeZoneOffsetSeconds:
        description: This is a default description.
        type: get
      arrivalAirportCode:
        description: This is a default description.
        type: get
      arrivalAirportLocation:
        description: This is a default description.
        type: get
  flightLegJson:
    properties:
      legId:
        description: This is a default description.
        type: get
      travelDuration:
        description: This is a default description.
        type: get
      fareBasisCode:
        description: This is a default description.
        type: get
      baggageFeesUrl:
        description: This is a default description.
        type: get
      segments:
        description: This is a default description.
        type: get
      isBasicEconomy:
        description: This is a default description.
        type: get
      basicEconomyTooltipInfo:
        description: This is a default description.
        type: get
      isRefundable:
        description: This is a default description.
        type: get
      isNonStop:
        description: This is a default description.
        type: get
      isEvolable:
        description: This is a default description.
        type: get
  postUrl:
    properties:
      requestPath:
        description: This is a default description.
        type: get
      formData:
        description: This is a default description.
        type: get
  baggageFeesSegmentInfo:
    properties:
      originapt:
        description: This is a default description.
        type: get
      bookingclass:
        description: This is a default description.
        type: get
      traveldate:
        description: This is a default description.
        type: get
      segmentnumber:
        description: This is a default description.
        type: get
      flightnumber:
        description: This is a default description.
        type: get
      farebasis:
        description: This is a default description.
        type: get
      destinationapt:
        description: This is a default description.
        type: get
      opcarrier:
        description: This is a default description.
        type: get
      cabinclass:
        description: This is a default description.
        type: get
      mktgcarrier:
        description: This is a default description.
        type: get
  tooltipInfoJson:
    properties:
      fareRulesTitle:
        description: This is a default description.
        type: get
      fareRules:
        description: This is a default description.
        type: get
  mobilePrice:
    properties:
      amount:
        description: This is a default description.
        type: get
      formattedPrice:
        description: This is a default description.
        type: get
      formattedWholePrice:
        description: This is a default description.
        type: get
  hotelPricing:
    properties: []
  pricePoints:
    properties:
      points:
        description: This is a default description.
        type: get
      pointsType:
        description: This is a default description.
        type: get
  passengerCategoryPrice:
    properties:
      passengerCategory:
        description: This is a default description.
        type: get
  flightSegmentAttributesJson:
    properties:
      bookingCode:
        description: This is a default description.
        type: get
      cabinCode:
        description: This is a default description.
        type: get
      isBasicEconomySegment:
        description: This is a default description.
        type: get
  flightOfferJson:
    properties:
      legIds:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      baseFare:
        description: This is a default description.
        type: get
      totalFare:
        description: This is a default description.
        type: get
      pricePerPassengerCategory:
        description: This is a default description.
        type: get
      numberOfTickets:
        description: This is a default description.
        type: get
      taxes:
        description: This is a default description.
        type: get
      fees:
        description: This is a default description.
        type: get
      showFees:
        description: This is a default description.
        type: get
      productKey:
        description: This is a default description.
        type: get
  searchCityJson:
    properties:
      code:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      province:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
      searchType:
        description: This is a default description.
        type: get
  airport:
    properties:
      airportCode:
        description: This is a default description.
        type: get
      regionId:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      country:
        description: This is a default description.
        type: get
  route:
    properties:
      origin:
        description: This is a default description.
        type: get
      destinations:
        description: This is a default description.
        type: get
  flightRulesJson:
    properties:
      isChangeAllowed:
        description: This is a default description.
        type: get
      isEnrouteChangeAllowed:
        description: This is a default description.
        type: get
      isEnrouteRefundAllowed:
        description: This is a default description.
        type: get
      isRefundable:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      changePenaltyAmount:
        description: This is a default description.
        type: get
      refundPenaltyAmount:
        description: This is a default description.
        type: get
      enrouteChangePenaltyAmount:
        description: This is a default description.
        type: get
      enrouteRefundAllowedAmount:
        description: This is a default description.
        type: get
      summaryText:
        description: This is a default description.
        type: get
  apiNewTrip:
    properties:
      itineraryNumber:
        description: This is a default description.
        type: get
      travelRecordLocator:
        description: This is a default description.
        type: get
      tripId:
        description: This is a default description.
        type: get
  flightDetailedRulesJson:
    properties:
      RuleToTextMap:
        description: This is a default description.
        type: get
      RuleToUrlMap:
        description: This is a default description.
        type: get
  apiPaymentOptionJson:
    properties:
      name:
        description: This is a default description.
        type: get
      fee:
        description: This is a default description.
        type: get
      feeCurrencyCode:
        description: This is a default description.
        type: get
      totalFarePriceWithFee:
        description: This is a default description.
        type: get
      formattedFee:
        description: This is a default description.
        type: get
  feeRange:
    properties: []
  pointsDetailJson:
    properties:
      programName:
        description: This is a default description.
        type: get
      rateId:
        description: This is a default description.
        type: get
      isAllowedToRedeem:
        description: This is a default description.
        type: get
  expediaRewardsForTripJson:
    properties:
      totalPointsToEarn:
        description: This is a default description.
        type: get
      isActiveRewardsMember:
        description: This is a default description.
        type: get
      rewardsMembershipTierName:
        description: This is a default description.
        type: get
  rewardsForTripJson:
    properties:
      programName:
        description: This is a default description.
        type: get
      totalPointsToEarn:
        description: This is a default description.
        type: get
      isActiveRewardsMember:
        description: This is a default description.
        type: get
      rewardsMembershipTierName:
        description: This is a default description.
        type: get
  addOn:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      termsUrl:
        description: This is a default description.
        type: get
      insuranceTypeId:
        description: This is a default description.
        type: get
      markupPercent:
        description: This is a default description.
        type: get
      displayPriceType:
        description: This is a default description.
        type: get
  frequentFlyerPlanDetails:
    properties:
      frequentFlyerPlanID:
        description: This is a default description.
        type: get
      frequentFlyerPlanCode:
        description: This is a default description.
        type: get
      airlineCode:
        description: This is a default description.
        type: get
      frequentFlyerPlanName:
        description: This is a default description.
        type: get
  frequentFlyerMembershipDetails:
    properties:
      frequentFlyerPlanID:
        description: This is a default description.
        type: get
      frequentFlyerPlanCode:
        description: This is a default description.
        type: get
      airlineCode:
        description: This is a default description.
        type: get
      frequentFlyerPlanName:
        description: This is a default description.
        type: get
      membershipNumber:
        description: This is a default description.
        type: get
  fareFamilyList:
    properties:
      fareFamilyName:
        description: This is a default description.
        type: get
      fareFamilyCode:
        description: This is a default description.
        type: get
      cabinClass:
        description: This is a default description.
        type: get
      fareFamilyComponents:
        description: This is a default description.
        type: get
      deltaPositive:
        description: This is a default description.
        type: get
  componentMap:
    properties:
      amenityCode:
        description: This is a default description.
        type: get
      localisedAmenityName:
        description: This is a default description.
        type: get
  insurance:
    properties:
      name:
        description: This is a default description.
        type: get
      productId:
        description: This is a default description.
        type: get
      policyNumber:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      termsUrl:
        description: This is a default description.
        type: get
      displayPriceType:
        description: This is a default description.
        type: get
      availableInsuranceAddOns:
        description: This is a default description.
        type: get
  mobileCoupon:
    properties:
      name:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
      instanceId:
        description: This is a default description.
        type: get
  textSection:
    properties:
      name:
        description: This is a default description.
        type: get
      content:
        description: This is a default description.
        type: get
  frequentFlyerPlans:
    properties:
      enrolledFrequentFlyerPlans:
        description: This is a default description.
        type: get
      allFrequentFlyerPlans:
        description: This is a default description.
        type: get
  region:
    properties:
      id:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
  jsonPhoto:
    properties:
      url:
        description: This is a default description.
        type: get
      thumbnailUrl:
        description: This is a default description.
        type: get
      featured:
        description: This is a default description.
        type: get
      displayText:
        description: This is a default description.
        type: get
  jsonBedType:
    properties:
      id:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
  jsonAvailabilityCancelPolicyInfo:
    properties:
      versionID:
        description: This is a default description.
        type: get
      cancelTime:
        description: This is a default description.
        type: get
      startWindowHours:
        description: This is a default description.
        type: get
      nightCount:
        description: This is a default description.
        type: get
      percent:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      timeZoneDescription:
        description: This is a default description.
        type: get
  jsonHotelRateInfo:
    properties:
      priceBreakdown:
        description: This is a default description.
        type: get
      promo:
        description: This is a default description.
        type: get
      rateChange:
        description: This is a default description.
        type: get
  mobileHotelSmokingPreference:
    properties:
      description:
        description: This is a default description.
        type: get
      locMsgId:
        description: This is a default description.
        type: get
  PromotionDetailsJson:
    properties:
      promoId:
        description: This is a default description.
        type: get
      minStay:
        description: This is a default description.
        type: get
      promoExpirationDate:
        description: This is a default description.
        type: get
      promoAdjustmentAmount:
        description: This is a default description.
        type: get
      promoAdjustmentType:
        description: This is a default description.
        type: get
      isPromoPartiallyApplied:
        description: This is a default description.
        type: get
  jsonHotelOffer:
    properties:
      productKey:
        description: This is a default description.
        type: get
      cancellationPolicy:
        description: This is a default description.
        type: get
      policy:
        description: This is a default description.
        type: get
      rateDescription:
        description: This is a default description.
        type: get
      roomTypeDescription:
        description: This is a default description.
        type: get
      roomLongDescription:
        description: This is a default description.
        type: get
      roomThumbnailUrl:
        description: This is a default description.
        type: get
      supplierType:
        description: This is a default description.
        type: get
      otherInformation:
        description: This is a default description.
        type: get
      rateChange:
        description: This is a default description.
        type: get
  lpasHotelOffer:
    properties:
      cancellationPolicy:
        description: This is a default description.
        type: get
      policy:
        description: This is a default description.
        type: get
      rateDescription:
        description: This is a default description.
        type: get
      roomTypeDescription:
        description: This is a default description.
        type: get
      roomLongDescription:
        description: This is a default description.
        type: get
      roomThumbnailUrl:
        description: This is a default description.
        type: get
      supplierType:
        description: This is a default description.
        type: get
      otherInformation:
        description: This is a default description.
        type: get
      rateChange:
        description: This is a default description.
        type: get
      nonRefundable:
        description: This is a default description.
        type: get
  jsonLoyaltyPointInfo:
    properties:
      pointValue:
        description: This is a default description.
        type: get
      pointType:
        description: This is a default description.
        type: get
  jsonLoyaltyPoints:
    properties:
      totalLoyaltyPoints:
        description: This is a default description.
        type: get
      loyaltyPointInfoList:
        description: This is a default description.
        type: get
  packageTripPricing:
    properties:
      taxesAndFeesIncluded:
        description: This is a default description.
        type: get
  jsonRoomOptions:
    properties:
      bedTypeName:
        description: This is a default description.
        type: get
      specialRequest:
        description: This is a default description.
        type: get
      hasExtraBedAdult:
        description: This is a default description.
        type: get
      hasExtraBedChild:
        description: This is a default description.
        type: get
      hasExtraBedInfant:
        description: This is a default description.
        type: get
      isSmokingPreferenceSelected:
        description: This is a default description.
        type: get
      isRoomOptionsAvailable:
        description: This is a default description.
        type: get
  jsonRoomOccupants:
    properties:
      adultCount:
        description: This is a default description.
        type: get
      childAndInfantAges:
        description: This is a default description.
        type: get
      bookingItemId:
        description: This is a default description.
        type: get
      orderLineGUID:
        description: This is a default description.
        type: get
      reservationStatus:
        description: This is a default description.
        type: get
      primaryOccupantName:
        description: This is a default description.
        type: get
  jsonHotelBooking:
    properties:
      error:
        description: This is a default description.
        type: get
      warnings:
        description: This is a default description.
        type: get
      cancellationPolicy:
        description: This is a default description.
        type: get
      nonLocalizedhotelName:
        description: This is a default description.
        type: get
      hotelName:
        description: This is a default description.
        type: get
      localizedHotelName:
        description: This is a default description.
        type: get
      hotelAddress:
        description: This is a default description.
        type: get
      hotelPostalCode:
        description: This is a default description.
        type: get
      hotelStateProvinceCode:
        description: This is a default description.
        type: get
      hotelCountryCode:
        description: This is a default description.
        type: get
  jsonPriceChange:
    properties: []
  checkout:
    properties: []
  mobileAirAttachQualifier:
    properties:
      airAttachQualified:
        description: This is a default description.
        type: get
      offerExpires:
        description: This is a default description.
        type: get
      offerExpiresTime:
        description: This is a default description.
        type: get
  tierInfo:
    properties:
      hotelNights:
        description: This is a default description.
        type: get
      tierName:
        description: This is a default description.
        type: get
  hotelCancelRules:
    properties:
      isRefundable:
        description: This is a default description.
        type: get
      isVenere:
        description: This is a default description.
        type: get
      isOpaque:
        description: This is a default description.
        type: get
      lowerFixedPenaltyPrice:
        description: This is a default description.
        type: get
      hasFixedPenaltyPrice:
        description: This is a default description.
        type: get
      isExpediaRate:
        description: This is a default description.
        type: get
      cancellationWindowDate:
        description: This is a default description.
        type: get
      cancellationWindowHours:
        description: This is a default description.
        type: get
      cancellationWindowDays:
        description: This is a default description.
        type: get
      cancellationTimeZoneName:
        description: This is a default description.
        type: get
  hotelCancelEnquiryRoomInfo:
    properties:
      ratePlanDescription:
        description: This is a default description.
        type: get
      adultCount:
        description: This is a default description.
        type: get
      numberOfNights:
        description: This is a default description.
        type: get
      orderLineGUID:
        description: This is a default description.
        type: get
  hotelCancelEnquiryInfo:
    properties:
      roomInfoList:
        description: This is a default description.
        type: get
  packageHotelOffer:
    properties:
      packageProductId:
        description: This is a default description.
        type: get
  packageTrip:
    properties:
      tripId:
        description: This is a default description.
        type: get
      itineraryNumber:
        description: This is a default description.
        type: get
      tealeafTransactionId:
        description: This is a default description.
        type: get
  vendor:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
      localPhoneNumber:
        description: This is a default description.
        type: get
      phoneNumber:
        description: This is a default description.
        type: get
      loyaltyProgram:
        description: This is a default description.
        type: get
  carLocation:
    properties:
      locationType:
        description: This is a default description.
        type: get
      locationDescription:
        description: This is a default description.
        type: get
      airportInstructions:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
      addressLine1:
        description: This is a default description.
        type: get
      addressLine2:
        description: This is a default description.
        type: get
      addressLine3:
        description: This is a default description.
        type: get
      addressLine4:
        description: This is a default description.
        type: get
      addressLine5:
        description: This is a default description.
        type: get
  rentalFare:
    properties:
      rateTerm:
        description: This is a default description.
        type: get
  carRentalMileageLimits:
    properties:
      freeMileage:
        description: This is a default description.
        type: get
      mileageUnit:
        description: This is a default description.
        type: get
  carRentalLimits:
    properties:
      minDuration:
        description: This is a default description.
        type: get
      maxDuration:
        description: This is a default description.
        type: get
      lastestReturnTime:
        description: This is a default description.
        type: get
  vendorWorkingHours:
    properties:
      pickUp:
        description: This is a default description.
        type: get
      dropOff:
        description: This is a default description.
        type: get
  vehicleInfo:
    properties:
      category:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      image:
        description: This is a default description.
        type: get
      fuel:
        description: This is a default description.
        type: get
      transmission:
        description: This is a default description.
        type: get
      drive:
        description: This is a default description.
        type: get
      hasAirConditioning:
        description: This is a default description.
        type: get
      makes:
        description: This is a default description.
        type: get
      minDoors:
        description: This is a default description.
        type: get
      maxDoors:
        description: This is a default description.
        type: get
  rentalOffer:
    properties:
      productKey:
        description: This is a default description.
        type: get
      creditCardRequiredToGuaranteeReservation:
        description: This is a default description.
        type: get
      isMerchant:
        description: This is a default description.
        type: get
  rentalFareBreakdownItem:
    properties:
      type:
        description: This is a default description.
        type: get
      includedInTotal:
        description: This is a default description.
        type: get
  detailedRentalFare:
    properties:
      rateTerm:
        description: This is a default description.
        type: get
      priceBreakdownOfTotalDueToday:
        description: This is a default description.
        type: get
      priceBreakdownOfTotalDueAtPickup:
        description: This is a default description.
        type: get
  mileageAllowance:
    properties:
      freeDistance:
        description: This is a default description.
        type: get
      distanceUnit:
        description: This is a default description.
        type: get
      extraDistanceInterval:
        description: This is a default description.
        type: get
      costPerExtraDistanceInterval:
        description: This is a default description.
        type: get
  rentalProduct:
    properties:
      pickupTime:
        description: This is a default description.
        type: get
      dropOffTime:
        description: This is a default description.
        type: get
      productKey:
        description: This is a default description.
        type: get
      creditCardRequiredToGuaranteeReservation:
        description: This is a default description.
        type: get
      minimumRental:
        description: This is a default description.
        type: get
      maximumRental:
        description: This is a default description.
        type: get
      rulesAndRestrictionsURL:
        description: This is a default description.
        type: get
  carMileageLimits:
    properties:
      freeDistance:
        description: This is a default description.
        type: get
      distanceUnit:
        description: This is a default description.
        type: get
      distancePeriod:
        description: This is a default description.
        type: get
      extraDistanceInterval:
        description: This is a default description.
        type: get
      costPerExtraDistanceInterval:
        description: This is a default description.
        type: get
  loyaltyPointDomain:
    properties:
      m_pointValue:
        description: This is a default description.
        type: get
      m_pointType:
        description: This is a default description.
        type: get
      m_pointDescription:
        description: This is a default description.
        type: get
      m_status:
        description: This is a default description.
        type: get
  rewardsDomain:
    properties:
      totalPoints:
        description: This is a default description.
        type: get
      basePoints:
        description: This is a default description.
        type: get
      bonusPoints:
        description: This is a default description.
        type: get
      logoUrl:
        description: This is a default description.
        type: get
      viewStatementURL:
        description: This is a default description.
        type: get
  customerSupportDomain:
    properties:
      customerSupportURL:
        description: This is a default description.
        type: get
      customerSupportPhoneInfo:
        description: This is a default description.
        type: get
      customerSupportPhoneNumberDomestic:
        description: This is a default description.
        type: get
      customerSupportPhoneNumberDomesticAfterHours:
        description: This is a default description.
        type: get
      customerSupportPhoneNumberInternational:
        description: This is a default description.
        type: get
      customerSupportPhoneInfoForEmail:
        description: This is a default description.
        type: get
      termsAndConditionsURL:
        description: This is a default description.
        type: get
  addressDomain:
    properties:
      addressLine1:
        description: This is a default description.
        type: get
      addressLine2:
        description: This is a default description.
        type: get
      addressLine3:
        description: This is a default description.
        type: get
      addressLine4:
        description: This is a default description.
        type: get
      addressLine5:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      cityLocalized:
        description: This is a default description.
        type: get
      companyName:
        description: This is a default description.
        type: get
      countrySubdivisionCode:
        description: This is a default description.
        type: get
      postalCode:
        description: This is a default description.
        type: get
  labelAndValuePairDomain:
    properties:
      label:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  hotelPropertyInfoDomain:
    properties:
      name:
        description: This is a default description.
        type: get
      starRating:
        description: This is a default description.
        type: get
      photoThumbnailURL:
        description: This is a default description.
        type: get
      photoThumbnail500pixURL:
        description: This is a default description.
        type: get
      photoThumbnail1000pixURL:
        description: This is a default description.
        type: get
      localPhone:
        description: This is a default description.
        type: get
      tollFreePhone:
        description: This is a default description.
        type: get
      formattedPhoneNumbers:
        description: This is a default description.
        type: get
      checkInPolicies:
        description: This is a default description.
        type: get
      generalRules:
        description: This is a default description.
        type: get
  lodgingPriceDetailsPerDayDomain:
    properties:
      primaryCurrencyCode:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      amountFormatted:
        description: This is a default description.
        type: get
  lodgingPriceDetailsDomain:
    properties:
      comment:
        description: This is a default description.
        type: get
      primaryCurrencyCode:
        description: This is a default description.
        type: get
      base:
        description: This is a default description.
        type: get
      baseFormatted:
        description: This is a default description.
        type: get
      baseWithAdjustmentForDRRRateDiscount:
        description: This is a default description.
        type: get
      baseWithAdjustmentForDRRRateDiscountFormatted:
        description: This is a default description.
        type: get
      extraGuestCharges:
        description: This is a default description.
        type: get
      extraGuestChargesFormatted:
        description: This is a default description.
        type: get
      taxesAndFees:
        description: This is a default description.
        type: get
      taxesAndFeesFormatted:
        description: This is a default description.
        type: get
  lodgingRulesDomain:
    properties:
      cancelChangeWarning:
        description: This is a default description.
        type: get
      cancelChangeRulesIntroduction:
        description: This is a default description.
        type: get
      cancelChangeRules:
        description: This is a default description.
        type: get
      opaqueRules:
        description: This is a default description.
        type: get
      opaquePolicies:
        description: This is a default description.
        type: get
      lateArrivalInstructions:
        description: This is a default description.
        type: get
      loyaltyPointsDisclaimer:
        description: This is a default description.
        type: get
      quebecResidentsIndemnityFund:
        description: This is a default description.
        type: get
      currencyDisclaimer:
        description: This is a default description.
        type: get
      currencyConversionDisclaimer:
        description: This is a default description.
        type: get
  priceDomain:
    properties:
      amount:
        description: This is a default description.
        type: get
  couponDomain:
    properties:
      name:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
  currencyDomain:
    properties:
      currencyCode:
        description: This is a default description.
        type: get
      defaultFractionDigits:
        description: This is a default description.
        type: get
      numericCode:
        description: This is a default description.
        type: get
      instances:
        description: This is a default description.
        type: get
      available:
        description: This is a default description.
        type: get
  guestDomain:
    properties:
      firstName:
        description: This is a default description.
        type: get
      fullName:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      primaryPhone:
        description: This is a default description.
        type: get
      phone:
        description: This is a default description.
        type: get
      frequentGuestPlanName:
        description: This is a default description.
        type: get
      frequentGuestMembershipCode:
        description: This is a default description.
        type: get
      frequentFlyerPlanName:
        description: This is a default description.
        type: get
      frequentFlyerMembershipCode:
        description: This is a default description.
        type: get
  occupancyInfoDomain:
    properties:
      adultCount:
        description: This is a default description.
        type: get
      childCount:
        description: This is a default description.
        type: get
      infantCount:
        description: This is a default description.
        type: get
      childAndInfantAges:
        description: This is a default description.
        type: get
  roomOptionsDomain:
    properties:
      bedTypeName:
        description: This is a default description.
        type: get
      defaultBedTypeName:
        description: This is a default description.
        type: get
      smokingPreference:
        description: This is a default description.
        type: get
      specialRequest:
        description: This is a default description.
        type: get
      accessibilityOptions:
        description: This is a default description.
        type: get
      hasExtraBedAdult:
        description: This is a default description.
        type: get
      hasExtraBedChild:
        description: This is a default description.
        type: get
      hasExtraBedInfant:
        description: This is a default description.
        type: get
      isSmokingPreferenceSelected:
        description: This is a default description.
        type: get
      isRoomOptionsAvailable:
        description: This is a default description.
        type: get
  bedDomain:
    properties:
      id:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      selected:
        description: This is a default description.
        type: get
  accessibilityDomain:
    properties:
      id:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      selected:
        description: This is a default description.
        type: get
  availableRoomOptionsDomain:
    properties:
      bedTypes:
        description: This is a default description.
        type: get
      accessibilityOptions:
        description: This is a default description.
        type: get
      isSmokingRoomAvailable:
        description: This is a default description.
        type: get
      isNonSmokingRoomAvailable:
        description: This is a default description.
        type: get
  roomPreferencesDomain:
    properties: []
  cancelRefundDetailsDomain:
    properties:
      condition:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      penaltyAmount:
        description: This is a default description.
        type: get
      penaltyAmountFormatted:
        description: This is a default description.
        type: get
      refundAmount:
        description: This is a default description.
        type: get
      refundAmountFormatted:
        description: This is a default description.
        type: get
  roomDomain:
    properties:
      uniqueID:
        description: This is a default description.
        type: get
      roomRatePlanDescription:
        description: This is a default description.
        type: get
      roomTypeCode:
        description: This is a default description.
        type: get
      ratePlanCode:
        description: This is a default description.
        type: get
      bookingStatus:
        description: This is a default description.
        type: get
      bookingStatusEnum:
        description: This is a default description.
        type: get
      hotelConfirmationNumber:
        description: This is a default description.
        type: get
      hotelCancellationId:
        description: This is a default description.
        type: get
      drrRateDiscountDescription:
        description: This is a default description.
        type: get
      orderLineNumber:
        description: This is a default description.
        type: get
  paymentAndCreditFeesDomain:
    properties:
      paymentsHotelFeesAndDepositsDisclaimer:
        description: This is a default description.
        type: get
      paymentsDepositRequired:
        description: This is a default description.
        type: get
      paymentsCreditsGDSHotelAnyRoomCancelled:
        description: This is a default description.
        type: get
      paymentsCreditsDAHotelAnyRoomCancelled:
        description: This is a default description.
        type: get
      noFeesStaticText:
        description: This is a default description.
        type: get
      isDirectAgency:
        description: This is a default description.
        type: get
      isGDS:
        description: This is a default description.
        type: get
      isFullyCancelled:
        description: This is a default description.
        type: get
      isAnyRoomCancelled:
        description: This is a default description.
        type: get
      isDepositRequired:
        description: This is a default description.
        type: get
  hotelDomain:
    properties:
      uniqueID:
        description: This is a default description.
        type: get
      hotelId:
        description: This is a default description.
        type: get
      checkInDate:
        description: This is a default description.
        type: get
      checkOutDate:
        description: This is a default description.
        type: get
      checkInDateLocalized:
        description: This is a default description.
        type: get
      checkOutDateLocalized:
        description: This is a default description.
        type: get
      numberOfNights:
        description: This is a default description.
        type: get
      bookingStatus:
        description: This is a default description.
        type: get
      bookingStatusText:
        description: This is a default description.
        type: get
      bookingStatusMessage:
        description: This is a default description.
        type: get
  confirmationNumberDomain:
    properties:
      airlineName:
        description: This is a default description.
        type: get
      number:
        description: This is a default description.
        type: get
  fareDomain:
    properties:
      airlineCardFee:
        description: This is a default description.
        type: get
      airlineCardFeeFormatted:
        description: This is a default description.
        type: get
      expediaServiceFee:
        description: This is a default description.
        type: get
      expediaServiceFeeFormatted:
        description: This is a default description.
        type: get
      insurance:
        description: This is a default description.
        type: get
      insuranceFormatted:
        description: This is a default description.
        type: get
      subTotal:
        description: This is a default description.
        type: get
      subTotalFormatted:
        description: This is a default description.
        type: get
      couponDiscount:
        description: This is a default description.
        type: get
      couponDiscountFormatted:
        description: This is a default description.
        type: get
  feeComponentDomain:
    properties:
      localizedName:
        description: This is a default description.
        type: get
      amount:
        description: This is a default description.
        type: get
      amountFormatted:
        description: This is a default description.
        type: get
  weightDomain:
    properties:
      value:
        description: This is a default description.
        type: get
      unit:
        description: This is a default description.
        type: get
  ancillaryFeeComponentDomain:
    properties:
      quantity:
        description: This is a default description.
        type: get
      addToTotal:
        description: This is a default description.
        type: get
      listOfLegsAncillaryAppliedTo:
        description: This is a default description.
        type: get
  phoneDomain:
    properties:
      countryCode:
        description: This is a default description.
        type: get
      phone:
        description: This is a default description.
        type: get
  seatDomain:
    properties:
      assigned:
        description: This is a default description.
        type: get
      requested:
        description: This is a default description.
        type: get
      seatPreference:
        description: This is a default description.
        type: get
      seatPreferenceLocalized:
        description: This is a default description.
        type: get
      ticketingStatus:
        description: This is a default description.
        type: get
      smokingAllowed:
        description: This is a default description.
        type: get
      legIndex:
        description: This is a default description.
        type: get
      segmentIndex:
        description: This is a default description.
        type: get
  frequentFlyerPlanDomain:
    properties:
      airlineCode:
        description: This is a default description.
        type: get
      programCode:
        description: This is a default description.
        type: get
      programName:
        description: This is a default description.
        type: get
      membershipNumber:
        description: This is a default description.
        type: get
  passengerFlightDomain:
    properties:
      typeCode:
        description: This is a default description.
        type: get
      typeLocalized:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
      fullName:
        description: This is a default description.
        type: get
      age:
        description: This is a default description.
        type: get
      gender:
        description: This is a default description.
        type: get
      TSARedressNumber:
        description: This is a default description.
        type: get
  farePerPassengerDomain:
    properties:
      passengerIndex:
        description: This is a default description.
        type: get
      passengerTypeCode:
        description: This is a default description.
        type: get
      passengerTypeCodeLocalized:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      base:
        description: This is a default description.
        type: get
      baseFormatted:
        description: This is a default description.
        type: get
      taxes:
        description: This is a default description.
        type: get
      taxesFormatted:
        description: This is a default description.
        type: get
      fees:
        description: This is a default description.
        type: get
      ancillaryFees:
        description: This is a default description.
        type: get
  locationDomain:
    properties:
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      longName:
        description: This is a default description.
        type: get
      airportCode:
        description: This is a default description.
        type: get
      airportMetroCode:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      countryCode:
        description: This is a default description.
        type: get
      countrySubdivisionCode:
        description: This is a default description.
        type: get
      fullAddress:
        description: This is a default description.
        type: get
  flightDelaysDomain:
    properties:
      departureGateDelay:
        description: This is a default description.
        type: get
      arrivalGateDelay:
        description: This is a default description.
        type: get
  segmentDomain:
    properties:
      transportationType:
        description: This is a default description.
        type: get
      departureType:
        description: This is a default description.
        type: get
      arrivalType:
        description: This is a default description.
        type: get
      departureTerminal:
        description: This is a default description.
        type: get
      departureGate:
        description: This is a default description.
        type: get
      arrivalTerminal:
        description: This is a default description.
        type: get
      arrivalGate:
        description: This is a default description.
        type: get
      airlineCode:
        description: This is a default description.
        type: get
      externalAirlineCode:
        description: This is a default description.
        type: get
      airlineName:
        description: This is a default description.
        type: get
  legDomain:
    properties:
      type:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      numberOfStops:
        description: This is a default description.
        type: get
      airlineLogoURL:
        description: This is a default description.
        type: get
      segments:
        description: This is a default description.
        type: get
      sharableFlightLegURL:
        description: This is a default description.
        type: get
      duration:
        description: This is a default description.
        type: get
      segmentChangeMessage:
        description: This is a default description.
        type: get
  textUrlTripleDomain:
    properties:
      text:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
      textAndURL:
        description: This is a default description.
        type: get
      apiURL:
        description: This is a default description.
        type: get
  rulesDomain:
    properties:
      bookingFeeText:
        description: This is a default description.
        type: get
      cancellationFeeLegalText:
        description: This is a default description.
        type: get
      bookingFeeLegalText:
        description: This is a default description.
        type: get
      faresNotGuaranteedText:
        description: This is a default description.
        type: get
      cancelChangeIntroductionText:
        description: This is a default description.
        type: get
      feeChangeRefundIntroductionText:
        description: This is a default description.
        type: get
      refundabilityText:
        description: This is a default description.
        type: get
      changePenaltyText:
        description: This is a default description.
        type: get
      bargainFairUpgradesText:
        description: This is a default description.
        type: get
      bargainFareStandbyText:
        description: This is a default description.
        type: get
  flightDomain:
    properties:
      uniqueID:
        description: This is a default description.
        type: get
      bookingStatus:
        description: This is a default description.
        type: get
      bookingStatusText:
        description: This is a default description.
        type: get
      bookingStatusMessage:
        description: This is a default description.
        type: get
      ticketingStatus:
        description: This is a default description.
        type: get
      orderNumber:
        description: This is a default description.
        type: get
      webCancelPathURL:
        description: This is a default description.
        type: get
      updateFrequentFlyerPathURL:
        description: This is a default description.
        type: get
      orderLineNumber:
        description: This is a default description.
        type: get
      expediaBookingId:
        description: This is a default description.
        type: get
  carTravelerDomain:
    properties:
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
  carLocationDomain:
    properties:
      locationType:
        description: This is a default description.
        type: get
      locationDescription:
        description: This is a default description.
        type: get
      airportInstructions:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
      addressLine1:
        description: This is a default description.
        type: get
      addressLine2:
        description: This is a default description.
        type: get
      addressLine3:
        description: This is a default description.
        type: get
      addressLine4:
        description: This is a default description.
        type: get
      addressLine5:
        description: This is a default description.
        type: get
  carOpenHoursDomain:
    properties: []
  carVendorDomain:
    properties:
      longName:
        description: This is a default description.
        type: get
      code:
        description: This is a default description.
        type: get
      shortName:
        description: This is a default description.
        type: get
      logoURL:
        description: This is a default description.
        type: get
      phoneNumber:
        description: This is a default description.
        type: get
      localPhoneNumber:
        description: This is a default description.
        type: get
  carDomainRulesDomain:
    properties:
      ruleType:
        description: This is a default description.
        type: get
      ruleName:
        description: This is a default description.
        type: get
  rulesAndRestrictions:
    properties:
      category:
        description: This is a default description.
        type: get
      text:
        description: This is a default description.
        type: get
  carTypeAttributesDomain:
    properties:
      vehicleTypeLocalized:
        description: This is a default description.
        type: get
      fuelType:
        description: This is a default description.
        type: get
      fuelTypeLocalized:
        description: This is a default description.
        type: get
      airConditioningType:
        description: This is a default description.
        type: get
      airConditioningTypeLocalized:
        description: This is a default description.
        type: get
      transmissionType:
        description: This is a default description.
        type: get
      transmissionTypeLocalized:
        description: This is a default description.
        type: get
      wheelDriveType:
        description: This is a default description.
        type: get
      wheelDriveTypeLocalized:
        description: This is a default description.
        type: get
  travelerContactInformation:
    properties:
      email:
        description: This is a default description.
        type: get
      phoneNumber:
        description: This is a default description.
        type: get
  carDomain:
    properties:
      uniqueID:
        description: This is a default description.
        type: get
      bookingStatus:
        description: This is a default description.
        type: get
      bookingStatusText:
        description: This is a default description.
        type: get
      bookingStatusMessage:
        description: This is a default description.
        type: get
      orderNumber:
        description: This is a default description.
        type: get
      orderLineNumber:
        description: This is a default description.
        type: get
      paymentModel:
        description: This is a default description.
        type: get
      reservationGuaranteePolicy:
        description: This is a default description.
        type: get
      confirmationNumber:
        description: This is a default description.
        type: get
      webCancelPathURL:
        description: This is a default description.
        type: get
  vendorLocationDomain:
    properties:
      name1:
        description: This is a default description.
        type: get
      name2:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
  activityTravelerFieldsDomain:
    properties:
      isRedeemer:
        description: This is a default description.
        type: get
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
      fullName:
        description: This is a default description.
        type: get
      age:
        description: This is a default description.
        type: get
      gender:
        description: This is a default description.
        type: get
      nationalityCountry:
        description: This is a default description.
        type: get
  phoneNumberDomain:
    properties:
      formatted:
        description: This is a default description.
        type: get
      costText:
        description: This is a default description.
        type: get
      useText:
        description: This is a default description.
        type: get
  hoursOfOperationDomain:
    properties:
      day:
        description: This is a default description.
        type: get
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
  vendorCustomerServiceOfficeDomain:
    properties:
      name:
        description: This is a default description.
        type: get
      emailAddress:
        description: This is a default description.
        type: get
      phoneCountryCode:
        description: This is a default description.
        type: get
      phoneNumber:
        description: This is a default description.
        type: get
      phoneNumbers:
        description: This is a default description.
        type: get
      hoursOfOperationText:
        description: This is a default description.
        type: get
      hoursOfOperation:
        description: This is a default description.
        type: get
  termsAndConditionsDomain:
    properties:
      instructions:
        description: This is a default description.
        type: get
      knowBeforeYouGo:
        description: This is a default description.
        type: get
      howToRedeem:
        description: This is a default description.
        type: get
      terms:
        description: This is a default description.
        type: get
      cancellationAddendum:
        description: This is a default description.
        type: get
      generalDisclaimer:
        description: This is a default description.
        type: get
      quebecResidentsIndemnityFund:
        description: This is a default description.
        type: get
  activityVoucherDomain:
    properties:
      id:
        description: This is a default description.
        type: get
      barcodeNumber:
        description: This is a default description.
        type: get
      securityCode:
        description: This is a default description.
        type: get
      barcodeImageURL:
        description: This is a default description.
        type: get
      validForRedemerTypeLocalized:
        description: This is a default description.
        type: get
      validForRedemerTypeEnglish:
        description: This is a default description.
        type: get
      supplierReferenceCode:
        description: This is a default description.
        type: get
  pricePerPassengerDomain:
    properties:
      keyForCategory:
        description: This is a default description.
        type: get
      numberOfPassengers:
        description: This is a default description.
        type: get
  localisePriceAndPassengerCountDomain:
    properties:
      localisedPassengerTypeAndCount:
        description: This is a default description.
        type: get
      localisedPrice:
        description: This is a default description.
        type: get
  activityFareDomain:
    properties:
      pricePerCategory:
        description: This is a default description.
        type: get
      localisedPriceAndPassengerCount:
        description: This is a default description.
        type: get
  activityDomain:
    properties:
      uniqueID:
        description: This is a default description.
        type: get
      bookingStatus:
        description: This is a default description.
        type: get
      bookingStatusText:
        description: This is a default description.
        type: get
      bookingStatusMessage:
        description: This is a default description.
        type: get
      bookingId:
        description: This is a default description.
        type: get
      supplierReferenceNumber:
        description: This is a default description.
        type: get
      paymentModel:
        description: This is a default description.
        type: get
      activityCategoryID:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      activityTitle:
        description: This is a default description.
        type: get
  packagePriceDomain:
    properties:
      currency:
        description: This is a default description.
        type: get
      subTotal:
        description: This is a default description.
        type: get
      subTotalFormatted:
        description: This is a default description.
        type: get
      taxesAndFees:
        description: This is a default description.
        type: get
      taxesAndFeesFormatted:
        description: This is a default description.
        type: get
      insurance:
        description: This is a default description.
        type: get
      insuranceFormatted:
        description: This is a default description.
        type: get
      coupon:
        description: This is a default description.
        type: get
      couponFormatted:
        description: This is a default description.
        type: get
      obfee:
        description: This is a default description.
        type: get
  packageDomain:
    properties:
      uniqueID:
        description: This is a default description.
        type: get
      bookingStatus:
        description: This is a default description.
        type: get
      orderNumber:
        description: This is a default description.
        type: get
      orderLineNumber:
        description: This is a default description.
        type: get
      isChangeable:
        description: This is a default description.
        type: get
      isLegacy:
        description: This is a default description.
        type: get
      startDate:
        description: This is a default description.
        type: get
      endDate:
        description: This is a default description.
        type: get
  generalComponentDomain:
    properties:
      comment:
        description: This is a default description.
        type: get
      startDate:
        description: This is a default description.
        type: get
      endDate:
        description: This is a default description.
        type: get
      bookingStatus:
        description: This is a default description.
        type: get
  promotionDomain:
    properties:
      promotionId:
        description: This is a default description.
        type: get
      promotionCode:
        description: This is a default description.
        type: get
      campaignId:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      cruiseCardName:
        description: This is a default description.
        type: get
      fullDescription:
        description: This is a default description.
        type: get
      shortDescription:
        description: This is a default description.
        type: get
      termsAndConditions:
        description: This is a default description.
        type: get
      rank:
        description: This is a default description.
        type: get
  passengerCruiseDomain:
    properties:
      passengerNumber:
        description: This is a default description.
        type: get
      titleCode:
        description: This is a default description.
        type: get
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
      birthDate:
        description: This is a default description.
        type: get
      gender:
        description: This is a default description.
        type: get
      citizenship:
        description: This is a default description.
        type: get
  pricingSummaryDomain:
    properties:
      baseAmount:
        description: This is a default description.
        type: get
      taxesAndFees:
        description: This is a default description.
        type: get
      totalAmount:
        description: This is a default description.
        type: get
  paymentHistoryDomain:
    properties:
      amountPaid:
        description: This is a default description.
        type: get
      paymentPending:
        description: This is a default description.
        type: get
      totalAmountReceivedInd:
        description: This is a default description.
        type: get
      currency:
        description: This is a default description.
        type: get
      remainingBalance:
        description: This is a default description.
        type: get
      finalPaymentDueDate:
        description: This is a default description.
        type: get
  cruiseDomain:
    properties:
      bookingStatus:
        description: This is a default description.
        type: get
      invoiceNumber:
        description: This is a default description.
        type: get
      cruiseLineName:
        description: This is a default description.
        type: get
      shipName:
        description: This is a default description.
        type: get
      departureDate:
        description: This is a default description.
        type: get
      returnDate:
        description: This is a default description.
        type: get
      promotions:
        description: This is a default description.
        type: get
      cruiseLineBkgConfNumber:
        description: This is a default description.
        type: get
      adultPassengers:
        description: This is a default description.
        type: get
      childPassengers:
        description: This is a default description.
        type: get
  simplifiedTripDomain:
    properties:
      levelOfDetail:
        description: This is a default description.
        type: get
      tripId:
        description: This is a default description.
        type: get
      apiDetailsURL:
        description: This is a default description.
        type: get
      webDetailsURL:
        description: This is a default description.
        type: get
      tripNumber:
        description: This is a default description.
        type: get
      title:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      updateTripNameDescPathURL:
        description: This is a default description.
        type: get
      startDate:
        description: This is a default description.
        type: get
      endDate:
        description: This is a default description.
        type: get
  productTypeDomain:
    properties:
      m_productType:
        description: This is a default description.
        type: get
      travelocityType:
        description: This is a default description.
        type: get
  userErrorMessageDomain:
    properties:
      hasPageLevelError:
        description: This is a default description.
        type: get
      hasModuleLevelError:
        description: This is a default description.
        type: get
      pageLevelErrorMessage:
        description: This is a default description.
        type: get
      moduleLevelErrorMessage:
        description: This is a default description.
        type: get
      moduleName:
        description: This is a default description.
        type: get
      errorKey:
        description: This is a default description.
        type: get
  priceChangeResponseDomain:
    properties:
      priceIncreased:
        description: This is a default description.
        type: get
      previousTotal:
        description: This is a default description.
        type: get
      previousTotalFormatted:
        description: This is a default description.
        type: get
      newTotal:
        description: This is a default description.
        type: get
      newTotalFormatted:
        description: This is a default description.
        type: get
  changeErrorResponseDomain:
    properties:
      serviceErrorCode:
        description: This is a default description.
        type: get
  errorDomain:
    properties:
      errorCode:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      stackTrace:
        description: This is a default description.
        type: get
      errorCategory:
        description: This is a default description.
        type: get
      errorType:
        description: This is a default description.
        type: get
      fields:
        description: This is a default description.
        type: get
  flightSearchResponse:
    properties:
      legs:
        description: This is a default description.
        type: get
      offers:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      searchCities:
        description: This is a default description.
        type: get
      obFeesDetails:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      percentDelaysCancellationsURL:
        description: This is a default description.
        type: get
      hasSubPub:
        description: This is a default description.
        type: get
      mayChargePaymentFees:
        description: This is a default description.
        type: get
  flightCacheSearchResponse:
    properties:
      cachedResultsFound:
        description: This is a default description.
        type: get
      bookable:
        description: This is a default description.
        type: get
  cardFee:
    properties:
      tripId:
        description: This is a default description.
        type: get
  apiCreateTripResponse:
    properties:
      passengerCategories:
        description: This is a default description.
        type: get
      validFormsOfPayment:
        description: This is a default description.
        type: get
      rewardsPoints:
        description: This is a default description.
        type: get
      isCustomerTitleRequired:
        description: This is a default description.
        type: get
      availableInsuranceProducts:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      tealeafTransactionId:
        description: This is a default description.
        type: get
      guestUserPromoEmailOptInStatus:
        description: This is a default description.
        type: get
      createTripStatus:
        description: This is a default description.
        type: get
  fareFamilyInformation:
    properties:
      productKey:
        description: This is a default description.
        type: get
  flightDetailJsonResponse:
    properties:
      productKey:
        description: This is a default description.
        type: get
      flightRules:
        description: This is a default description.
        type: get
      priceChangeAmount:
        description: This is a default description.
        type: get
      fareBasisCodeDetails:
        description: This is a default description.
        type: get
      obFeeTotalAmount:
        description: This is a default description.
        type: get
      legs:
        description: This is a default description.
        type: get
      basicEconomyFareRules:
        description: This is a default description.
        type: get
  flightCreateTripForPartnerResponse:
    properties:
      productKey:
        description: This is a default description.
        type: get
      flightRules:
        description: This is a default description.
        type: get
      priceChangeAmount:
        description: This is a default description.
        type: get
      obFeeTotalAmount:
        description: This is a default description.
        type: get
      legs:
        description: This is a default description.
        type: get
  imageJsonResponse:
    properties:
      imageUrl:
        description: This is a default description.
        type: get
      cacheKey:
        description: This is a default description.
        type: get
  airportDropDownDataResponse:
    properties:
      airport:
        description: This is a default description.
        type: get
      routes:
        description: This is a default description.
        type: get
  passengerDetailsJson:
    properties:
      title:
        description: This is a default description.
        type: get
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
      phone:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      dateOfBirth:
        description: This is a default description.
        type: get
      gender:
        description: This is a default description.
        type: get
      redressNumber:
        description: This is a default description.
        type: get
      tsaPreCheckNumber:
        description: This is a default description.
        type: get
  apiCheckoutResponseFlightOkResponse:
    properties:
      orderId:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      totalCharges:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      debugTealeafInfo:
        description: This is a default description.
        type: get
  apiCheckoutResponseFlightPriceChangeResponse:
    properties:
      errors:
        description: This is a default description.
        type: get
  flightFareRuleResponseJson:
    properties:
      airFareRules:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
  FareRuleDetailsJson:
    properties:
      fareBasisCode:
        description: This is a default description.
        type: get
      passengerCategory:
        description: This is a default description.
        type: get
      origin:
        description: This is a default description.
        type: get
      destination:
        description: This is a default description.
        type: get
      carrierCode:
        description: This is a default description.
        type: get
      departureDate:
        description: This is a default description.
        type: get
      fareRules:
        description: This is a default description.
        type: get
  FareRuleJson:
    properties:
      category:
        description: This is a default description.
        type: get
      text:
        description: This is a default description.
        type: get
  jsonOpaqueHotelSearchResponse:
    properties:
      totalHotelCount:
        description: This is a default description.
        type: get
      opaqueHotelList:
        description: This is a default description.
        type: get
      opaqueNeighborhoodList:
        description: This is a default description.
        type: get
  hotelSearchResponse:
    properties:
      numberOfRoomsRequested:
        description: This is a default description.
        type: get
      filterUnavailableHotelsRequested:
        description: This is a default description.
        type: get
      totalHotelCount:
        description: This is a default description.
        type: get
      availableHotelCount:
        description: This is a default description.
        type: get
      searchRegionId:
        description: This is a default description.
        type: get
      hotelList:
        description: This is a default description.
        type: get
      allNeighborhoodsInSearchRegion:
        description: This is a default description.
        type: get
      filteredSearchMatchedNoHotels:
        description: This is a default description.
        type: get
      amenityFilterOptions:
        description: This is a default description.
        type: get
      starOptions:
        description: This is a default description.
        type: get
  hotelSearchV3Response:
    properties:
      numberOfRoomsRequested:
        description: This is a default description.
        type: get
      filterUnavailableHotelsRequested:
        description: This is a default description.
        type: get
      totalHotelCount:
        description: This is a default description.
        type: get
      availableHotelCount:
        description: This is a default description.
        type: get
      searchRegionId:
        description: This is a default description.
        type: get
      hotelList:
        description: This is a default description.
        type: get
      allNeighborhoodsInSearchRegion:
        description: This is a default description.
        type: get
      filteredSearchMatchedNoHotels:
        description: This is a default description.
        type: get
      amenityFilterOptions:
        description: This is a default description.
        type: get
      starOptions:
        description: This is a default description.
        type: get
  hotelAmbiguousResponse:
    properties:
      numberOfMatches:
        description: This is a default description.
        type: get
      cityList:
        description: This is a default description.
        type: get
  jsonGetOfferResponse:
    properties:
      hotelTagline:
        description: This is a default description.
        type: get
      checkInDate:
        description: This is a default description.
        type: get
      checkOutDate:
        description: This is a default description.
        type: get
      numberOfRoomsRequested:
        description: This is a default description.
        type: get
      numberOfNights:
        description: This is a default description.
        type: get
      tripAdvisorRating:
        description: This is a default description.
        type: get
      timeZoneUTCOffsetMinutes:
        description: This is a default description.
        type: get
      checkInInstructions:
        description: This is a default description.
        type: get
      shortDescription:
        description: This is a default description.
        type: get
      hotelRoomResponse:
        description: This is a default description.
        type: get
  lpasHotelOfferResponse:
    properties:
      hotelTagline:
        description: This is a default description.
        type: get
      checkInDate:
        description: This is a default description.
        type: get
      checkOutDate:
        description: This is a default description.
        type: get
      numberOfRoomsRequested:
        description: This is a default description.
        type: get
      numberOfNights:
        description: This is a default description.
        type: get
      tripAdvisorRating:
        description: This is a default description.
        type: get
      timeZoneUTCOffsetMinutes:
        description: This is a default description.
        type: get
      checkInInstructions:
        description: This is a default description.
        type: get
      shortDescription:
        description: This is a default description.
        type: get
      hotelRoomResponse:
        description: This is a default description.
        type: get
  jsonCreateTripResponse:
    properties:
      error:
        description: This is a default description.
        type: get
      warnings:
        description: This is a default description.
        type: get
      tripId:
        description: This is a default description.
        type: get
      userId:
        description: This is a default description.
        type: get
      userCoupons:
        description: This is a default description.
        type: get
      tealeafTransactionId:
        description: This is a default description.
        type: get
      validFormsOfPayment:
        description: This is a default description.
        type: get
      guestUserPromoEmailOptInStatus:
        description: This is a default description.
        type: get
      pointsDetails:
        description: This is a default description.
        type: get
  apiCheckoutResponseHotelResponse:
    properties:
      orderId:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      totalCharges:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      debugTealeafInfo:
        description: This is a default description.
        type: get
  apiFieldsResponse:
    properties:
      paymentFields:
        description: This is a default description.
        type: get
  hotelCancelEnquiryResponse:
    properties:
      errors:
        description: This is a default description.
        type: get
      amountPaid:
        description: This is a default description.
        type: get
      amountRefund:
        description: This is a default description.
        type: get
  hotelCancelEnquiryV2Response:
    properties:
      errors:
        description: This is a default description.
        type: get
      cancelEnquiryInfoList:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
  jsonGetProductResponse:
    properties:
      errors:
        description: This is a default description.
        type: get
      checkInDate:
        description: This is a default description.
        type: get
      checkOutDate:
        description: This is a default description.
        type: get
      checkInTime:
        description: This is a default description.
        type: get
      checkOutTime:
        description: This is a default description.
        type: get
      adultCount:
        description: This is a default description.
        type: get
      numberOfNights:
        description: This is a default description.
        type: get
      numberOfRooms:
        description: This is a default description.
        type: get
      hotelId:
        description: This is a default description.
        type: get
      hotelName:
        description: This is a default description.
        type: get
  jsonOpaqueGetProductResponse:
    properties:
      checkInDate:
        description: This is a default description.
        type: get
      checkOutDate:
        description: This is a default description.
        type: get
      adultCount:
        description: This is a default description.
        type: get
      numberOfNights:
        description: This is a default description.
        type: get
      numberOfRoomsRequested:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
  jsonHotelInformationResponse:
    properties:
      errors:
        description: This is a default description.
        type: get
      hotelId:
        description: This is a default description.
        type: get
      hotelName:
        description: This is a default description.
        type: get
      localizedHotelName:
        description: This is a default description.
        type: get
      nonLocalizedHotelName:
        description: This is a default description.
        type: get
      hotelAddress:
        description: This is a default description.
        type: get
      hotelCity:
        description: This is a default description.
        type: get
      hotelStateProvince:
        description: This is a default description.
        type: get
      hotelCountry:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
  hotelConfirmCancelResponse:
    properties:
      statusResponse:
        description: This is a default description.
        type: get
      amountRefund:
        description: This is a default description.
        type: get
  calculatePointsResponse:
    properties:
      programName:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
  jsonCancellationRoomResponse:
    properties: []
  jsonCancellationResponse:
    properties:
      guidToResponseMap:
        description: This is a default description.
        type: get
  apiCheckoutResponsePackageResponse:
    properties:
      orderId:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      totalCharges:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      debugTealeafInfo:
        description: This is a default description.
        type: get
  tripResponse:
    properties:
      apiVersion:
        description: This is a default description.
        type: get
      responseType:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      responseData:
        description: This is a default description.
        type: get
  tripTitleDescriptionUpdateResponse:
    properties:
      status:
        description: This is a default description.
        type: get
      errorMessage:
        description: This is a default description.
        type: get
  signInResponse:
    properties:
      tuid:
        description: This is a default description.
        type: get
      expUserId:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
      success:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      detailedStatus:
        description: This is a default description.
        type: get
      detailedStatusMsg:
        description: This is a default description.
        type: get
  createUserResponse:
    properties:
      tuid:
        description: This is a default description.
        type: get
      email:
        description: This is a default description.
        type: get
      firstName:
        description: This is a default description.
        type: get
      middleName:
        description: This is a default description.
        type: get
      lastName:
        description: This is a default description.
        type: get
  updateTravelerResponse:
    properties:
      succeeded:
        description: This is a default description.
        type: get
      tuid:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
  associateUserToTripResponse:
    properties:
      rewardsPoints:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
  carSearchResponse:
    properties:
      pickupTime:
        description: This is a default description.
        type: get
      dropOffTime:
        description: This is a default description.
        type: get
      offers:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
  carCreateTripResponse:
    properties:
      errors:
        description: This is a default description.
        type: get
      tripId:
        description: This is a default description.
        type: get
      itineraryNumber:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      validFormsOfPayment:
        description: This is a default description.
        type: get
  apiCheckoutResponseCarsResponse:
    properties:
      orderId:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      totalCharges:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
  carCancelResponse:
    properties:
      status:
        description: This is a default description.
        type: get
      tripId:
        description: This is a default description.
        type: get
      totalAmount:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
  apiErrorJsonResponse:
    properties:
      errors:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      debugTealeafInfo:
        description: This is a default description.
        type: get
  railsTripResponse:
    properties:
      errors:
        description: This is a default description.
        type: get
      tripId:
        description: This is a default description.
        type: get
      offerToken:
        description: This is a default description.
        type: get
      validFormsOfPayment:
        description: This is a default description.
        type: get
  lxCreateTripResponse:
    properties:
      errors:
        description: This is a default description.
        type: get
      tripId:
        description: This is a default description.
        type: get
      itineraryNumber:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
      validFormsOfPayment:
        description: This is a default description.
        type: get
  apiCheckoutResponseLxResponse:
    properties:
      orderId:
        description: This is a default description.
        type: get
      currencyCode:
        description: This is a default description.
        type: get
      totalCharges:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      activityId:
        description: This is a default description.
        type: get
x-collection-name: Expedia
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---