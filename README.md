# CoWin-solt-availability

https://cdn-api.co-vin.in/api/v2/admin/location/states

Use above link to get state_id of required state. After getting state_id replace in below link ending.

https://cdn-api.co-vin.in/api/v2/admin/location/districts/state_id

example, for telangana https://cdn-api.co-vin.in/api/v2/admin/location/districts/32

From this link get required district_ids in which you want to search for vaccine availability and substitute in "dids" array in function func() and execute the cells.

This code searches for availability of vaccine for 15 days including the current day. To change no.of days, change value of variable "numdays".

While loop is used to execute function every minute which checks for availability of vaccince in selected districts.

If vaccine is availabe then code prints the hospital, vaccine details and plays ringtone for notifying user.
