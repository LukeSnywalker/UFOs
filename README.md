# UFOs

## Overview

The purpose of this project is to use HTML and JavaScript to create a website that filters data of UFO sightings based on user input.

## Results

This website features a table of UFO sightings that occurred between January 1st and January 13th, 2010. Each sighting has its date, the city, state, and country it took place in, the shape of the UFO(s), the duration of the sighting, and any comments made by the witness.

![How the table appears when the page first loads](/Resources/default_table.png)

The table can be filtered on any of the criteria listed on the left side, under "Filter Search". To perform a search, the user can enter what they would like to search for in any of the text boxes, hit Enter, and the table will automatically display all of the data that contain that search criterion. Examples are listed in each of the text boxes. For example, if the user were to input "st. louis" in the City box, the table would display all sightings that took place in St. Louis (which in this case is only one sighting).

![Search results for "st. louis" as the city](/Resources/search_example.png)

The user can also search for multiple criteria. For example, if they wanted to see all sightings of triangle-shaped UFOs in Oregon, they would input "or" in the State box and "triangle" in the Shape box.

![Search results for "or" as the state and "triangle" as the shape](/Resources/multiple_search_example.png)

## Summary

A drawback of this webpage is that the searches are case-sensitive, and they must match the exact format and spelling as in the data. If the user were to search for "St. Louis" or "st louis" instead of "st. louis", results would not be displayed, because the website script only searches for exact matches for the user input.

To further develop this webpage, we could find a way to be make data matches more lenient, possibly using regex in the filterTable() function in app.js. We could also add code in app.js and an additional "li" element in index.html that would allow the user to search the comments for certain keywords.