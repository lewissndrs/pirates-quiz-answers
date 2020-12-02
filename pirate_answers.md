Requesting All Pirates

Question 1 Which component is responsible for requesting all the pirates?

- PirateContainer

Question 2 Which hook do we use to carry out the requestAll() method and when does it get triggered?

- UseEffect, which is triggered when the page is mounted.

Question 3 The requestAll() method creates a new instance of Request() in order to gain the functionality to carry out various forms of request. Where is the Request class?

- The request class is found in the "helpers" folder.

Question 4 Which method are we using from the Request class here?

- The get() method.

Question 5 The PirateList component is in charge of rendering a list of pirate components. What is the pirateNodes function returning?

- it is returning a mapped list of Pirate components.

Viewing a Single Pirate
Question 1 When we click on one of the pirates names in the pirate list, our app renders a PirateDetail component. PirateDetail is in charge of rendering the information for a single pirate. But where is it getting its props passed down from?

- PirateContainer

Question 2

if (!pirate){
 return "Loading..."
}
What is the purpose of this code in PirateDetail?

- This code is to prevent an error from occuring if the pirate prop being passed into PirateDetail is null.

Question 3 In PirateDetail, to delete a pirate, we have a button with a listener "onClick" which triggers a method called "handleDelete". The handleDelete method uses a method onDelete which has been passed in as a prop from PirateContainer. Why have we passed this method down as a prop?

- This method has been passed down as a prop because the list of pirates is stored as a state in PirateContainer.

Bonus Points Questions
Question 1 In PirateContainer, what does Promise.all return?
- a single Promise which resolves to an array of the individual input Promises.

Question 2 Ideally, we want our state to live at the top of our component chain, except in one other scenario. This is when our component contains a, what?
- form.