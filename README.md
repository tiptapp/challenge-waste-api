# API coding challenge

Imagine a neighborhood where each house has a bag of mixed waste placed outside the door. Each bag can contain several types of waste, like paper, plastics, or electronics. Garbage collectors from different recycling centers will come and pick up some bags based on their contents. The recycling centers have different rules of what types of waste they collect. All of them accept paper and plastics, but only some of them accept electronics. The rules change regularly.

Write the Backend for an app that lets the households classify what types of waste their bag contains, and the garbage collectors to know which bags to pick. Identify each bag with at minimum the street number by which they are placed.

1. Install Docker.
2. Clone this repository.
3. Run `docker-compose up --build` in the project folder.
4. Add two endpoints:
   - POST endpoint for creating a listing of a bag of waste, that accepts a payload containing only the waste types and the street number at which it is located.
   - GET endpoint for listing the bags, with a single parameter for specifying the id of a recycling center.
     - Bonus: remove the recycling center id, and get the recycling center id in some other way.
5. Bonus: add a GET endpoint for listing which recycling centers allow a list of certain bags, that accepts an array of bag ids as its only parameter.
