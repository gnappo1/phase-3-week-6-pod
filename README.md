# Week 6 Pod Challenge Instructions

Before you start, decide who will be the driver first. Keep an eye on the time and make sure you switch drivers at the halfway mark. Please ask for help if you are unsure how to share your code across github.

## Step 1

- Install the [corneal-new gem](https://github.com/cjbrock/corneal-new/)

```unix
gem install corneal-new
```

- Use the corneal gem to create a new Sinatra application called 'ice-cream-shop'

```unix
 corneal new doctor-office
```

- `cd` into your new doctor-office directory

## Step 2

- Go to github and create a new repository
- Connect the repository with your newly created corneal app
- Refresh the page on github to make sure it is correctly synced

## Step 3

Create migrations and set up models. You should have the following models:

- Physician
    has the following attributes: name, title, age, email, phone, experience (in years), (password only if you have gotten to the section on passwords)

- Patient
    has the following attributes: name, email, (password only if you have gotten to the section on passwords)

- Appointment
    has the following attributes: physician_id, patient_id, date (datetime), location

Don't forget to migrate before moving on.

## Step 4

Add appropriate model [validations](https://guides.rubyonrails.org/active_record_validations.html) (presence, uniqueness, length, inclusion/exclusion) and [associations](https://guides.rubyonrails.org/association_basics.html)!

## Step 5

Create some seed data. You can do this using a seeds.rb file or by starting the `rake console` (or tux) and creating a few objects.

## Step 6

In your Controller, write out all 5 of the restful routes for appointments (move to the other controllers when you're done). Try to do this on your own but if you get stuck, you can google the REST summary chart online. Add comments above each route to say what it will be used for.

## Step 8

- Test your routes and logic using Postman
