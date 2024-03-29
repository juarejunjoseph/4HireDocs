# 4Hire Documentation
4Hire is an app built on the Thunkable Cross Platform app builder. It provides the opportunity for job seekers to find jobs posted by companies and businesses.


## Firebase Component Usage

The Firebase component is used for authentication in the app. If you need to, create a firebase account and make sure you apply your own firebase API Key to enable the authentication feature.


## Web Api Component Usage

For all the web api components make sure that you apply your own API keys to ensure that they function properly. 


## Airtable Component Usage

The airtable component is used in the app. To make your own airtable storage to store the following information in 4 different tables create an account and a base with the following table names specified below:


- **users** - Regular User profiles are stored here, they are the users who will seek out jobs on the platform
  
- **businesses** - Business User profiles are stored here, they are the users who will post the jobs on the platform
  
- **jobslist** - Individual job information is stroed here, each record holds all the information realting to a single job
  
- **deletionrequests** - this table is still under development but its purpose is: users can delete their account and their UID is stored here so it can be looked up on firebase authentication so that their account can be deleted
  
  
### Airtable Table Column Headers

- **users**
  - useruid
  - email
  - useridnum
  - name
  - phonenum
  - bio
  - linktocv
  - creationdate (automatically set by airtable when record is created)
  - profilepicurl
  - jobapplications
      
- **businesses**
  - businessuid
  - email
  - name
  - phone
  - location
  - businessname
  - joblistings
  - creationdate
  - businesswebsite
  - logourl
     
- **jobslist**
  - businessrownum
  - jobnum
  - businessname
  - available
  - skills
  - startdate
  - finishdate
  - jobtype
  - description
  - applicants
  - salary
  - salarytype
  - worktimequantity
  - listingdate

- **deletionrequests**
  - uid
  
## Color Palette

- #f2f4f6 (Light Primary)
- #1ee3cf (Light Secondary)

- #6b48ff (Dark Primary)
- #525252 (Dark Secondary)
- #0d3f67 (Dark Tertiary

Visit https://colorhunt.co/palette/148116 for a preview of the color palette.

## Design Standards

- All screens are **CENTER** aligned horizontally and **TOP** aligned vertically
- Each screen has a padding of **5%** on the left and the right only
- Border radius used on buttons is **10px**
- Border radius used on card style view and list views is **30px**
- All components (excluding those which have an Alpha component to their color) are raised with an elevation of **5**
- Back navigation/other secondary buttons are smaller than the primary button
- Error and Success messages must all use the same 2 Alert components but the message can vary per usage

