# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident that you know how the function works.
* Write a summary of what the function does.

```js
function (person, petName){
  for (let dog of person.dogs){
    if (dog.name === petName){
      return dog
    }
  }
}
```


Inputs and outputs should be valid JavaScript values!

| Input | 
(Andrew = {
  dogs: [
    {
      name: "Roxie",
      age: 10,
      color: "brown"
    },
    {
      name: "Mia",
      age: 12,
      color: "black"
    }
  ]
  cats: [
    {
      name: "Raja",
      age: 5,
      color: "orange"
    },
    {
      name: "Ellie",
      age: 7,
      color: "tri-colored"
    }
  ]
}
  , "Roxie")     

| Output | 
{
      name: "Roxie",
      age: 10,
      color: "brown"
    }

| Input | 
(Andrew = {
  dogs: [
    {
      name: "Roxie",
      age: 10,
      color: "brown"
    },
    {
      name: "Mia",
      age: 12,
      color: "black"
    }
  ]
  cats: [
    {
      name: "Raja",
      age: 5,
      color: "orange"
    },
    {
      name: "Ellie",
      age: 7,
      color: "tri-colored"
    }
  ]
}
  , "Mia")     

| Output | 
{
      name: "Mia",
      age: 12,
      color: "black"
    }

| Input | 
(Andrew = {
  dogs: [
    {
      name: "Roxie",
      age: 10,
      color: "brown"
    },
    {
      name: "Mia",
      age: 12,
      color: "black"
    }
  ]
  cats: [
    {
      name: "Raja",
      age: 5,
      color: "orange"
    },
    {
      name: "Ellie",
      age: 7,
      color: "tri-colored"
    }
  ]
}
  , "Raja")     

| Output | 
{
      undefined
    }


<table>
  <tr>
    <th>What does this program do?</th>
    <td>This program takes an input of an object(person) which includes an array (dogs) of objects. Inside the objects will be a property for the name of the object. The program also takes another input of a string (petName). The program will compare the string to the names of each object. If the string matches the name of the object, the program will output the entire object.    </td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
