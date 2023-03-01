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
 code{
  

         TimerCountdown(
                    format: remainingTime!.inMinutes != 30
                        ? CountDownTimerFormat.daysHoursMinutes
                        : CountDownTimerFormat.daysHoursMinutesSeconds,
                    endTime: DateTime.now().add(remainingTime!),
                    timeTextStyle: remainingTime!.inDays == 0
                        ? const TextStyle(
                            color: ThemeStyles.redColor,
                            fontWeight: FontWeight.bold,
                          )
                        : const TextStyle(
                            color: ThemeStyles.blackColor,
                            fontWeight: FontWeight.bold,
                          ),
                    descriptionTextStyle: remainingTime!.inDays == 0
                        ? const TextStyle(
                            color: ThemeStyles.redColor,
                            fontWeight: FontWeight.bold,
                          )
                        : const TextStyle(
                            color: ThemeStyles.blackColor,
                            fontWeight: FontWeight.bold,
                          ),
                  )

