# Application Flow

# ID attribute values

* _races_
    Applied to a div tag.  The list of races in this representation.
* _runners_
    Applied to a div tag.  The list of runners in this representation.
* _race_
    Applied to a dl tag.  The list of parameters for a race in this representation.
* _runner_
    Applied to a dl tag.  The list of parameters for a runner in this representation.

# Class attribute values

* _actions_
    Applied to an unordered list.  The list of actions for the application.
* _all-races_
    Applied to an unordered list.  Represents the entire list of races.
* _race_
    Applied to a list item tag or a dd tag.  Represents a race.
* _race-url_
    Applied to an A tag.  Represents the URL for a race.
* _race-name_
    Applied to a span tag.  Represents the name for a race.
* _race-description_
    Applied to a span tag.  Represents the description of a race.
* _update-race_
    Applied to a form tag.  Used to update attributes for a race in this representation.
* _all-runners_
    Applied to an unordered list.  Represents the entire list of runners.
* _runner_
    Applied to a list item tag.  Represents a runner.
* _runner-url_
    Applied to an A tag.  Represents the URL for a runner.
* _runner-name_
    Applied to a span tag.  Represents the name of a runner.
* _runner-time_
    Applied to a span tag.  Represents the time of a runner in a race.
* _runner-image_
    Applied to an img tag.  Represents the image of a runner.
* _country_
    Applied to a span tag.  Represents the country of a runner.
* _search-runners_
    Applied to a form tag.  Used to search for runners in this representation.
* _create-runner_
    Applied to a form tag.  Used to create a runner in this representation.
* _update-runner_
    Applied to a form tag.  Used to update a runner in this representation.

# Name attribute values

* __method_
    Applied to an INPUT[hidden] element.  The method of a form.
* _item[id]_
    Applied to an INPUT[text] element.  The ID of a race.
* _item[name]_
    Applied to an INPUT[text] element.  The name of a race or a runner.
* _item[url]_
    Applied to an INPUT[url] element.  The URL of a race.
* _item[description]_
    Applied to a TEXTAREA element.  The description of a race.
* _name_
    Applied to an INPUT[text] element.  The name of a runner, when searching for a runner.
* _item[race]
    Applied to an INPUT[hidden] element or a SELECT element.  The ID of a race, used for linking runners to races
* _item[time]
    Applied to an INPUT[text] element.  The time of a runner in a race.
* _item[image]
    Applied to an INPUT[url] element.  The URL of an image of a runner.
* _item[country]
    Applied to an INPUT[text] element.  The country of a runner.

# Rel attribute values

* _index_
    Applied to an A tag.  A reference to the list of actions of the application.
* _races_
    Applied to an A tag.  A reference to the list of all races.
* _runners_
    Applied to an A tag.  A reference to the list of all runners.
* _race_
    Applied to an A tag.  A reference to a single race.
* _runner_
    Applied to an A tag.  A reference to a single runner.

# Data Description (RDFa)

* _vocab_
    * http://schema.org/
* _typeof_
    * SportsEvent - used to refer to a single race
    * Person - used to refer to one or more runners in a race
* _property_
    * url (in SportsEvent) - used to refer to the URL of a race   
    * name (in SportsEvent) - used to refer to the name of a race
    * performers (in SportsEvent) - used to refer to the runners of a race.  Typeof is Person
    * description (in SportsEvent) - used to refer to the description of a race
    * url (in Person) - used to refer to the URL of a runner
    * name (in Person) - used to refer to the name of a runner
    * nationality (in Person) - used to refer to the country of a runner
    * performerIn (in Person) - used to refer to the race in which a runner participated.  Typeof is SportsEvent
    * awards (in Person) - used to refer to the runner's time in a race
    * image (in Person) - used to refer to the image of a runner
    
    