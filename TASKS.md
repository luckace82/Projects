# Milestones for Development

1. `Week 1-2`: Set up the project with Django, create models for ***User, Post, and Analytics***. Set up the database and configure user authentication.

2. `Week 3-4`: Implement OAuth integration for social media platforms. Fetch user data from Twitter, Instagram, and Facebook.

3. `Week 5-6`: Implement post creation, media upload, and scheduling. Allow users to create posts from the dashboard and share them on linked social media accounts.

4. `Week 7-8`: Add analytics and sentiment analysis. Show post engagement metrics and use AI for sentiment analysis of posts.

5. `Week 9-10`: Build the frontend using Bootstrap, make the dashboard responsive, and integrate real-time notifications.

6. `Week 11-12`: Test the platform thoroughly, fix any bugs, and deploy it on a cloud service like Heroku.


# Work Distribution

## Step 1: Member 1 sets up the foundation (Alone first)
- Create the Django project (`startproject`).
- Create the Django app (`startapp`).
- Setup database connection in `settings.py`.
- Install Django REST Framework (DRF) and add it to `INSTALLED_APPS`.
- Setup GitHub repo and push the initial empty project.

## Step 2: Split work cleanly

| Member |	Tasks	| Notes |  
| -------| -------- | ----- |
| Member 1 |	**User Authentication** <br> - Login/SignUp<br>- User View<br>- HTML templates (`login.html`, `signup.html`)| Owns `views.py`, `forms.py`, templates/auth/ <br>Stays away from models for now  |
| Member 2 |	**Post and Analytics MOdels** <br> - Create `Post` model<br>- Create `Analytics` model<br>- Register them in `admin.py`| Owns `models.py`, `admin.py` only<br>No touching of views or template yet |
## Step 3: Rules to Avoid Conflict
✅ One person edits models.py, admin.py.  
✅ One person edits views.py, urls.py, templates/.  
✅ Always pull before pushing.  
✅ Commit frequently with small, clear commits (e.g., "Added Post model", "Created login view").  
✅ Use separate feature branches:
- `feature/user-auth`
- `feature/post-analytics`

✅ Then create pull requests (PRs) and review each other's code before merging to main.

## 📌 Better Folder/Area Ownership

| Member	| Files/Folders to work on | 
| --------- | ------------------------ |
|Member 1	|`views.py`, `forms.py`,` urls.py`, templates/, static/|
|Member 2	|`models.py`, `admin.py`, migrations files (migrations/)|
