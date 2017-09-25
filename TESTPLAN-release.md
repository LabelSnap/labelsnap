# Labelsnap Release Testplan
### style / responsiveness pass
Verify:
- [ ] site does not appear broken on any page at various screen sizes

### free address return labels
1. not logged in create address return labels
2. click download on the preview page
3. register

Verify:
- [ ] registration works
- [ ] you are presented with a link to download your free address labels

### subscription purchase / redemption
1. choose subscription pricing
2. create some labels and go to checkout

Verify:
- [ ] you see at checkout that you are purchasing a subscription
- [ ] upon going back to the pricing page post-checkout you see the subscription pricing options
- [ ] you see that you have a license in your my account page

### subscription redemption
1. Buy a subscription and then create a new label group

Verify:
- [ ] checkout has been replaced by download on the preview page 
- [ ] upon going back to the pricing page post-checkout you see the subscription pricing options


### user creation and login / logout
1. Create a new user. 
2. Logout

Verify
- [ ] you are logged in after creating the new user
- [ ] you are correctly logged out when clicking logout
- [ ] logging back in works as expected

### label creation / order flow as anon user / upgrade flow
1. Start the label creation flow logged out
2. Do not log in or insert during label creation
3. Provide an email address at checkout

Verify:
- [ ] you receive an order confirmation email
- [ ] your order confirmation email contains a link to upgrade to a real account
- [ ] this form shows an error if your passwords do not match
- [ ] when successful you can logout / log back in as this user and see your order in your history
- [ ] you receive a welcome email

### label creation / order flow as new user
1. Start the label creation flow logged out
2. Once on the preview page click insert labels and create a new account

Verify:
- [ ] you receive an order email
- [ ] you can log out / log back in and see your order history

### label creation / order flow as pre-existing user
1. Create a new account and stay logged in
2. Start the label creation flow and purchase labels
3. Log out of this accountnt
4. Start another label creation flow
5. Log into the pre-existing account and finish

### label creation via upload
1. Create a new account and stay logged in.
2. Create a new label group via uploading. 

Verify:
- [ ] verify template link
- [ ] verify upload fails with bad sheet
- [ ] verify upload succeeds with good sheet
- [ ] verify upload succeeds after trying again after bad sheet

### label creation via copy / paste
1. Create a new account and stay logged in
2. Create a new label group via copy / paste

Verify:
- [ ] form submit is disabled if empty
- [ ] pasting addresses creates labels

### label creation manual
1. Create a new account and stay logged in
2. Create a new label group manually

Verify:
- [ ] preview page loads empty

### updating password
1. create a new user
2. go to my account
3. update password

Verify:
- [ ] errors render properly if old password doesn't match
- [ ] errors render properly if new password doesn't match
- [ ] you can log out / log in with the new password

### updating email address
1. create a new user
2. go to my account
3. update email address

Verify:
- [ ] you get an error if no @ sign is in the email address
- [ ] upon changing the header of the page updates

### forgot password flow
Verify:
- [ ] forgot password form linked from sign in
- [ ] you receive an email which contains a link to a reset password page
- [ ] you can reset your password and log in

### home page / header
Verify:
- [ ] links in header work
- [ ] pricing link in body goes to pricing page
- [ ] links in footer work
- [ ] get started links work

### pricing page
Verify:
- [ ] prices look sane
- [ ] get started link works
- [ ] contact us link works
- [ ] faq snippet works

### faq page
Verify:
- [ ] smoke test expand / collapse
- [ ] link to pricing page works
- [ ] support link works

### preview page settings
Verify:
- [ ] changing typeface works
- [ ] changing weight works
- [ ] changing size works
- [ ] alignment works
- [ ] changing label size works
- [ ] can progress through next and previous search results
- [ ] can clear search
- [ ] can scroll to view additional sheets
- [ ] scroll buttons appear on hover and work
- [ ] zoom controls work
- [ ] undo and redo controls work

### preview page - correction flow
Verify:
- [ ] corrections and counts appear correctly in the right column
- [ ] suggestions appear correctly in modal
- [ ] suggestions disappear and count reduces once corrected
- [ ] previous, next and done buttons in modal work correctly
- [ ] label highlights appear and disappear correctly

### preview page - add / delete
Verify:
- [ ] can add a label manually
- [ ] can manually select / delete a label

### my labels
Verify:
- [ ] see empty list from a new account with a link to create labels
- [ ] for completed orders see link to download and link to edit
- [ ] for in progress orders only see a link to edit

### preview page - edit  past order
1. Order labels and go to my account
2. Click the edit link

Verify:
- [ ] secure checkout is replaced by download link
- [ ] clicking download downloads the new order

### checkout page
Verify:
- [ ] validation errors for each field work correctly
- [ ] submit button only becomes active when all fields are filled out
- [ ] information on the right is accurate and displays correctly
- [ ] checkout form submits successfully and taken to download page and receive purchase confirmation email

### download page
Verify:
- [ ] download link works correctly
- [ ] PDF opens in the browser and appears correctly
