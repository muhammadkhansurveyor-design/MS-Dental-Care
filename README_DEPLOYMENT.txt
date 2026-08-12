MS Dental Care Cloud - Final Production Package

WHAT IS INCLUDED
- Secure email/password login
- Roles: Super Admin, Branch Admin, Entry User, Viewer
- Branch-level data isolation
- Patients + search + edit
- Medical history
- Visit history
- Doctor and treatment selection
- X-Ray/image upload
- Billing, discount, received, balance
- Additional payments against old invoices
- Credit patient report
- Expenses
- Doctors
- Staff
- Salaries / advance / balance
- Treatment price master
- Activity log
- Dashboard
- Charts: treatment revenue, doctor revenue, monthly collection
- CSV export
- SQLite backup for local mode
- PostgreSQL support for cloud mode
- Docker deployment files

DEFAULT LOGIN (CHANGE AFTER FIRST LOGIN)
Email: admin@msdental.local
Password: 1234

LOCAL TEST
1. Install Python 3.12+
2. pip install -r requirements.txt
3. python app.py
4. Open http://127.0.0.1:5000

CLOUD LIVE USE
For Pakistan entry + Saudi live view:
1. Create a low-cost Python web host account.
2. Create a PostgreSQL database.
3. Upload/deploy this project.
4. Set environment variables:
   SECRET_KEY=<long random string>
   DATABASE_URL=<PostgreSQL connection string>
5. Start command:
   gunicorn app:app
6. Open the public HTTPS link.
7. Login as Super Admin and immediately create your real Super Admin user / change credentials.
8. Add branches, doctors, staff, treatment prices, and users.
9. Assign each non-super user to exactly one branch.

IMPORTANT
Cloud hosting itself requires an account with a hosting provider. This package is fully prepared, but the final deployment click/account creation must be done using your hosting account credentials.

LOW-COST RECOMMENDATION
Use a basic Python hosting plan + managed PostgreSQL. Start without a custom domain; use the host's HTTPS URL. Add a domain later only if needed.
