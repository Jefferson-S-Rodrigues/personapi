# People Management System

This project is a small system for managing people in a company through a REST API, created with Spring Boot.


## Run Project

To run the project on the terminal, type the following command:

```shell script
mvn spring-boot:run 
```

After executing the above command, just open the following address and view the project execution:

```
http://localhost:8080/api/v1/people
```

#### Cloud

* [Cloud Project Link](https://personapi-dio-jsr.herokuapp.com/api/v1/people)

## Services

Uri | Method | Description | Request Stream | Response Stream | Status Code Returned
---|---|---|---|---|---
/people | GET | All people in the System | n/a | **Person** Collection | 200/404
/people/`{id}` | GET | Get specific **Person** | n/a | **Person** | 200/404
/people | POST | Create a new **Person** entity in the  system. | **Person** without `id` specified | **Person** | 201/404
/people/`{id}` | PUT | Modifies a **Person** resource | **Person** | n/a | 200/404
__/people/`{id}`__ | __DELETE__ | __Deletes a **Person** resource__ | __n/a__ | __n/a__ | __200/404__
