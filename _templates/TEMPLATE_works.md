
%% update the page title to the title of the work %% 

objectid:: %% add next sequential id to the tag tree # -object-id/ %%
storyverse::  %% populate the appropriate # storyverse tag %% 
title:: %% populate  the book title  %%
creator:: %% populate the author name as a page link %%
creator_type:: #creator-type/author
storyverse_type:: #storyverse-type/related-book
date:: %% populate published year %%
series_info:: %% populate value from tag tree  # series-info/ %%
description:: %% populate description %%

#### catalog info
form::  %% populate value from tag tree # form/ %%
dewey:: %% populate dewey. take out any "/" so all numeric %%
dewey_source:: %% populate value from tag tree  # -catalog-source/ %%
subject-headings:: %% populate subject heading. if more than one, add additional subject headings under this one (1 per line) %%
subject-headings_source:: %% populate value from tag tree  # -catalog-source/ %%
genres:: %% populate genre. if more than one, add additional genres under this one (1 per line) %%
genres_source::  %% populate value from tag tree  # -catalog-source/ %%

### other 
era:: %% populate value from tag tree # era/1900s/ %%
location:: %% populate value from tag tree  # loc/ . if more than one, add additional locations under this one (1 per line) %%
latitude:: %% add lat of 'primary' location %%
longitude:: %% add long of 'primary' location %%
subject:: %% populate folksonomy tags from tag tree # svf/ (storyversefolksonomy). if more than one (and there should be!) add additional subjects under this one (1 per line) %%
	subject:: 

#### book cover images
identifier:: %% currently optional %%
display_template:: %% select from tag tree  # -display-template/ . for book covers always image; any others, look into %%
object_location:: %% add the repository location for the cover image: naming convention generally objects/objectid_cover_title.jpg %%
	 image_small:: %% add the repository path - objects/small/X_sm.jpg %%
	 image_thumb:: %% add the repository path - objects/thumbs/X_th.jpg %%
image_alt_text:: %% currently optional %%


#### object transcript
object_transcript:: %% currently optional %%