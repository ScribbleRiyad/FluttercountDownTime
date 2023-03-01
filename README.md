# FluttercountDownTime
 getTimeDuration() {
    String tripTime = widget.upcomingTripDetails.pickupDateTime;

    DateTime dateTime = DateTime.parse(tripTime);

    remainingTime = dateTime.difference(DateTime.now());
  }
