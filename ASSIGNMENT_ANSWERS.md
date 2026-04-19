# Capstone Project Assignment Answers
## GitHub Repository: https://github.com/SiRipo92/Fullstack_Dev_Capstone_Project

---

## IMPLEMENTATION STATUS CHECKLIST

| Task | Description | Status |
|------|-------------|--------|
| 1 | README.md with project name | ✅ DONE |
| 2 | Django server terminal output (file: django_server) | ⚠️ FILE NEEDS CREATION |
| 3 | About.html with CSS, images, names, roles, emails | ✅ DONE |
| 4 | Contact.html with CSS, navbar, images, contact details | ✅ DONE |
| 5 | cURL login command output (file: loginuser) | ⚠️ FILE NEEDS CREATION |
| 6 | cURL logout command output (file: logoutuser) | ⚠️ FILE NEEDS CREATION |
| 7 | Register.jsx with 5 input fields + Register button | ✅ DONE |
| 8 | cURL dealer reviews output (file: getdealerreviews) | ⚠️ FILE NEEDS CREATION |
| 9 | cURL all dealers output (file: getalldealers) | ⚠️ FILE NEEDS CREATION |
| 10 | cURL dealer by ID output (file: getdealerbyid) | ⚠️ FILE NEEDS CREATION |
| 11 | cURL dealers by Kansas output (file: getdealersbyState) | ⚠️ FILE NEEDS CREATION |
| 12 | Screenshot admin login (admin_login.png) | ⚠️ SCREENSHOT NEEDED |
| 13 | Screenshot admin logout (admin_logout.png) | ⚠️ SCREENSHOT NEEDED |
| 14+15 | cURL all car makes/models (file: getallcarmakes) | ⚠️ FILE NEEDS CREATION |
| 16 | cURL sentiment analysis (file: analyzereview) | ⚠️ FILE NEEDS CREATION |
| 17 | Screenshot home page before login (get_dealers.png) | ⚠️ SCREENSHOT NEEDED |
| 18 | Screenshot home page logged in (get_dealers_loggedin.png) | ⚠️ SCREENSHOT NEEDED |
| 19 | Screenshot dealers by state (dealersbystate.png) | ⚠️ SCREENSHOT NEEDED |
| 20 | Screenshot dealer detail + reviews (dealer_id_reviews.png) | ⚠️ SCREENSHOT NEEDED |
| 21 | Screenshot post review page (dealership_review_submission.png) | ⚠️ SCREENSHOT NEEDED |
| 22 | Screenshot added review (added_review.png) | ⚠️ SCREENSHOT NEEDED |
| 23 | GitHub Actions workflow output (file: CICD) | ⚠️ FILE NEEDS CREATION |
| 24 | Deployment URL (file: deploymentURL) | ⚠️ FILE NEEDS CREATION |
| 25 | Screenshot deployed landing page (deployed_landingpage.png) | ⚠️ SCREENSHOT NEEDED |
| 26 | Screenshot deployed logged-in (deployed_loggedin.png) | ⚠️ SCREENSHOT NEEDED |
| 27 | Screenshot deployed dealer detail (deployed_dealer_detail.png) | ⚠️ SCREENSHOT NEEDED |
| 28 | Screenshot deployed add review (deployed_add_review.png) | ⚠️ SCREENSHOT NEEDED |

---

## TASK ANSWERS

### Task 1 (1 point) — README.md GitHub URL
**Answer:**
```
https://github.com/SiRipo92/Fullstack_Dev_Capstone_Project/blob/main/README.md
```

### Task 2 (1 point) — Django Server Terminal Output
**What to submit:** Contents of file named `django_server`
**How to generate:**
1. Start the Django server: `cd server && python manage.py runserver`
2. Copy the terminal output into a file named `django_server`

**Expected output looks like:**
```
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
April 20, 2026 - 10:00:00
Django version 3.2.x, using settings 'djangoproj.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.
```
**File location to submit:** `server/django_server` (contents of the file named `django_server`)

---

### Task 3 (3 points) — About.html GitHub URL
**Answer:**
```
https://github.com/SiRipo92/Fullstack_Dev_Capstone_Project/blob/main/server/frontend/static/About.html
```
**What's implemented:** CSS links to bootstrap.min.css and style.css, 3 team members (Benjamin Carter, Emily Johnson, Donald Draper) with person1.png/person2.png/person3.png images, roles, descriptions, and email IDs.

---

### Task 4 (2 points) — Contact.html GitHub URL
**Answer:**
```
https://github.com/SiRipo92/Fullstack_Dev_Capstone_Project/blob/main/server/frontend/static/Contact.html
```
**What's implemented:** CSS links, navbar with "Contact Us" as active item, car_dealership.jpg image, contact emails and phone for Customer Service, National Advertising, PR, and office contact.

---

### Task 5 (2 points) — cURL Login Command Output
**What to submit:** Contents of file named `loginuser`
**Command to run (with Django server running on port 8000):**
```bash
curl -v -c cookies.txt -X POST http://localhost:8000/djangoapp/login \
  -H "Content-Type: application/json" \
  -d '{"userName": "testuser", "password": "testpassword123"}'
```
**Save output to file named `loginuser`**

---

### Task 6 (2 points) — cURL Logout Command Output
**What to submit:** Contents of file named `logoutuser`
**Command to run:**
```bash
curl -v -b cookies.txt -X POST http://localhost:8000/djangoapp/logout/ \
  -H "Content-Type: application/json"
```
**Save output to file named `logoutuser`**

---

### Task 7 (1 point) — Register.jsx GitHub URL
**Answer:**
```
https://github.com/SiRipo92/Fullstack_Dev_Capstone_Project/blob/main/server/frontend/src/components/Register/Register.jsx
```
**What's implemented:** 5 input fields — Username, First Name, Last Name, Email, Password — plus Register (Submit) button. All with state management via React hooks.

---

### Task 8 (2 points) — cURL Dealer Reviews Output
**What to submit:** Contents of file named `getdealerreviews`
**Command to run (Django server + Node backend running):**
```bash
curl -v http://localhost:8000/djangoapp/reviews/dealer/1
```
**Save output to file named `getdealerreviews`**

---

### Task 9 (2 points) — cURL All Dealers Output
**What to submit:** Contents of file named `getalldealers`
**Command to run:**
```bash
curl -v http://localhost:8000/djangoapp/get_dealers/
```
**Save output to file named `getalldealers`**

---

### Task 10 (2 points) — cURL Dealer By ID Output
**What to submit:** Contents of file named `getdealerbyid`
**Command to run:**
```bash
curl -v http://localhost:8000/djangoapp/dealer/1
```
**Save output to file named `getdealerbyid`**

---

### Task 11 (2 points) — cURL Dealers by State (Kansas) Output
**What to submit:** Contents of file named `getdealersbyState`
**Command to run:**
```bash
curl -v "http://localhost:8000/djangoapp/get_dealers/Kansas"
```
**Save output to file named `getdealersbyState`**

---

### Task 12 (2 points) — Admin Login Screenshot
**What to submit:** File named `admin_login.png` or `admin_login.jpeg`
**Steps:**
1. Start Django server
2. Navigate to http://localhost:8000/admin/
3. Log in with superuser credentials (root/root or admin you created)
4. Take a screenshot showing the login page OR the logged-in admin panel
5. Save as `admin_login.png`

---

### Task 13 (1 point) — Admin Logout Screenshot
**What to submit:** File named `admin_logout.png` or `admin_logout.jpeg`
**Steps:**
1. While logged into admin, click "LOG OUT"
2. Take a screenshot of the logged-out confirmation page
3. Save as `admin_logout.png`

---

### Tasks 14 & 15 (4 points) — cURL All Car Makes/Models Output
**What to submit:** Contents of file named `getallcarmakes`
**Command to run (Django server running, DB populated):**
```bash
curl -v http://localhost:8000/djangoapp/get_cars
```
**Expected output includes:** Nissan, Mercedes, Audi, Kia, Toyota makes with their models
**Save output to file named `getallcarmakes`**

---

### Task 16 (2 points) — cURL Sentiment Analysis Output
**What to submit:** Contents of file named `analyzereview`
**Sentiment Analyzer URL (from .env):** https://sentianalyzer.1qgxvy3nypne.us-south.codeengine.appdomain.cloud
**Command to run:**
```bash
curl -v "https://sentianalyzer.1qgxvy3nypne.us-south.codeengine.appdomain.cloud/analyze/Fantastic%20services"
```
**Expected output:**
```json
{"sentiment": "positive"}
```
**Save output to file named `analyzereview`**

---

### Task 17 (1 point) — Dealers Home Page (Before Login) Screenshot
**What to submit:** File named `get_dealers.png` or `get_dealers.jpeg`
**Steps:**
1. Start Django server (and Node backend)
2. Open http://localhost:8000/ in browser (not logged in)
3. Take a screenshot showing the dealer list
4. The browser address bar must show the endpoint
5. Save as `get_dealers.png`

---

### Task 18 (2 points) — Dealers Home Page (After Login) Screenshot
**What to submit:** File named `get_dealers_loggedin.png` or `get_dealers_loggedin.jpeg`
**Steps:**
1. Log in with a valid user
2. Navigate to home page showing dealers
3. Screenshot must show: "Review Dealer" option, logged-in username, and endpoint in browser address bar
4. Save as `get_dealers_loggedin.png`

---

### Task 19 (2 points) — Dealers Filtered by State Screenshot
**What to submit:** File named `dealersbystate.png` or `dealersbystate.jpeg`
**Steps:**
1. On home page, filter dealers by a state (e.g., Kansas)
2. The browser address bar must show the state endpoint
3. Save screenshot as `dealersbystate.png`

---

### Task 20 (1 point) — Dealer Detail + Reviews Screenshot
**What to submit:** File named `dealer_id_reviews.png` or `dealer_id_reviews.jpeg`
**Steps:**
1. Click on any dealer to view their detail page
2. Page should show dealer details + reviews
3. Browser address bar must show the endpoint (e.g., /dealer/1)
4. Save as `dealer_id_reviews.png`

---

### Task 21 (1 point) — Post Review Page Screenshot
**What to submit:** File named `dealership_review_submission.png`
**Steps:**
1. Log in and navigate to a dealer's page
2. Click "Review Dealer" to open the review form
3. Fill in review details but DON'T submit yet
4. Take screenshot showing the filled form
5. Save as `dealership_review_submission.png`

---

### Task 22 (2 points) — Added Review Screenshot
**What to submit:** File named `added_review.png`
**Steps:**
1. Submit the review form
2. Take a screenshot showing the newly posted review appearing on the dealer page
3. Save as `added_review.png`

---

### Task 23 (3 points) — GitHub Actions CI/CD Workflow Output
**What to submit:** Contents of file named `CICD`
**How to get:**
1. Go to: https://github.com/SiRipo92/Fullstack_Dev_Capstone_Project/actions
2. Click on a completed workflow run
3. Expand the steps and copy the terminal output
4. OR: push a commit, wait for workflow to run, then copy output
5. Save to file named `CICD`

**The workflow (.github/workflows/main.yml) runs:**
- Lint Python files with flake8
- Lint JavaScript files with JSHint

---

### Task 24 (1 point) — Deployment URL
**What to submit:** Contents of file named `deploymentURL`
**Note:** The sentiment analyzer is deployed at:
```
https://sentianalyzer.1qgxvy3nypne.us-south.codeengine.appdomain.cloud
```
The Node.js backend is deployed at:
```
https://ripochesierr-3030.theiadockernext-1-labs-prod-theiak8s-4-tor01.proxy.cognitiveclass.ai
```
**For Task 24, the Django application deployment URL is needed** — deploy the Django app on IBM Cloud Code Engine or similar, then save the URL to a file named `deploymentURL`.

---

### Tasks 25–28 — Deployed Application Screenshots
**What to submit:** Screenshots from your deployed Django app URL

- **Task 25:** `deployed_landingpage.png` — Home page at deployment URL
- **Task 26:** `deployed_loggedin.png` — Home page logged in (show username + address bar)
- **Task 27:** `deployed_dealer_detail.png` — Dealer detail page through deployment URL
- **Task 28:** `deployed_add_review.png` — Review posted/displayed in deployed app

---

## HOW TO START THE SERVERS (Quick Reference)

```bash
# Terminal 1 - Start Node.js + MongoDB backend
cd server/database
docker-compose up

# Terminal 2 - Start Django server
cd server
pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py runserver

# Terminal 3 - (Optional) Start sentiment analyzer locally
cd server/djangoapp/microservices
pip install flask nltk
python app.py
```

## BASE URL FOR cURL COMMANDS
- Django (local): http://localhost:8000
- Node backend (deployed): https://ripochesierr-3030.theiadockernext-1-labs-prod-theiak8s-4-tor01.proxy.cognitiveclass.ai
- Sentiment analyzer: https://sentianalyzer.1qgxvy3nypne.us-south.codeengine.appdomain.cloud
