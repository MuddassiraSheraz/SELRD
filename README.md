# SELRD
Software Engineering Learning Resources Dataset

Dataset is designed to facilitate learning concepts of Software Engineering.
It comprises of learning resources and their prerequisite relationships between topics referring to Software Engineering Learning Resources (SELR)

#Metadata.csv
metadata.csv comprises of the following fields

ID	Unique Identifier of SELR, URL	:In case of lectures referring to the LR/ Wikipedia page. I case of Books’ section, it refers to book’s URL, Topic Title:	The main topic presented in SELR,  Institute	Name of the University from where the lecture notes are extracted, Author/ Presented	Author of the book:  Presenter’s name in case of the lecture. In case of Wikipedia file it remains empty,  Reading Time:	Reading time required to read the text .Reading time is computed using PyPI  ‘readtime’ library which calculates read time on the average reading speed  of an adult which is 265words per minutes.
 

#SEPreReq.csv organizes the preresuite relations among the topics using the following format

PreReqRelID:	Unique Identifier for each prerequisite pair, PreReqTopic:	The topicID of the topic that must be read prior to PostReqTopic, PostReqTopic:	Topic ID of the topic which requires understanding of PreReqTopic , PreReqRelation: is 1 if the PreReqTopic serves a prerequisite for learning PostReqTopic, otherwise 0.


There are total 704Learning resources, 592 positive prerequisite relations among 302  topics
