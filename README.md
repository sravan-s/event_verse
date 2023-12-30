# event_verse
Implement Activitypub(https://www.w3.org/TR/activitypub/) based meetup clone\

V1 Functionality
* Event_verse is made up of servers( **club** ) that talk to eachother using activity pub protocol
* Each **club** can have admin, normal users
* **club_hub** -> discovery server(s) to which club-admins can register if they want
* User can signup to home**club**
* User has a home **club** and can post event notice
* Admin can change meta information of **club**
* Events have title, description, date
* Events can be created, edit by user. Delted by admin/user
* Events are searchable
* If user wants, can broadcast event to other **clubs**
* Users of other **clubs** can RSVP and to subscribe to the event
* UI -> Singup, Login, User Profile, Event CRUD, Public Feed, ADMIN panel
* Only implement list API for for **club_hub** - Add server, get authentication key all manually

V2 Functionality
* User subscribe to other hubs
* Admin panel, API for **club_hub**
* etc...

Idea - to implement activity pub based meetup clone to show case
Technologies:
* rust -> server in docker
* react-native -> client
* mongo + SQLite(?) -> database
* Maybe some event queue -> event sourcing(?)
* club_hub -> nextjs (?)
* Activitypub protocol -> https://www.w3.org/TR/activitypub/

> I make some small adjustments to Activitypub protocol, will be updating wiki as we go
> Also, club_hub is not really part of original Activitypub protocol, is inspired by fediverse
