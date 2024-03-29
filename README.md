# Spotify scraper for R

## Interacting with the Spotify API 

### Obtaining the credentials. 

The first necessary conditions for obtaining the credentials for using the Spotify Web API is having a valid account for the [application](https://www.spotify.com). 

As a next step, we need to register an app in [Spotify for Developers](https://developer.spotify.com/dashboard/login). As you already should have a valid user and password for Spotify, you should log in with that Spotify Account and then click in the _create an app_ button. For a valid app, only a name and a description is necessary (as well as accepting Spotify's developer terms). The purpose of creating this app is obtaining two central things: the _client ID_ and the _client secret_.

These _client ID_ and the _client secret_ are the credentials needed to obtain the OAth 2.0 token, in order to interact with the API. Again, in the dashboard tab, we find the _client ID_ at the left of the screen; below the name and the description. In order to see the secret, we have to click in _show client secret_. Finally, the token is obtained via a POST request to the API itself (detailed in the FinalRMD). 

The final step is to create two _.txt_ documents outside the folder of the repository, named: 
- client_id.txt (Containing only the _Client ID_). 
- client_secret.txt (Contaning only the _Client secret_). 
They should only include the respective information for each one, and nothing else. 

Note: for an easier and quicker access to the API, place these into an easy directory, as you will later need to link them to the .Rmd. 

Once this is done, just paste the directories in the chunks in lines 51 and 55, and the 'Spotify scraper.Rmd' will be ready to run, so that you can easily scrape Spotify's information. 

### Summary

Thus, the process can be summarised in: 

1. Creating a Spotify account. 
2. Loging in in Registering an app in [Spotify for Developers](https://developer.spotify.com/dashboard/login).
3. Obtaining the _Client ID_ and _Client secret_ and storing them in two separate .txt files, in the specified format.
4. Link these two .txt to the .Rmd document, sepcifying where they're located.
5. Run the code. 
 

