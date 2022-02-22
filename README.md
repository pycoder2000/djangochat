# Django ChatApp

[![forthebadge](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMTAuNTYiIGhlaWdodD0iMzUiIHZpZXdCb3g9IjAgMCAyMTAuNTYgMzUiPjxyZWN0IGNsYXNzPSJzdmdfX3JlY3QiIHg9IjAiIHk9IjAiIHdpZHRoPSIxMTUuMzEiIGhlaWdodD0iMzUiIGZpbGw9IiMzMUM0RjMiLz48cmVjdCBjbGFzcz0ic3ZnX19yZWN0IiB4PSIxMTMuMzEiIHk9IjAiIHdpZHRoPSI5Ny4yNSIgaGVpZ2h0PSIzNSIgZmlsbD0iIzM4OUFENSIvPjxwYXRoIGNsYXNzPSJzdmdfX3RleHQiIGQ9Ik0xNS42OSAyMkwxNC4yMiAyMkwxNC4yMiAxMy40N0wxNi4xNCAxMy40N0wxOC42MCAyMC4wMUwyMS4wNiAxMy40N0wyMi45NyAxMy40N0wyMi45NyAyMkwyMS40OSAyMkwyMS40OSAxOS4xOUwyMS42NCAxNS40M0wxOS4xMiAyMkwxOC4wNiAyMkwxNS41NSAxNS40M0wxNS42OSAxOS4xOUwxNS42OSAyMlpNMjguNDkgMjJMMjYuOTUgMjJMMzAuMTcgMTMuNDdMMzEuNTAgMTMuNDdMMzQuNzMgMjJMMzMuMTggMjJMMzIuNDkgMjAuMDFMMjkuMTggMjAuMDFMMjguNDkgMjJaTTMwLjgzIDE1LjI4TDI5LjYwIDE4LjgyTDMyLjA3IDE4LjgyTDMwLjgzIDE1LjI4Wk00MS4xNCAyMkwzOC42OSAyMkwzOC42OSAxMy40N0w0MS4yMSAxMy40N1E0Mi4zNCAxMy40NyA0My4yMSAxMy45N1E0NC4wOSAxNC40OCA0NC41NyAxNS40MFE0NS4wNSAxNi4zMyA0NS4wNSAxNy41Mkw0NS4wNSAxNy41Mkw0NS4wNSAxNy45NVE0NS4wNSAxOS4xNiA0NC41NyAyMC4wOFE0NC4wOCAyMS4wMCA0My4xOSAyMS41MFE0Mi4zMCAyMiA0MS4xNCAyMkw0MS4xNCAyMlpNNDAuMTcgMTQuNjZMNDAuMTcgMjAuODJMNDEuMTQgMjAuODJRNDIuMzAgMjAuODIgNDIuOTMgMjAuMDlRNDMuNTUgMTkuMzYgNDMuNTYgMTcuOTlMNDMuNTYgMTcuOTlMNDMuNTYgMTcuNTJRNDMuNTYgMTYuMTMgNDIuOTYgMTUuNDBRNDIuMzUgMTQuNjYgNDEuMjEgMTQuNjZMNDEuMjEgMTQuNjZMNDAuMTcgMTQuNjZaTTU1LjA5IDIyTDQ5LjUxIDIyTDQ5LjUxIDEzLjQ3TDU1LjA1IDEzLjQ3TDU1LjA1IDE0LjY2TDUxLjAwIDE0LjY2TDUxLjAwIDE3LjAyTDU0LjUwIDE3LjAyTDU0LjUwIDE4LjE5TDUxLjAwIDE4LjE5TDUxLjAwIDIwLjgyTDU1LjA5IDIwLjgyTDU1LjA5IDIyWk02Ni42NSAyMkw2NC42OCAxMy40N0w2Ni4xNSAxMy40N0w2Ny40NyAxOS44OEw2OS4xMCAxMy40N0w3MC4zNCAxMy40N0w3MS45NiAxOS44OUw3My4yNyAxMy40N0w3NC43NCAxMy40N0w3Mi43NyAyMkw3MS4zNSAyMkw2OS43MyAxNS43N0w2OC4wNyAyMkw2Ni42NSAyMlpNODAuMzggMjJMNzguOTAgMjJMNzguOTAgMTMuNDdMODAuMzggMTMuNDdMODAuMzggMjJaTTg2Ljg3IDE0LjY2TDg0LjIzIDE0LjY2TDg0LjIzIDEzLjQ3TDkxLjAwIDEzLjQ3TDkxLjAwIDE0LjY2TDg4LjM0IDE0LjY2TDg4LjM0IDIyTDg2Ljg3IDIyTDg2Ljg3IDE0LjY2Wk05Ni4yNCAyMkw5NC43NSAyMkw5NC43NSAxMy40N0w5Ni4yNCAxMy40N0w5Ni4yNCAxNy4wMkwxMDAuMDUgMTcuMDJMMTAwLjA1IDEzLjQ3TDEwMS41MyAxMy40N0wxMDEuNTMgMjJMMTAwLjA1IDIyTDEwMC4wNSAxOC4yMUw5Ni4yNCAxOC4yMUw5Ni4yNCAyMloiIGZpbGw9IiNGRkZGRkYiLz48cGF0aCBjbGFzcz0ic3ZnX190ZXh0IiBkPSJNMTMxLjQ3IDIyTDEyNy41MCAyMkwxMjcuNTAgMTMuNjBMMTMxLjQ3IDEzLjYwUTEzMi44NSAxMy42MCAxMzMuOTIgMTQuMTJRMTM0Ljk5IDE0LjYzIDEzNS41OCAxNS41OFExMzYuMTYgMTYuNTMgMTM2LjE2IDE3LjgwTDEzNi4xNiAxNy44MFExMzYuMTYgMTkuMDcgMTM1LjU4IDIwLjAyUTEzNC45OSAyMC45NyAxMzMuOTIgMjEuNDhRMTMyLjg1IDIyIDEzMS40NyAyMkwxMzEuNDcgMjJaTTEyOS44OCAxNS41MEwxMjkuODggMjAuMTBMMTMxLjM4IDIwLjEwUTEzMi40NSAyMC4xMCAxMzMuMTEgMTkuNDlRMTMzLjc2IDE4Ljg4IDEzMy43NiAxNy44MEwxMzMuNzYgMTcuODBRMTMzLjc2IDE2LjcyIDEzMy4xMSAxNi4xMVExMzIuNDUgMTUuNTAgMTMxLjM4IDE1LjUwTDEzMS4zOCAxNS41MEwxMjkuODggMTUuNTBaTTEzOS44MSAyMC45M0wxMzkuODEgMjAuOTNMMTQxLjExIDE5LjQwUTE0MS43OCAyMC4yNyAxNDIuNTUgMjAuMjdMMTQyLjU1IDIwLjI3UTE0Mi41NiAyMC4yNyAxNDIuNTYgMjAuMjdMMTQyLjU2IDIwLjI3UTE0My4wOCAyMC4yNyAxNDMuMzUgMTkuOTZRMTQzLjYyIDE5LjY1IDE0My42MiAxOS4wNUwxNDMuNjIgMTkuMDVMMTQzLjYyIDE1LjQ0TDE0MC43MiAxNS40NEwxNDAuNzIgMTMuNjBMMTQ1Ljk3IDEzLjYwTDE0NS45NyAxOC45MVExNDUuOTcgMjAuNTQgMTQ1LjE1IDIxLjM2UTE0NC4zMyAyMi4xNyAxNDIuNzMgMjIuMTdMMTQyLjczIDIyLjE3UTE0MS44MSAyMi4xNyAxNDEuMDUgMjEuODVRMTQwLjI5IDIxLjUzIDEzOS44MSAyMC45M1pNMTUyLjQ4IDIyTDE1MC4wNSAyMkwxNTMuNzYgMTMuNjBMMTU2LjEwIDEzLjYwTDE1OS44MiAyMkwxNTcuMzUgMjJMMTU2LjY5IDIwLjM3TDE1My4xNCAyMC4zN0wxNTIuNDggMjJaTTE1NC45MSAxNS45M0wxNTMuODMgMTguNjFMMTU1Ljk5IDE4LjYxTDE1NC45MSAxNS45M1pNMTY2LjMwIDIyTDE2My45NyAyMkwxNjMuOTcgMTMuNjBMMTY1LjkzIDEzLjYwTDE2OS42NCAxOC4wN0wxNjkuNjQgMTMuNjBMMTcxLjk2IDEzLjYwTDE3MS45NiAyMkwxNzAuMDEgMjJMMTY2LjMwIDE3LjUyTDE2Ni4zMCAyMlpNMTc2LjcwIDE3LjgwTDE3Ni43MCAxNy44MFExNzYuNzAgMTYuNTQgMTc3LjMwIDE1LjU0UTE3Ny44OSAxNC41NSAxNzguOTYgMTMuOTlRMTgwLjAzIDEzLjQzIDE4MS4zNyAxMy40M0wxODEuMzcgMTMuNDNRMTgyLjU1IDEzLjQzIDE4My40OSAxMy44M1ExODQuNDMgMTQuMjIgMTg1LjA1IDE0Ljk3TDE4NS4wNSAxNC45N0wxODMuNTQgMTYuMzNRMTgyLjY5IDE1LjQwIDE4MS41MiAxNS40MEwxODEuNTIgMTUuNDBRMTgxLjUwIDE1LjQwIDE4MS41MCAxNS40MEwxODEuNTAgMTUuNDBRMTgwLjQyIDE1LjQwIDE3OS43NiAxNi4wNlExNzkuMTAgMTYuNzEgMTc5LjEwIDE3LjgwTDE3OS4xMCAxNy44MFExNzkuMTAgMTguNTAgMTc5LjQwIDE5LjA0UTE3OS43MCAxOS41OSAxODAuMjQgMTkuODlRMTgwLjc4IDIwLjIwIDE4MS40NyAyMC4yMEwxODEuNDcgMjAuMjBRMTgyLjE2IDIwLjIwIDE4Mi43NiAxOS45M0wxODIuNzYgMTkuOTNMMTgyLjc2IDE3LjYyTDE4NC44NiAxNy42MkwxODQuODYgMjEuMTBRMTg0LjEzIDIxLjYxIDE4My4yMCAyMS44OVExODIuMjcgMjIuMTcgMTgxLjMzIDIyLjE3TDE4MS4zMyAyMi4xN1ExODAuMDEgMjIuMTcgMTc4Ljk1IDIxLjYxUTE3Ny44OSAyMS4wNSAxNzcuMzAgMjAuMDVRMTc2LjcwIDE5LjA2IDE3Ni43MCAxNy44MFpNMTg5LjQyIDE3LjgwTDE4OS40MiAxNy44MFExODkuNDIgMTYuNTUgMTkwLjAyIDE1LjU1UTE5MC42MyAxNC41NiAxOTEuNjkgMTQuMDBRMTkyLjc1IDEzLjQzIDE5NC4wOCAxMy40M0wxOTQuMDggMTMuNDNRMTk1LjQxIDEzLjQzIDE5Ni40OCAxNC4wMFExOTcuNTQgMTQuNTYgMTk4LjE1IDE1LjU1UTE5OC43NSAxNi41NSAxOTguNzUgMTcuODBMMTk4Ljc1IDE3LjgwUTE5OC43NSAxOS4wNSAxOTguMTUgMjAuMDRRMTk3LjU0IDIxLjA0IDE5Ni40OCAyMS42MFExOTUuNDIgMjIuMTcgMTk0LjA4IDIyLjE3TDE5NC4wOCAyMi4xN1ExOTIuNzUgMjIuMTcgMTkxLjY5IDIxLjYwUTE5MC42MyAyMS4wNCAxOTAuMDIgMjAuMDRRMTg5LjQyIDE5LjA1IDE4OS40MiAxNy44MFpNMTkxLjgyIDE3LjgwTDE5MS44MiAxNy44MFExOTEuODIgMTguNTEgMTkyLjEyIDE5LjA1UTE5Mi40MiAxOS42MCAxOTIuOTQgMTkuOTBRMTkzLjQ1IDIwLjIwIDE5NC4wOCAyMC4yMEwxOTQuMDggMjAuMjBRMTk0LjcyIDIwLjIwIDE5NS4yNCAxOS45MFExOTUuNzUgMTkuNjAgMTk2LjA1IDE5LjA1UTE5Ni4zNSAxOC41MSAxOTYuMzUgMTcuODBMMTk2LjM1IDE3LjgwUTE5Ni4zNSAxNy4wOSAxOTYuMDUgMTYuNTRRMTk1Ljc1IDE2IDE5NS4yNCAxNS43MFExOTQuNzIgMTUuNDAgMTk0LjA4IDE1LjQwTDE5NC4wOCAxNS40MFExOTMuNDUgMTUuNDAgMTkyLjkzIDE1LjcwUTE5Mi40MiAxNiAxOTIuMTIgMTYuNTRRMTkxLjgyIDE3LjA5IDE5MS44MiAxNy44MFoiIGZpbGw9IiNGRkZGRkYiIHg9IjEyNi4zMSIvPjwvc3ZnPg==)](https://forthebadge.com)

A small real time chat application built using Django. It also uses Channels and Vanilla Javascript with Web Sockets.

![](Demo.gif)


## Architecture ##
 - When a user logs in, the frontend downloads the room list and opens a Websocket connection to the server.
 - When a user selects another user to chat, the frontend downloads the latest 25 messages (see [Line #13 in views.py](room/views.py)) they've exchanged.
 - When a user sends a message, the frontend sends a POST to the framework, then Django saves the message and will be displayed for every user.

## Scaling ##

> Because Channels takes Django into a multi-process model, you no longer run everything in one process along with a WSGI server (of course, you’re still free to do that if you don’t want to use Channels). Instead, you run one or more interface servers, and one or more worker servers, connected by that channel layer you configured earlier.

In this case, I'm using the In-Memory channel system, but could be changed to the Redis backend to improve performance.

Please take a look at this [link](https://channels.readthedocs.io/en/latest/introduction.html) below for more information.

### Database ###
For this demo, I'm using a simple SQLite setup.

## Future Work ##
Because of time constraints this project lacks of:

- User Selector Pagination
- Good Test Coverage
- Better Comments / Documentation Strings
- Frontend Tests
- Backend Tests
- Modern Frontend Framework (like React)
- Frontend Package (automatic lintin, building and minification)
- Proper UX / UI design (looks plain bootstrap)

## Run ##

1. Move to the project root folder.

2. Create and activate a virtual environment.
```bash
virtualenv env
source env/bin/activate
```
> (for mac)

To deactivate the environment
```bash
deactivate
```

3. Install requirements

```bash
pip3 install -r requirements.txt
```

4. Initialize database
```bash
python3 manage.py migrate
```

5. Create admin user
```bash
python3 manage.py createsuperuser
```

6. Run development server
```bash
python3 manage.py runserver
```

## Directory Layout

```bash
📦djangochat
 ┣ 📂core
 ┃ ┣ 📂static
 ┃ ┃ ┣ 📂images
 ┃ ┃ ┃ ┗ 📜favicon.ico
 ┃ ┣ 📂templates
 ┃ ┃ ┣ 📂core
 ┃ ┃ ┃ ┣ 📜base.html
 ┃ ┃ ┃ ┣ 📜frontpage.html
 ┃ ┃ ┃ ┣ 📜login.html
 ┃ ┃ ┃ ┗ 📜signup.html
 ┃ ┣ 📜admin.py
 ┃ ┣ 📜apps.py
 ┃ ┣ 📜forms.py
 ┃ ┣ 📜models.py
 ┃ ┣ 📜tests.py
 ┃ ┣ 📜urls.py
 ┃ ┗ 📜views.py
 ┣ 📂djangochat
 ┃ ┣ 📜asgi.py
 ┃ ┣ 📜settings.py
 ┃ ┣ 📜urls.py
 ┃ ┗ 📜wsgi.py
 ┣ 📂room
 ┃ ┣ 📂templates
 ┃ ┃ ┣ 📂room
 ┃ ┃ ┃ ┣ 📜room.html
 ┃ ┃ ┃ ┗ 📜rooms.html
 ┃ ┣ 📜admin.py
 ┃ ┣ 📜apps.py
 ┃ ┣ 📜consumers.py
 ┃ ┣ 📜models.py
 ┃ ┣ 📜routing.py
 ┃ ┣ 📜tests.py
 ┃ ┣ 📜urls.py
 ┃ ┗ 📜views.py
 ┣ 📜db.sqlite3
 ┣ 📜manage.py
 ```
