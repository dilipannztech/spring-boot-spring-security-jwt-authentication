step 1:
INSERT INTO roles(name) VALUES('ROLE_USER');
INSERT INTO roles(name) VALUES('ROLE_MODERATOR');
INSERT INTO roles(name) VALUES('ROLE_ADMIN');

step 2:

http://localhost:8080/api/auth/signup

request
{
"username": "mod_usernmae",
"email": "mod@ssw",
"password": "your_password",
"role": [
"user"
]
}

step 3:
http://localhost:8080/api/auth/signin

request
{
"username": "mod_usernmae",
"password": "your_password"
}
