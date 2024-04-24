# Part : Making a ChatServer!
## The Code: (Credited to Skill Demo 1's `StringServer.java` and wavelet's `NumberServer.java` folder downloaded from Week 2's lab)
![Image](ChatServerSS1.png)
![Image](ChatServerSS2.png)
## `/add-message` Example 1:
![Image](ChatServerMessage1.png)
### Which methods in your code are called?
In this example, the method `handleRequest` is being called.
### What are the relevant arguments to those methods, and the values of any relevant fields of the class?
*The Relevant Arguments:* The URL (specifically the path an query)\
*The Relevant Fields:*
1. `URI url`: This is the method’s only parameter, and it contains the URL of the page that we are using.
2. `StringBuilder builder`: An object of `StringBuilder` (a standard class in the java.lang package) which allows you to add different pieces of text together, which is used to build the final message.
3. `String[] parameters`: An array of strings used to store the split-up parts of the query part of the URL.
4. `String records`: A string variable which logs the conversations (each `/add-message` that happens) on the server.
### How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
`StringBuilder builder`, `ArrayList<String> conversations`, and `String records` all change from this request. `StringBuilder builder` is initialized as an empty object, and then it is appended to, so it changes. The ArrayList that is not in the method but within the class, `ArrayList<String> conversations`, stores the message, so it also changes from being empty to containing the chat that is appended to it. `String records` stores all the messages as a single string, and as of now, it has one chat: `Shanu: Hi! This is Shanu's ChatServer!`, so it also changed.
