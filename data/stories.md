## complete path
* greet
    - utter_greet
* restaurant_search
    - utter_ask_location
* restaurant_search{"location": "delhi"}
    - slot{"location": "delhi"}
	- verify_location
    - utter_ask_cuisine
* restaurant_search{"cuisine": "chinese"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "delhi"}
    - utter_ask_budget_for_two
* restaurant_search{"budgetmin": "0", "budgetmax": "300"}
    - slot{"budgetmax": "300"}
    - slot{"budgetmin": "0"}
    - verify_budget
    - slot{"budgetmin": 0}
    - slot{"budgetmax": 300}
    - slot{"budget_ok": true}
    - action_search_restaurants
    - slot{"location": "Delhi"}
    - slot{"restaurant_exist": true}
    - utter_ask_ifmail
* affirm
    - utter_ask_email
* send_email{"email": "sarojrasaproject@gmail.com"}
    - slot{"email": "sarojrasaproject@gmail.com"}
    - action_validate_email
    - slot{"email_ok": true}
    - slot{"email": "sarojrasaproject@gmail.com"}
    - action_send_mail
* goodbye
    - utter_goodbye
    - export

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"cuisine": "chinese", "location": "Delhi"}
    - slot{"cuisine": "chinese"}
    - slot{"location": "Delhi"}
    - verify_location
    - slot{"location": "Delhi"}
    - slot{"location_ok": true}
    - utter_ask_budget_for_two
* restaurant_search{"budgetmin": "300", "budgetmax": "700"}
    - slot{"budgetmax": "700"}
    - slot{"budgetmin": "300"}
    - verify_budget
    - slot{"budgetmin": 300}
    - slot{"budgetmax": 700}
    - slot{"budget_ok": true}
    - action_search_restaurants
    - slot{"location": "Delhi"}
    - slot{"restaurant_exist": true}
    - utter_ask_ifmail
* affirm
    - utter_ask_email
* send_email{"email": "sarojrasaproject@gmail.com"}
    - slot{"email": "sarojrasaproject@gmail.com"}
    - action_validate_email
	- slot{"email_ok": true}
    - slot{"email": "sarojrasaproject@gmail.com"}
    - action_send_mail
* goodbye
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "xyz"}
    - slot{"location": "xyz"}
    - verify_location
    - slot{"location": null}
    - slot{"location_ok": false}
    - utter_ask_location
* restaurant_search{"location": "patna"}
    - slot{"location": "patna"}
    - verify_location
    - slot{"location": "patna"}
    - slot{"location_ok": true}
    - utter_people
* people
    - utter_ask_budget_for_two
* restaurant_search{"budgetmin": "300", "budgetmax": "700"}
    - slot{"budgetmax": "700"}
    - slot{"budgetmin": "300"}
    - utter_ask_cuisine
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - action_search_restaurants
    - slot{"location": "patna"}
    - slot{"restaurant_exist": true}
    - utter_ask_ifmail
* affirm
    - utter_ask_email
* send_email{"email": "sarojrasaproject@gmail.com"}
    - slot{"email": "sarojrasaproject@gmail.com"}
    - action_validate_email
    - slot{"email_ok": true}
    - action_send_mail
* affirm
    - utter_goodbye

## interactive_story_1
* greet
    - utter_greet
* restaurant_search{"location": "dumdum"}
    - slot{"location": "dumdum"}
    - verify_location
    - slot{"location": null}
    - slot{"location_ok": false}
    - utter_ask_location
* restaurant_search{"location": "Kolkata"}
    - slot{"location": "Kolkata"}
    - verify_location
    - slot{"location": "Kolkata"}
    - slot{"location_ok": true}
    - utter_people
* people
    - utter_ask_budget_for_two
* restaurant_search{"budgetmin": "300", "budgetmax": "700"}
    - slot{"budgetmax": "700"}
    - slot{"budgetmin": "300"}
    - utter_ask_cuisine
    - utter_ask_cuisine
* restaurant_search{"cuisine": "South Indian"}
    - slot{"cuisine": "South Indian"}
    - action_search_restaurants
    - slot{"location": "Kolkata"}
    - slot{"restaurant_exist": true}
    - utter_ask_ifmail
* affirm
    - utter_ask_email
* send_email{"email": "sarojrasaproject@gmail.com"}
    - slot{"email": "sarojrasaproject@gmail.com"}
    - action_validate_email
    - slot{"email_ok": true}
    - action_send_mail
* affirm
    - utter_goodbye