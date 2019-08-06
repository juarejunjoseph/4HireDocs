## 4HireDocs
4Hire is an app built on the Thunkable Cross Platform app builder. It provides the opportunity for job seekers to find jobs posted by companies and businesses.

# Airtable Component Usage
The airtable component is used in the app. To make your own airtable storage to store the following information in 4 different tables create an account and a base with the following table names specified below:

  • users - Regular User profiles are stored here, they are the users who will seek out jobs on the platform
  • businesses - Business User profiles are stored here, they are the users who will post the jobs on the platform
  • jobslist - Individual job information is stroed here, each record holds all the information realting to a single job
  • deletionrequests - this table is still under development but its purpose is: users can delete their account and their UID is stored here so it can be looked up on firebase authentication so that their account can be deleted
  
# Airtable Table Column Headers
  • users
      -useruid
      -email
      -useridnum
      -name
      -phonenum
      -bio
      -linktocv
      -creationdate (automatically set by airtable when record is created)
      -profilepicurl
      -jobapplications
      
  • businesses
      - businessuid
      -email
      -name
      -phone
      -location
      -businessname
      -joblistings
      -creationdate
      -businesswebsite
      -logourl
      
  • jobslist
      -
