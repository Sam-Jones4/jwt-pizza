# Learning notes

## JWT Pizza code study and debugging

As part of `Deliverable ⓵ Development deployment: JWT Pizza`, start up the application and debug through the code until you understand how it works. During the learning process fill out the following required pieces of information in order to demonstrate that you have successfully completed the deliverable.

| User activity                                       | Frontend component | Backend endpoints | Database SQL |
| --------------------------------------------------- | ------------------ | ----------------- | ------------ |
| View home page                                      |   home.jsx         |      none         |    none      |
| Register new user<br/>(t@jwt.com, pw: test)         |   register.jsx     |  [POST] /api/auth | INSERT INTO user (name, email,password) VALUES (?, ?, ?)
                                                                                                 INSERT INTO userRole (userId, role, objectId) VALUES (?, ?, ?)
| Login new user<br/>(t@jwt.com, pw: test)            |     login.tsx      |  [PUT]/api/auth   | SELECT * FROM user WHERE email=?
                                                                                                 SELECT * FROM userRole WHERE userId=? |
| Order pizza                                         |     menu.tsx       |                   |              |
| Verify pizza                                        |                    |                   |              |
| View profile page                                   | dinerDashboard.tsx |      none         |    none      |
| View franchise<br/>(as diner)                       |                    |                   |              |
| Logout                                              |    logout.tsx      |                   |              |
| View About page                                     |                    |                   |     none     |
| View History page                                   |                    |                   |     none     |
| Login as franchisee<br/>(f@jwt.com, pw: franchisee) |                    |                   |              |
| View franchise<br/>(as franchisee)                  |                    |                   |      none    |
| Create a store                                      |                    |                   |              |
| Close a store                                       |                    |                   |              |
| Login as admin<br/>(a@jwt.com, pw: admin)           |                    |                   |              |
| View Admin page                                     | adminDashboard.tsx |                   |    none      |
| Create a franchise for t@jwt.com                    |createFranchise.tsx |                   |              |
| Close the franchise for t@jwt.com                   | closeFranchise.tsx |                   |              |
