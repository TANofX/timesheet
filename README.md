# Licensing

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).


# Changing settings

There are some settings which can be changed to adapt this for your team.
These can be found in app/helpers/application_helper.rb

### Timezone
> <dl>
> 	<dt>Description</dt>
> 	<dd>
> 		The time zone associated with the times. It will determine what times show up, when the end of the day is, etc.
> 	</dd>
> 	<dt>Method</dt>
> 	<dd>
> 		self.TimeZone
> 	</dd>
> 	<dt>Default</dt>
> 	<dd>
> 		Eastern Standard Time
> 	</dd>
> 	<dt>Modification</dt>
> 	<dd>
> 		Change the string to one of the approved rails timezones. 
> 			* To get the timezones, you can run the command rake time:zones:all (computer must have RoR installed)
>   	  	* More info on getting timezone list: http://codedecoder.wordpress.com/2013/09/09/timezone-in-rails/
>   	  	* Timezones are also listed below
> 	</dd>
> </dl>

### Start of Year
> <dl>
> 	<dt>Description</dt>
> 	<dd>
> 		This is when the 'year' begins. Views of weeks start with the first day in the month
> 	</dd>
> 	<dt>Method</dt>
> 	<dd>
> 		self.getStartMonth
> 	</dd>
> 	<dt>Default</dt>
> 	<dd>
> 		1st of July
> 	</dd>
> 	<dt>Modification</dt>
> 	<dd>
> 		Change the 7 (July) to the integer corresponding to the month you want to begin
> 	</dd>
> </dl>

		
### Last Out
> <dl>
> 	<dt>Description</dt>
> 	<dd>
> 		The last possible time to sign out for the day. If a record isn't signed out by then, only 1 minute is credited for the day.
> 	</dd>
> 	<dt>Method</dt>
> 	<dd>
> 		self.today
> 	</dd>
> 	<dt>Default</dt>
> 	<dd>
> 		1 am
> 	</dd>
> 	<dt>Modification</dt>
> 	<dd>
> 		Change the 1 in the partial line below to correspond with the number of hours after midnight to cut off
> ```
> 	Time.now.in_time_zone  ...  + 1.hours
> ```
> 	</dd>
> </dl>
	
### Build Season Hours Required
> <dl>
> 	<dt>Description</dt>
> 	<dd>
> 		The minimum number of hours required from a student during build season. This is used in the student view. Will show true/false based >on meeting the different criteria
> 	</dd>
> 	<dt>Method</dt>
> 	<dd>
> 		hoursBuildSeason(hours)
> 	</dd>
> 	<dt>Default</dt>
> 	<dd>
> 		6 hours
> 	</dd>
> 	<dt>Modification</dt>
> 	<dd>
> 		Change the 6 to the number of hours required
> 	</dd>
> </dl>
	
### Build Season Meetings Required
> <dl>
> 	<dt>Description</dt>
> 	<dd>
> 		The minimum number of meetings required from a student during build season. This is used in the student view. Will show true/false >based on meeting the different criteria
> 	</dd>
> 	<dt>Method</dt>
> 	<dd>
> 		meetingsBuildSeason(hours)
> 	</dd>
> 	<dt>Default</dt>
> 	<dd>
> 		2 Meeting
> 	</dd>
> 	<dt>Modification</dt>
> 	<dd>
> 		Change the 2 to the number of meetings required
> 	</dd>
> </dl>

### Pre Season Meetings Required
> <dl>
> 	<dt>Description</dt>
> 	<dd>
> 		The minimum number of meetings required from a student during build season. This is used in the student view. Will show true/false >based on meeting the different criteria
> 	</dd>
> 	<dt>Method</dt>
> 	<dd>
> 		meetingsBuildSeason(hours)
> 	</dd>
> 	<dt>Default</dt>
> 	<dd>
> 		1 Meeting
> 	</dd>
> 	<dt>Modification</dt>
> 	<dd>
> 		Change the 2 to the number of meetings required
> 	</dd>
> </dl>


# Timezones
* UTC -11:00 
  * American Samoa
  * International Date Line West
  * Midway Island

* UTC -10:00
  * Hawaii

* UTC -09:00
  * Alaska

* UTC -08:00
  * Pacific Time (US & Canada)
  * Tijuana

* UTC -07:00
  * Arizona
  * Chihuahua
  * Mazatlan
  * Mountain Time (US & Canada)

* UTC -06:00
  * Central America
  * Central Time (US & Canada)
  * Guadalajara
  * Mexico City
  * Monterrey
  * Saskatchewan

* UTC -05:00
  * Bogota
  * Eastern Time (US & Canada)
  * Indiana (East)
  * Lima
  * Quito

* UTC -04:30
  * Caracas

* UTC -04:00
  * Atlantic Time (Canada)
  * Georgetown
  * La Paz
  * Santiago

* UTC -03:30
  * Newfoundland

* UTC -03:00
  * Brasilia
  * Buenos Aires
  * Greenland

* UTC -02:00
  * Mid-Atlantic

* UTC -01:00
  * Azores
  * Cape Verde Is.

* UTC +00:00
  * Casablanca
  * Dublin
  * Edinburgh
  * Lisbon
  * London
  * Monrovia
  * UTC

* UTC +01:00
  * Amsterdam
  * Belgrade
  * Berlin
  * Bern
  * Bratislava
  * Brussels
  * Budapest
  * Copenhagen
  * Ljubljana
  * Madrid
  * Paris
  * Prague
  * Rome
  * Sarajevo
  * Skopje
  * Stockholm
  * Vienna
  * Warsaw
  * West Central Africa
  * Zagreb

* UTC +02:00
  * Athens
  * Bucharest
  * Cairo
  * Harare
  * Helsinki
  * Istanbul
  * Jerusalem
  * Kyiv
  * Pretoria
  * Riga
  * Sofia
  * Tallinn
  * Vilnius

* UTC +03:00
  * Baghdad
  * Kuwait
  * Minsk
  * Nairobi
  * Riyadh

* UTC +03:30
  * Tehran

* UTC +04:00
  * Abu Dhabi
  * Baku
  * Moscow
  * Muscat
  * St. Petersburg
  * Tbilisi
  * Volgograd
  * Yerevan

* UTC +04:30
  * Kabul

* UTC +05:00
  * Islamabad
  * Karachi
  * Tashkent

* UTC +05:30
  * Chennai
  * Kolkata
  * Mumbai
  * New Delhi
  * Sri Jayawardenepura

* UTC +05:45
  * Kathmandu

* UTC +06:00
  * Almaty
  * Astana
  * Dhaka
  * Ekaterinburg

* UTC +06:30
  * Rangoon

* UTC +07:00
  * Bangkok
  * Hanoi
  * Jakarta
  * Novosibirsk

* UTC +08:00
  * Beijing
  * Chongqing
  * Hong Kong
  * Krasnoyarsk
  * Kuala Lumpur
  * Perth
  * Singapore
  * Taipei
  * Ulaan Bataar
  * Urumqi

* UTC +09:00
  * Irkutsk
  * Osaka
  * Sapporo
  * Seoul
  * Tokyo

* UTC +09:30
  * Adelaide
  * Darwin

* UTC +10:00
  * Brisbane
  * Canberra
  * Guam
  * Hobart
  * Melbourne
  * Port Moresby
  * Sydney
  * Yakutsk

* UTC +11:00
  * New Caledonia
  * Vladivostok

* UTC +12:00
  * Auckland
  * Fiji
  * Kamchatka
  * Magadan
  * Marshall Is.
  * Solomon Is.
  * Wellington

* UTC +13:00
  * Nuku'alofa
  * Samoa
  * Tokelau Is.
