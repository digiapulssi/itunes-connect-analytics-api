# itunes-connect-analytics-api
Docker container for iTunes Connect's App Analytics.

The code is forked from [itunes-connect-analytics-api by Mitsuki Ogasahara](https://github.com/yamitzky/itunes-connect-analytics-api) which uses library [iTunesConnectAnalytics by JanHalozan](https://github.com/JanHalozan/iTunesConnectAnalytics).

Usage example:

`docker run --rm  digiapulssi/itunes-connect-analytics-api --appleId [<appleId>] --password [<password>] --app [<applicationid>] --type "metrics" --time 5 --timetype years --measure '["installs","units"]'`

where:

* appleid = username
* password = password
* app = Integer found in My Apps -> App -> Apple ID.
* type = metrics
* time = Numeric value of years or days
* timetype = Type of time value, "years" or "days"
* measure = available values: installs, sessions, pageViews, activeDevices, crashes, payingUsers, units, sales, iap (in app purchases), impressions, impressionsUnique
