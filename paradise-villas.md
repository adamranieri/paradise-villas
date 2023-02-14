# Paradise Villas

You and your team will be creating a mobile app for a vacation resort called Paradise Villas. You can make the resort any work appropriate vacation resort you want, Ski Resort, Beach Resort etc... Paradise Villas is trying to create a new digital experience. They want all their guests to be able to use the Resort App for an all inclusive portal once they arrive. Another team has already developed the APIs and backend infrastructure. You will be provided.
- Diagrams of how the app should look and operate
- User Stories
- A github repo linked to a jenkins instance 
  - This jenkins instance will perform builds of your application
- A splunk server that you will use to consolidate the logs from you application
- A Firebase project that will be used for 
  - Logging/tracking events
  - Storing images
  - Realtime DB

### Main features
- Employee Clock-in
  - Managers want to know who is currently available at any time
- Employee Messaging
  - Employees can send messages to each other
  - Employees can view all their messages
  - Employees can search their messages
- Employee Photos
  - Per guest request an employee can take a picture on with the employee's phone, look up the vacationer and send them the picture
- Vacation Event finder
  - Vacationers can find events going on at the resport
  - Can search by time, or tags
- Vacation Problem Reporter
  - Vactioners can report problems via app
- Vacation Room Service
  - Vacationers can request room service and get updates
- Vacation QR Code Reservations
  - Vacationers can scan QR codes found around the resort to register for events and make reservations
- Vacation Details and pictures
  - Vactioners can look at
    - Their reservation info
    - Any events they have signed up for
    - Any photos sent to them

### User Stories
|As a | I Want to | So That|
|-----|-----------|--------|
| Vacationer | Login with my reservation ID | I can see my reservation details (room, check-in check-out) |
| Vacationer | View upcoming events and shows | I can attend events I am interested in |
| Vacationer | Order Room Service | I can have food delivered to my room |
| Vacationer | Report a problem | issues can be addressed |
| Vacationer | Report a problem and attach an optional photo | the problem can be made clear |
| Vacationer | scan hidden VR codes | participate in the scavenger hunt for rewards |
| Manager    | Login with my username and password | I can manage my employees |
| Manager    | view active employees | I can see who is currently available |
| Manager    | View current problems | I can address problems as they arise |
| Manager    | Message employees | I can get quick updates notes |
| Manager    | Create Events | Guests can be engaged in the latest happenings |
| Manager    | Create assignments for employees | I can manage workloads |
| Employee   | Login with my username and password | I can find my work assignments |
| Employee   | Set my status | My manager knows what I am engaged with |
| Employee   | Send messages to managers and other employees | I can staty in constant communcation |
| Employee   | Send messages and photos to guests | Guests can get appropriate links |

## Firebase requirements
- Images are stored in firebase storage
- Realtime DB is used for tracking room service
- Firebase events is used to track
  - Vacationer login
  - Vacationer room service sent, fulfilled and updated
  - Errors

## Splunk Monitoring/logging
- All key events must be logged in splunk
  - Vactioneer login
  - Vacationer room service sent and fulfilled and upate
  - Employee login
  - Employee logout
- All bugs and errors should be sent to splunk
- You should create dashboards and queries
  - A dashboard to show off feature usage
  - A dashboard to show off employee hours
  - A dashboard to show off bugs encountered in the application

***You will be making logs in Firebase and splunk***


### Presentation Format
- You will have your application available to download for android.
- You will share your phone on the computer and walk through your features. 

### Technial Requirements
- All code is in github
- Project has been fully managed using agile methodologies by Github projects
- All code has been sent to jenkins