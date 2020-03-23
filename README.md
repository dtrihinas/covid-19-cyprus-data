# covid-19-cyprus-data
Dataset capturing the publically released data regarding covid-19 cases across Cyprus.

Hopefully this dataset can be used in the future (as covid-19 from what I understand will be seasonal) by relevant practitioners and data scientists.

This dataset is intended to be updated daily when new announcements (although I hope there are no more) about possitive cases released.

I assume no responsibility for the accuracy of this data. It was collected by trawling the goverment's announcements and from scraped information released by media outlets. There are times where these do not completely agree.

This is an open call to anyone willing to help with the data collection process. If you are interested in correcting, updating or enriching the dataset then contact me (trihinas{at}unic.ac.cy) or do a pull/push request. The end goal is to host this data publically and in an open format (like others are doing in the EU). Possible repository could be the cyprus open data platform.

Dataset attributes:

- caseid: only used to refer contacts with initial cases. may be useful to discover communities.
- date: this is the date the case was announced to the public.
- gender, age, nationality and profession: these are data referring to the case subject. If data is missing it is labeled as NA. Initially, there was more data released by media outlets but with the increase of cases the data is more sparse.
- area: this data reflects the cyprus providence. It can be more fine-grained in the future (e.g., stavrovouni instead of larnaca).
- impact: how the case was (possibly) occured. Travel includes the origin. contact is the other possibility and we also have unknown.
- hospitalized refers to hospitalization of the case, ICU means the patient was admitted to the ICU while recovered refers to the patient recovered. This data can be completely wrong. Also, up to now, recovered cases are just referred by the goverment as numbers (e.g., 2 recovered) and do not state which case has recovered. so this attribute may be completely useless.
- relation: this attribute refers to contacts and if we know which case was the contact related to (e.g., all the nurse personell in paphos gen. hospital came in contact with patient in ICU). A -1 is used for cases that were occured by travel and NA if the contact is unknown.

