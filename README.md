# 311-make-a-complaint-page

This repository contains information pulled from the NYC 311 Make a Complaint web application, which can be found at [http://www1.nyc.gov/311/index.page](http://www1.nyc.gov/311/index.page).  To view the app, select "Make a Complaint" from the left-side navigation bar.

Topics (e.g. "Your Home") and subtopics (e.g. for "Your Home" -> "Heat or Hot Water") one can view via the drop-down menus on the application and can also find in [this json](http://www1.nyc.gov/311_contentapi/booker.json) were extracted and parsed.  

On the application, when a subtopic is selected, it loads information from a unique json.  For example, when "Heat or Hot Water" is selected, it loads [this json](http://www1.nyc.gov/311_contentapi/services/20090318-D7301A3A-13C9-11DE-B3B8-E2470D3B2251.json). 

In this repository, [public/topics-subtopics-selected-types.json](https://github.com/fma2/311-make-a-complaint-page/blob/master/public/topics-subtopics-selected-types.json) contains topics, subtopics, subtopics' json links, and added details about each subtopic found in its unique json: categories, complaint types, and topic names.

And, [public/category-buckets-with-topics.json](https://github.com/fma2/311-make-a-complaint-page/blob/master/public/category-buckets-with-topics.json) groups topics, subtopics, and complaint types (if any) by identified category.  Category assignments were found in each subtopic's unique json - e.g. ['Heat or Hot Water'](http://www1.nyc.gov/311_contentapi/services/20090318-D7301A3A-13C9-11DE-B3B8-E2470D3B2251.json).