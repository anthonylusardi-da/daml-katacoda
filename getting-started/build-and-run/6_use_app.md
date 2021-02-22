[On the the UI tab](https://[[HOST_SUBDOMAIN]]-3000-[[KATACODA_HOST]].environments.katacoda.com) you should now see a login page. For simplicity of this app, there is no password or sign-up required.

Enter "Alice" in the box and click Log in.

> Note: Usernames are case sensitive.

You should see the main screen with two panels. One for the users you are following and one for your followers.

Follow "Bob" by typing their name in the text box and clicking on the Follow button in the top panel.

You’ll notice that the user you just started following appears in the Following panel. However they do not yet appear in the Network panel. This is because:

1. They have not signed up and are not parties on the ledger
2. They have not yet started following "Alice" back

This social network is similar to LinkedIn or a private Instagram, where by following someone (ie. "Bob"), you make your profile visible to him but not vice versa. Bob still needs to choose on whether or not you're allowed to see his profile.

To make this relationship reciprocal, logout from "Alice" and login as "Bob".

Now have Bob follow Alice by clicking the + sign next to Alice's name.

Once Bob starts following Alice both of them can now see each other in their Network. Try logging back in as Alice and you'll see Bob is now in her network. Then log back in as Bob and you'll see the same for him.

Play around more with the app at your leisure: create new users and start following more users. Observe when a user becomes visible to others - this will be important to understanding Daml’s privacy model later.

> Note: If you want to see the code within this `create-daml-app` project click on the IDE tab or [check it out on GitHub](https://github.com/digital-asset/daml/tree/master/templates/create-daml-app).
