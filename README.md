# Unit 11 Express Homework: Note Taker

https://week11-note-taker.herokuapp.com/notes

## Description

Create an application that can be used to write, save, and delete notes. This application will uses express backend and save and retrieve note data from a JSON file.

- The application frontend was created, I built the backend and connected the two.

- The following HTML routes are used:

  - GET `/notes` returns the `notes.html` file. ![Screen Shot of /notes path.](./Develop/public/assets/notes.png)

* GET `*` returns the `index.html` file. ![Screen Shot of home page.](./Develop/public/assets/home.png)

- The notes are stored in a `db.json` file on the backend. The `fs` module is used to read and write to this file.

* The following API royes were created:

  - GET `/api/notes` reads the `db.json` file and return all saved notes as JSON. ![Screen shot of /api/notes (get)](./Develop/public/assets/getapi.png)

  - POST `/api/notes` receives a new note to save on the request.body, add it to the `db.json` file, and then return the new note to the client when the save icon is clicked. Here is the screen shot before saving (with the save icon circled): ![Screen shot before saving](./Develop/public/assets/before.png)
