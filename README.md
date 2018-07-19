# moment-date-range-picker
React date range selector component based on momentJS. 

This is a test library. Not for production.

### Install
```
npm install moment-date-range-picker --save
```

### Usage
```js
import MomentDateRange from "moment-date-range-picker/dist/MomentDateRange";
import { WeekDays } from "moment-date-range-picker/dist/utils";
require("moment-date-range-picker/dist/MomentDateRange.css");

 <MomentDateRange
                formatString="DD MMM YYYY"
                monthsCount={1}
                weekStartDay={WeekDays.Friday}
                to={moment().add(1, 'month')}
                firstDisplayedMonth={moment().add(1, 'month')}
                onRangeChange={(from, to) => console.info(from != null ? from.format("MM/DD/YY") : null, to != null ?          
                to.format("MM/DD/YY") : null)}
 />
```
