# How to Set Up Instagram Basic Display

## Prerequisites

- Must have an app (with type "consumer") created under a [Meta Developers](https://developers.facebook.com/) account
- Must have "Instagram Basic Display" product under app (Only available on app with type "consumer")

## Guide

1. Navigate to developers.facebook.com
	- Select the app

2. Locate left navigation side menu
	- Click the “Roles” button to open the dropdown
	- Click the “roles” button from the dropdown

3. Scroll down to “Instagram Testers”
	- Click “Add Instagram Testers”
	- Enter a username of the Instagram account that should be displayed into the web app

4. Log in to the Instagram account
	- Navigate to: https://www.instagram.com/accounts/manage_access/ 
	- Click the “Tester Invites” tab and accept

5. Navigate back to developers.facebook.com

6. Locate left navigation side menu
	- Click the “Instagram Basic Display” button to open the dropdown
	- Click the “Basic Display” button from the dropdown

7. Scroll down to “User Token Generator”
	- Click “Generate Token” on the user that you added

8. Click Pop-up window
	- Login with credentials

9. Use token in web app

## Keep In Mind

### Default Method

The Instagram tokens must be renewed by making a request to the following:

https://graph.instagram.com/refresh_access_token?grant_type=ig_refresh_token&access_token=${access_token}

replace "${access_token}" with actual access token.

### Alternative Method

Set up a Instagram auto token refresher using something like [instagram-token-agent](https://github.com/companionstudio/instagram-token-agent)

