# Game-Analytics-ETL-In-R
downloading Game Analytics files from server and import them into a RDBMS




1. Export all the links from GA pannel
2. Save all the links you want to download in text file. (here:   D:work/garageGames/GA_links.txt)
3. My Ga has 3 main Component. I save 2 important ones :   user_meta   and  data. so I save field-names in 2 Vectors:db_fields_user_meta , df_fields_data
4. input credentials of db. (mysql in my case)
5. create a table including all this fields in your DB
6. Run the FOR loop. It does the followings:
   A) download the link
   B) Unzip the Jason file
   C) Parse Jsone into 2 Dataframes (user_meta   and    data)
   D) Conbines user_meta   and  data in a dataframe called "All"
   E) save "All" to mysql
   
   
   
