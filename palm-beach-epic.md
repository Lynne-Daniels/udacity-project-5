Udacity Front End Web Developer Nanodegree Project Five
6/6/2015 by Lynne Daniels

This single page website provides information about a local cycling route. The trackline shows the route to be taken by riders, and the markers 
show points of interest that the riders need to know about.

	1. Knockout used to link a search box with a list of search terms.
	2. Google map with a track and markers
	
		a. Track is an XML file - has to be on a web server,
		   currently at http://floridabiketrail.org/gpsdata/palm-beach-epic-jupiter-start10.kml
		b. Markers are in separate JSON file, but also repeated in the code for easy testing w/o cross origin issues.
		
	3. Data from www.strava.com shows riders who have ridden a section of the course.
	
		a. Segment definition provided by Strava.  We have to find or upload new segments for any new pages.
		
	4. An infowindow describing the marker's location pulls data from TripAdvisor API to list local POI.
	
		a. TripAdvisor API key is for testing only.  Must show them the final page to get approval to publish.
		b. markers also have static content in their "html" attribute, which precedes the TripAdvisor Listings
		
	5. Uses online libraries from CDNs -- see URLs in file map-page.js
	
		a. Bootstrap
		b. JQuery
		c. Google Maps
		d. Knockout
		
	6. Files Required
	
		a. palm-beach-epic.html
		b. js/map-page.js
		c. styles/map-page.css
		d. images/ florida-cypress-swamp-biking.jpg
		e. avatar/athlete/large.png (This is a kludge for now - Strava's API returns a local path when there is no image.  Should be updated to use CSS/HTML instead.)
			(Remember those old phone bills that said "This page intentionally left blank." It's like that -- easier to mail a blank page that to fix it.)
		f. palm-beach-epic-jupiter-start10.kml - track data served on a web host
		g. json - goal is to use only jsons, but this version is optional - see comments in js file