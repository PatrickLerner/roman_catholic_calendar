# Roman Catholic Calendar

## Feasts

Feasts are saved as json document with each feast in one file. The following keys are used in the format:

### `date`

The date format of the feast is either a fixed date, a date variable based on easter or the 'Feast of Christ the King', which has a special date calculation based on it's own.

If the date is fixed, date is a json object with the keys `month` and `day`.

If the date depends on easter, it is a json object with only the key `days_after_easter`.

If the event is the 'Feast of Christ the King', then the hash has only the `days_after_christ_king` key.

### `rank`

Rank determines the importance of observations of the feast. Possible values are:

`solemnity`, `feast`, `memorial` and `optional memorial`

### `color`

Color determines the liturgical color of the feast. Possible values are:

`white`, `red`, `black`, `green` and `violet` (violet is never used)

### `name`

Name is a json object that gives the name of the feast in different languages. The files here come with two languages: `de` (German) and `en` (English)
