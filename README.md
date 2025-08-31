# postman-practice
Practice project in API testing using Postman with Swagger Petstore. Includes CRUD requests, environment variables, and automated Postman tests


# Pokémon API – Postman Practice Collection

This repository contains my **Postman practice** using the [Swagger Petstore](https://petstore.swagger.io/#/) API.  
The collection demonstrates a basic **CRUD** flow for Pokémon (pets).

---

## Files

- **Practice.postman_collection.json** – Postman collection with requests.  
- **DEV POKEMONS.postman_environment.json** – Postman environment with variables:
  - `url` → API base URL (`https://petstore.swagger.io/v2`)  
  - `pokemonIDSkebob` → `2222`  
  - `pokemonIDAskibidi` → `3333`  
  - `Bandit228` → `228`  

---

## Collection overview

1. **Create new Pokémon**  
   - `POST /pet`  
   - Example body:
     ```json
     {
       "id": 228,
       "name": "Bandit228",
       "status": "available"
     }
     ```

2. **Get Pokémon by ID**  
   - `GET /pet/{{pokemonIDAskibidi}}`  
   - `GET /pet/{{pokemonIDSkebob}}`  

3. **Get Pokémon by status**  
   - `GET /pet/findByStatus?status=available`  

4. **Update Pokémon info**  
   - `PUT /pet`  
   - Example body:
     ```json
     {
       "id": 2222,
       "name": "Skebob",
       "status": "available"
     }
     ```

5. **Delete Pokémon**  
   - `DELETE /pet/{{Bandit228}}`  

---

## How to use

1. Import both files into **Postman**:  
   - `Practice.postman_collection.json` (Collection)  
   - `DEV POKEMONS.postman_environment.json` (Environment)  
2. Select environment **DEV POKEMONS** in Postman.  
3. Run requests in order:  
   **Create → Get → Update → Delete**.  

---

## Notes

- This project was created as part of my practice in **API testing**.  
- It demonstrates working with **CRUD operations**, **variables**, and the **Swagger Petstore API**.  
- Additional tests can be added in Postman to automatically validate status codes and response body fields.  
