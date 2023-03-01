# FluttercountDownTime

//First Input Time from PickupDate Time Database
// Then parse the time to  DateTime
// Calculate The time Difference remainingTime


    getTimeDuration() {
    String tripTime = widget.upcomingTripDetails.pickupDateTime;

    DateTime dateTime = DateTime.parse(tripTime);

    remainingTime = dateTime.difference(DateTime.now());
    }
 // Then Install Flutter Timer Countdown Package
 // Set The Code Following Ways With Multiple  Conditions
