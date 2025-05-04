``` dataview
TABLE WITHOUT ID 
	file.aliases AS i,
	regexreplace(objectid,".*/(.*)","$1") AS objectid, 
	storyverse, 
	title, 
	creator, 
		regexreplace(creator_type,".*/(.*)","$1") AS creator_type,
	regexreplace(storyverse_type,".*/(.*)","$1") AS storyverse_type, 
	date, 
	regexreplace(series_info,".*/(.*)","$1") AS series_info, 
	description,
	regexreplace(form,".*/(.*)","$1") AS form, 
	dewey, regexreplace(dewey_source,".*/(.*)","$1") AS dewey_source, 
	join(map(subject-headings, (x) => "#s-h/ " + x),"; ") AS subject-headings, 
		regexreplace(subject-headings_source,".*/(.*)","$1") AS subject-headings_source, 
	join(map(genres, (x) => "#g/ " + x),"; ") AS genres, 
		regexreplace(genres_source,".*/(.*)","$1") AS genres_source,
	join(era,"; ") AS era, 
	join(location,"; ") AS location, 
	longitude, latitude, 
	join(subject,"; ") AS subject,
	identifier, regexreplace(display_template,".*/(.*)","$1") AS display_template, 
	object_location, image_small, image_thumb, image_alt_text
FROM "works" 
SORT objectid
```


