# springsecurity-secureauthserver
A Simple OAuth Sever based on Spring Security

Do a post call to the endpoint to get the token

curl --location --request POST 'localhost:9000/oauth/token' \
--header 'Authorization: Bearer 94533ceef2f866f32521c7d9b7f49f756479c6e5' \
--header 'Authorization: Basic cGx1cmFsc2lnaHQ6cGx1cmFsc2lnaHRzZWNyZXQ=' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'client_id=pluralsight' \
--data-urlencode 'username=user1' \
--data-urlencode 'password=pass1'



Use BAsic auth and use clienntID:slicnetsecret pair
security.oauth2.client.clientId: pluralsight
security.oauth2.client.clientSecret: pluralsightsecret

In the body use 
grant_type=password
client_id=pluralsight
username=user1
password=pass1
