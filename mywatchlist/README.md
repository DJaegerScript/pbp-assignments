# [Assignment 3: Implement Data Delivery using Django](https://pbp-assigments-adjie.herokuapp.com/)

## Name : Adjie Djaka Permana

## NPM : 2106702485

# QUESTIONS

1. **Explain the difference between JSON, XML, and HTML!**  
   
   - **JSON**, JavaScript Object Notation is a standard data transfer format that is based on Javascript object syntax. It is exist as a string and must be parsed to native Javascript object to access the data. Hence, JSON provide an easy way to parse its data. Although, JSON is based on JavaScript, it is used independently as `.json` file and can be used universally.
   - **XML**, Extensible Markup Language is a markup language that the tag is can be defined as you want. This markup language is usually used to store the data. Also, the XML structure is standardized. So, if you transmit the XML data across the platform, the recipient will easily parse its data.
   - **HTML**, Hypertext Markup Language is a markup language with many predefined tags. It defines the meaning and structure of web content.

   So, HTML will store the data in form of web content, but it is not easy to access the data of HTML because it can be structured differently. While, JSON & XML provide a powerful way to stores the data and an easy way to access the data, but JSON is more readable and lightweight than XML.
   
2. **Explain why we need the data delivery when implementing on a platform!**

   Every software in every platform is developed uniquely and authorized by different people. But, sometimes, they need the same data to ensure their business logic to perform correctly. In this case, we need data delivery to provide communication between these apps.

   A simple example of data delivery is how the front end communicates with the back end. The front will become a friendly interface for users to input their data. While the backend organizes the data that is sent by the front end. They can deliver the data using different kinds of data delivery mechanisms.  

3. **Explain how do you complete the tasks in this assignment!**

   At first, I'll create the new Django app named `mywatchlist` using `startapp` command and then register it on `INSTALLED_APPS` in `settings.py`. 

   After that, I register the URL path on the main's `urls.py` and register the variations of the URL path on `mywatchlist`'s `urls.py` . 
   
   Before developing the views, I create and distribute the data of the model using `makemigrations`, `migrate`, and `loaddata`.

   Almost the last, I develop the views logic for each URLs that I registered. But, for `mywatchlist/` and `mywatchlist/html`, I used the same views logic because they're supposed to respond with the same data.

   Lastly, I deployed the apps, but I did a bit modifications on the `Procfile`'s `release` job. Instead of making it to load only a specific app's fixtures, I make it to load all the fixtures in the project. So, when in the future I have to add a new fixture, I don't have to modify the `Procfile` each time I want to deploy.

# POSTMAN SCREENSHOT

1. `/mywatchlist`
   ![/mywatchlist](https://github.com/DJaegerScript/pbp-assignments/blob/main/mywatchlist/mywatchlist.png?raw=true)

2. `/mywatchlist/html`
   ![/mywatchlist](https://github.com/DJaegerScript/pbp-assignments/blob/main/mywatchlist/mywatchlist-html.png?raw=true)

3. `/mywatchlist/json`
   ![/mywatchlist](https://github.com/DJaegerScript/pbp-assignments/blob/main/mywatchlist/mywatchlist-json.png?raw=true)
   
4. `/mywatchlist/json/6`
   ![/mywatchlist](https://github.com/DJaegerScript/pbp-assignments/blob/main/mywatchlist/mywatchlist-json-6.png?raw=true)
   
5. `/mywatchlist/xml`
   ![/mywatchlist](https://github.com/DJaegerScript/pbp-assignments/blob/main/mywatchlist/mywatchlist-xml.png?raw=true)
   
6. `/mywatchlist/xml/9`
   ![/mywatchlist](https://github.com/DJaegerScript/pbp-assignments/blob/main/mywatchlist/mywatchlist-xml-9.png?raw=true)
   
