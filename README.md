# SELRD
Software Engineering Learning Resources Dataset

Dataset is designed to facilitate learning concepts of Software Engineering.
It comprises of learning resources and their prerequisite relationships between topics referring to Software Engineering Learning Resources (SELR)

#Metadata.csv
metadata.csv comprises of the following fields

Sr.	Field	Description
1	ID	Unique Identifier of SELR
2	URL	In case of lectures referring to the LR/ Wikipedia page. I case of Books’ section, it refers to book’s URL
3	Topic Title	The main topic presented in SELR
4	Institute	Name of the University from where the lecture notes are extracted
5	Author/ Presented	Author of the book/ Presenter’s name in case of the lecture. In case of Wikipedia file it remains empty
6	Reading Time	Reading time required to read the text .Reading time is computed using PyPI  ‘readtime’ library which calculates read time on the average reading speed  of an adult which is 265words per minutes.
 

#Prerequisite.csv
prerequisite.csv comprises of the following format
Sr. No	Feature	Description
1	PreReqRelID	Unique Identifier for each prerequisite pair
2	PreReqTopic	The topicID of the topic that must be read prior to PostReqTopic
3	PostReqTopic	Topic ID of the topic which requires understanding of PreReqTopic 
4	PreReqRelation	PreReqRelation is 1 if the PreReqTopic serves a prerequisite for learning PostReqTopic, otherwise 0.


There are total 704Learning resources, 592 positive prerequisite relations among 302  topics
