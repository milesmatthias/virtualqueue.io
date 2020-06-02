# virtualqueue.io
A virtual queue system that can be used for any physical location. [Inspiration](https://twitter.com/miles_matthias/status/1267553622168125441?s=20)

## Joining the line

1. A volunteer creates a line. That volunteer will be physically present at the line location the entire time.
2. Someone who wishes to join the line is physically at the line and asks the volunteer (in person) to join the line.
3. The volunteer creates a unique, one-time use code to give to the individual.
4. The individual texts a phone number with that code to join the line. They'll acknowledge an agreement + privacy policy, confirm the line physical location and line close time.

The individual is now "in line" and can go about their business without having to stand in the physical line.

## When it's your turn in line

1. The volunteer will monitor people completing the line.
2. When the volunteer wants the next-up individual(s) in the virtual line to return to the physical location for their turn, they will be able to notify the next X virtual line participants that it's their turn via a button/form.
3. The line participant will receive a SMS message notifying them their turn in the physical line is near and encourage them to return to the physical location. In addition, it will remind them of the physical line closing time (ex: 7pm).

The individuals notified will be considered "completed" at this point, and will no longer be in the virtual line.

## Line closure

X hours before the line is set to close, an SMS notification will be sent to all active, non-complete line members to notify them.

(X is a number of hours set by the volunteer when creating the line, defaulting to 2)

## Technical Architecture
* Rails?
* domain = virtualqueue.io (already purchased)
* Scalability & speed is a major concern (CDN, cloud-native, etc.)

## TODO

* [ ] agreement to be clear that service is not responsible for participants missing a line (ex: due to notification failure or volunteer failure)
* [ ] privacy policy
* [ ] non-profit organization creation
* [ ] hosting partner / sponsor
* [ ] sms partner / sponsor
* [ ] donations?
