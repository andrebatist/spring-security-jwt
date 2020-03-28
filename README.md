https://www.youtube.com/watch?v=X80nJ5T7YpE&list=PLqq-6Pq4lTTYTEooakHchTGglSvkZAjnE&index=12

POST 

http://localhost:8080/authenticate

Body raw JSON 
{
	"username": "foo",
	"password": "foo"
}

response 

{
  "jwt": "eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJmb28iLCJleHAiOjE1ODU0NDAzOTQsImlhdCI6MTU4NTQwNDM5NH0.25geTPkG_XyffsI-fZ1-qiXBQN0Km8R6sxY6iPgztOU"
}

---------------------------

GET 

http://localhost:8080/hello

Headers 

Content-Type application/json

Authorization Bearer  eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJmb28iLCJleHAiOjE1ODU0NDAzOTQsImlhdCI6MTU4NTQwNDM5NH0.25geTPkG_XyffsI-fZ1-qiXBQN0Km8R6sxY6iPgztOU

response

Hello world
