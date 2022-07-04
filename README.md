### Source structure ###
```
├── api
│   └── server.go
├── config.env
├── database
│   ├── gorm
│   ├── migration
│   ├── mock
│   └── util
│       ├── config.go
│       └── password.go
├── go.mod
├── main.go
├── Makefile
├── readme.md
└── token
    ├── jwt_token.go
    └── payload.go
```


**Description** 

1. api
    - server.go :  config and setup all router 
    - ...       :  solve logic and error with http status for all api
2. database
    - gorm      : folder for code with solving query and call data from database
    - migration : folder saving the version of database to update and backup 
    - mock      : folder saving all file mock code for testing purposes
    - util      : folder for saving all file code envole with configuration(env_variable, symetric_key, etc...) and file solving function encrypt and decrypt password
3. token 
    - jwt_token.go  : file code for all funtion solving jwt token
    - payload.go    : file code for all function solving payload 
4. main.go      : file code for connecting to database and start server
5. Makefile     : file saving all command(CLI) during coding development
6. config.env   : file saving all environment variables and symetric key for encrypting and decrypting password, link for connecting to database, server address, duration of token ...
