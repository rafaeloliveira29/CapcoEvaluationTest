# CapcoEvaluationTest
Status: under Development.
____________________________________________________________________________________________________________________
Requirements: 
- Use .NetCore - OK
- C# - OK
- WebApi - OK
- Restful - OK
- Http Protocol - OK
- JSON - OK
- GIT (Make the code available in an own repository) - OK 
___________________________________________________________________________________________________________________
Evaluation Test to Capco for interview process - Description

This is a .NetCore API that consumes the https://swapi.co/ (The star wars API) and shows some informations obtained from it.
There are 4 methods of type GET on the "on development" API.
  - Index();
  - GetCharacterAsync();
  - GetCharactersList();
  - GetHumanCharacters();
  
  The index page was designed to make easier the calling of the functions described above. The function GetCharactersAsync() returns
  the character id, the character name, the year of birth if availabe and the names of the movies this character has participated. The 
  function GetCharactersListByName() returns all the characters ordered by name and shows between the character name, the number of films 
  has participated. The function GetHumanCharacter() returns all human characters, their heights and calculate the mean between all the
  human character heights.
  ____________________________________________________________________________________________________________________________
  Running The API:
  Download the code using the ˜clone or download button˜ on the right top corner of the page , open the .sln file on visual studio, execute the solution. it might open the job description page (localhost:port/api/character/index).
  
  to access the resources:
  => Get One character  => localhost:port/api/character/{characterId} => the id is in the range 1-86
  => Get The list of characters and its respective number of films made => localhost:port/api/character/order
  => Get only the human characters, ther height and the mean of the human heights => localhost:port/api/character/humans => Note that this one is the slowest link to load.
____________________________________________________________________________________________________________________________
  Tests:
