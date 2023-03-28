
#### You can format or get relavant date for the date specified.
    import relt from "reltjs"

### Usage

```// OPTIONS
const options = {
    date: 'March 30 2023 5:45 PM',
    timeZone: 'America/New_York'  // Just specify a valid timezone and time will be returned in it. :)
}
const reltDate1 = relt(options);

//console.log(reltDate1.relative())

// console.log(reltDate1.format("DD-MM-YYYY"))

// console.log(datreltDate1e1.format("DDDD, Do MMMM YYYY Z"))

// console.log(reltDate1.count(date1.date))
```
#### Available functions
```
format()

fullDate()

relative()

count()
```
#### reltDate has following properties

```
Relt {
  timeZone: 'Asia/Calcutta',
  locale: 'en-US',
  date: 2023-03-14T18:30:00.000Z,
  weekDayName: 'Wednesday',
  month: '03',
  day: '15',
  year: '2023',
  period: 'AM',
  timeZoneCode: 'GMT+5:30',
  hour: '12',
  minutes: '00',
  seconds: '00'
}
```

#### format()
```
reltDate.format('DD MM YYYY hh:mm:ss am D Mx Do Mo MMMM YYYY DDDD Z')

// Output: 01 03 2023 12:30:00 PM 1 M 1st 3rd March 2023 Wednesday GMT+5:30
```
#### relative()
```
reltDate.relative()

// Output: as -> Just now | Today | Yesterday | Tommorrow | March 5, 2023
```
#### fullDate()
```
reltDate.fullDate()

// Output: March 26, 2023
```

#### count()
You will get the difference between two dates reltDate.count(date2)
```
// Output: 8 hours 3 minutes
// Output: 1 Days 2 hours 3 minutes
```

###### The choice between using Moment or Relt depends on the specific needs of your project.

Moment is a widely used library with a lot of features for working with dates and times, including parsing, formatting, and manipulating them. It has a large community and a lot of resources available.

On the other hand, Relt is a smaller library with fewer features, but it has a simpler API and is easier to learn and use. It also has good support for time zones, which can be a challenging aspect of working with dates and times.

If you have a large project with complex date and time requirements, then Moment might be the better choice because of its wider range of features and more extensive documentation. However, if you have a smaller project or are looking for a simpler API, Relt might be a good option. Ultimately, the choice depends on the specific needs of your project and your own preferences.


## License

Relt.js is freely distributable under the following terms

Copyright (c) JS Foundation and other contributors

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.