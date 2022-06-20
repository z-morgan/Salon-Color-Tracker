Link to the app: https://salon-color-tracker.herokuapp.com/signin

Salon Color Tracker is a web app designed to help hair dressers manage their supply of hair color products. It is a Ruby web app built using the Sinatra web development framework. It employs ERB as the templating language for dynamically generating HTML pages. The app is backed by a PostgreSQL database. Passwords are secured using bcrypt, and user input is sanatized throughout the site to protect against cross-site scripting. A comprehensive test suite is provided which uses Rack's built-in testing library. 

Some things to be aware of:
1. If you are not familiar with hair products it may be helpful to know that hair colors employ a special classification system comprised of two numbers seperated by a "/". The first number is the "Depth" of the color, and is an integer from 1 to 11. The second number is the "Tone" of the color, and is composed of an alphanumeric character representing the major tone, with an optional second character representing the minor tone. The minor tone is a subdivision of the major tone. Thus, "11" would come after "1", but before "2". The complete color number will look like this: "3/5", where "3" is the depth and "5" is the tone. 

2. The "color line" is the brand which produces the color product. 


Thank you for checking out my app! I hope you enjoy your visit. 

Zach Morgan - Developer



Notes for developers:
If you pull down the code to your local machine, you must setup the database yourself. This can be done easily by `cd`ing into the `/data` directory, and running `ruby db_setup.rb`. As long as you have PostgreSQL installed and running on your machine, this (along with `bundle install`) should be all you need to run the app locally. 