# Lunch Reviews
What's for lunch?  
Something Good?

## Running The Application

Make sure you're in the `lunch-reviews` directory.  Once there, run the following two commands to configure your application correctly:

```
$ bundle install --without production
$ rake setup:dotenv
```

### On Cloud9

If you're using [Cloud9](http://c9.io), run the application with

```
$ ruby lunch-review-app.rb -p $PORT -o $IP
```

### On Your Own Computer

If you're on your own computer, run the application with

```
$ ruby lunch-review-app.rb
```

If everything runs successfully, you should be able to visit <http://localhost:4567> and see the web application.



-------------------
irb -r./environment

Seed.rb is for all the necessary things for our program to run as Jesse said.

lunch = Lunch.new(date: "2015-4-25")
lunch.add_menu_item_ids(["1", "2"])


user = User.find_by_email("kirby@kirby.com")
user.admin = true
user.save