##Berlin Clock

Create a representation of the Berlin Clock for a given time (hh::mm:ss).

The Berlin Uhr (Clock) is a rather strange way to show the time.
On the top of the clock there is a yellow lamp that blinks on/off every two seconds.
The time is calculated by adding rectangular lamps.

The top two rows of lamps are red. These indicate the hours of a day. In the top row there are 4 red lamps.
Every lamp represents 5 hours. In the lower row of red lamps every lamp represents 1 hour.
So if two lamps of the first row and three of the second row are switched on that indicates 5+5+3=13h or 1 pm.

The two rows of lamps at the bottom count the minutes. The first of these rows has 11 lamps, the second 4.
In the first row every lamp represents 5 minutes.
In this first row the 3rd, 6th and 9th lamp are red and indicate the first quarter, half and last quarter of an hour.
The other lamps are yellow. In the last row with 4 lamps every lamp represents 1 minute.

The lamps are switched on from left to right.

Y = Yellow

R = Red

O = Off


![alt text](http://a1.mzstatic.com/us/r30/Purple4/v4/f8/27/8a/f8278af9-4aed-82fc-80a8-3eea0fd75320/screen480x480.jpeg)

1) Tee `convertToBerlinTime(String inputTime)` -metodi, joka saa normaaliajan ja palauttaa BerlinClock:n mukaisen ajan. Esimerkki:

```
String[] berlinTime = berlinClock.convertToBerlinTime("16:37:16");
String[] expected = new String[] {"Y", "RRRO", "ROOO", "YYRYYRYOOOO", "YYOO"};
```
