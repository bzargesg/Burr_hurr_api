# [Burr_hurr_api](#burrhurrapi)
  - [Description](#description)
  - [Requests](#requests)
  - [Responses](#responses)
  - [Pagination](#pagination)
  - [Response Status Codes](#response-status-codes)
## Description
A Rest/Crud API for [Burr-Hurr](https://github.com/bzargesg/BurrHurr) and application designed to help model homebrewing recipes. 
## Requests
| Method | Action                        |
| ------ | ----------------------------- |
| GET    | Retrieves Resources           |
| POST   | Creates Resources             |
| PUT    | Changes or replaces resources |
| DELETE | Removes resources             |
## Responses
This API will return all data as a JSON object

## Pagination
Some endpoints will support paging and support both the offset and limit as query parameters. Offset is 0 based.
```
http://api.burrhurr.com/v1/fermentables?offset=20&limit=10
```
## Response Status Codes
| Status Code | Description                                                               |
| ----------- | ------------------------------------------------------------------------- |
| 200         | OK- request succesful                                                     |
| 201         | Created - Request has been fulfilled                                      |
| 202         | Accepted - the request has been accepted but is not yet completed         |
| 204         | No Content - The request has been succesful but there is no message body. |
| 304         | Not Modified                                                              |
| 400         | Bas Request - The request could not be understood.                        |
| 403         | Forbidden - The server is refusing to fulfill                             |
| 404         | Not Found - The requested resource could not be found.                    |

## API Endpoints
[Fermentables](#Fermentables)
[Hops](#Hops)
[Misc](#Misc)
[Recipes](#Recipes)
[Equipment](#Equipment)
[Fermentations](#Fermentations)
[Yeasts](#Yeasts)
## Fermentables
| Method | Endpoint           | Usage                                  | Returns              |
| ------ | ------------------ | -------------------------------------- | -------------------- |
| GET    | /fermentables/     | Get the List of Available Fermentables | Fermentables Objects |
| GET    | /fermentables/{id} | Get a single fermentable               | fermentable          |
## Hops
| Method | Endpoint | Usage                          | Returns      |
| ------ | -------- | ------------------------------ | ------------ |
| GET    | /hops/   | Get the List of Available Hops | Hops Objects |
## Misc
| Method | Endpoint | Usage                          | Returns      |
| ------ | -------- | ------------------------------ | ------------ |
| GET    | /misc/   | Get the List of Available Misc | Misc Objects |
## Recipes
| Method | Endpoint | Usage                             | Returns        |
| ------ | -------- | --------------------------------- | -------------- |
| GET    | /recipes | Get the List of Available recipes | recipe Objects |
## Equipment
| Method | Endpoint    | Usage                               | Returns           |
| ------ | ----------- | ----------------------------------- | ----------------- |
| GET    | /equipment/ | Get the List of Available equipment | equipment Objects |
## Fermentations
| Method | Endpoint        | Usage                                   | Returns              |
| ------ | --------------- | --------------------------------------- | -------------------- |
| GET    | /fermentations/ | Get the List of Available fermentations | fermentation Objects |
## Yeasts
| Method | Endpoint | Usage                            | Returns       |
| ------ | -------- | -------------------------------- | ------------- |
| GET    | /yeasts/ | Get the List of Available yeasts | yeast Objects |