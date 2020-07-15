• It’s full stack but filter is developed only in .Net core c#.

• Reasoning behind your technical choices, including architectural. - Best practices with SOLID principles

• Trade-offs you might have made, anything you left out, or what you might do differently if
you were to spend additional time on the project.- If I had time, I would have first written unit tests, interation tests, implemented Logger, Imporoved DB design, secured credentials into secret vault.


Follow below steps to run this project:

Restore the SQL server DB attached with the name "TEMS.sql", I have use sql server 2016.

unzip "Movies Services using Dot Net Core API with EF Core.zip".

Open the .net core solution and change the sql connection string.
Run the .net core application and open below URL
http://localhost:55618/swagger/index.html

Below are the APIs implemented.

VideoLibrary

GET
​/api​/VideoLibrary​/GetAllVideos
GET
​/api​/VideoLibrary​/GetVideos
GET
​/api​/VideoLibrary​/GetVideoById
POST
​/api​/VideoLibrary​/AddVideo
POST
​/api​/VideoLibrary​/UpdateVideo
DELETE
​/api​/VideoLibrary​/DeleteVideoById


​/api​/VideoLibrary​/GetVideos    -  This api is implemented with filter 

in filterColumn use the column name to filter such as Locations and in filterQuery the content like "newyork"


Unzip "Angular Video Library UI App.zip"
This applicaton is developed on angular 9 and above API is already integrated in this. Filter is not done in the UI due to time contraint.
Follow below steps:
npm i
ng serve
