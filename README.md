# date_diiference-_calculator




# python

from datetime import datetime
from dateutil.relativedelta import relativedelta

# Define the two dates
date1 = datetime.strptime("2001-08-02", "%Y-%m-%d")
date2 = datetime.strptime("2004-1-26", "%Y-%m-%d")

# Calculate the difference
difference = relativedelta(date2, date1)

# Print result
print(f"{difference.years} years, {difference.months} months, and {difference.days} days")





# javascript

// Import Luxon (if using Node.js)
// const { DateTime } = require("luxon");

// Define the two dates
const date1 = luxon.DateTime.fromFormat("2001-08-02", "yyyy-MM-dd");
const date2 = luxon.DateTime.fromFormat("2004-01-26", "yyyy-MM-dd");

// Calculate the difference
const diff = date2.diff(date1, ["years", "months", "days"]).toObject();

// Print result
console.log(`${Math.floor(diff.years)} years, ${Math.floor(diff.months)} months, and ${Math.floor(diff.days)} days`);
