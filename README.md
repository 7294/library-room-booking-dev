#Readme

Software requirements:

* Ruby version: 2.3.1

* Rails version: 5.0.0.1

System dependencies: See gemfile

To run, download this folder, navigate to it and run 

* bundle install

* rake db:migrate

* rake db:seed #replace seeds.rb by seeds2.rb

* rails server

If you are running this app on your local machine, replace seeds.rb by seeds2.rb before running rake db:seed.
Credentials are available in seeds.rb.

This app is deployed at: https://nameless-journey-10600.herokuapp.com/

Default credentials: admin2@ncsu.edu

Password: admin01

NOTE TO REVIEWERS: PLEASE DO NOT CHANGE THE DEFAULT ADMIN PASSWORD. If you are reviewing this app and cannot login as admin, it is because another reviewer has changed the password. Please contact me at [github username] at [gmail] dot [com] so I can make a new admin. Also, please create anything that you deleted when testing, such as a room or a user. With great power comes great responsibility.

Number of reviewers inconvenienced by password changes: 1

To use:
Login as admin. Here you can create new admins, rooms and library members. As admin, you can book rooms for other members as well. You can also cancel bookings, provided the booking start time has not passed. 
You may create users as admin or sign up from the login page to create regular library users who can book rooms for themselves. As a user, you can view your own booking history and cancel booking, provided the start time has not elapsed. All bookings can be done for two hour slots only. This was assumed based on the requirements.

When logged in as a user or admin, you can edit your profile by clicking on your own name.

To test: rake test

Deleting a room with a booking:

This is not possible in the app, as the delete button will not show for a room that has a booking.

Deleting a user with a booking:

This is not possible as the delete button does not show for a user with a booking. 

For both these cases, you must first cancel all bookings for that room or user and then delete the room/user.

To edit the details of the room, there is an icon next to the room name on the left side.

Sending email to attendees is currently not working as app-specific passwords have not been set up.
