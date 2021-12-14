| User should be able to . . .                                                         |             |
| :----------------------------------------------------------------------------------- | ----------: |
| Visit the deployed pages on GitHub pages, with link in the About section of the Github repo|        1 |

| Events  `                                                                            |             |
| :----------------------------------------------------------------------------------- | ----------: |
| On the home page (`'/'`), Login and Signup using the login and signup form. On success, redirect to the `/polls` page   |        2 |
| Logout by clicking the logout button                                                       |        1 |
| If a non-logged-in user tries to visit the polls page, redirect them to the login page | 1 |
| On the polls page load, see a form and empty current poll div                              |        2 |
| On the polls page load, fetch all past polls and render them to the past polls div         |        2 |
| On submit, add the poll options and question to the current poll div                                      |        1 |
| On clicking add or subtract, increment and decrement the correct score in the current poll div|     1 |
| On clicking finish, empty the current poll div, and use supabase to add the current poll to the database. |1|
| On clicking finish, clear the past polls div, then fetch all past polls from supabase and render them in the past polls div. |2|

| Functions                                                              |             |
| :----------------------------------------------------------------------------------- | ----------: |
| IMPURE: `displayCurrentPollEl()` : displays the form state to the current poll DOM element | 1|
| IMPURE: `displayAllPolls()` : clears out and appends to polls div | 1|
| PURE with TDD: `renderPoll(poll)` : returns DOM node | 1|
| ASYNC: `createPoll(poll)` : creates a poll for currently logged in user in supabase |1|
| ASYNC: `getPolls()` : returns polls for currently logged in user from supabase |1|
