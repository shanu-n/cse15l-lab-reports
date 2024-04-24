# Part 1: Making a ChatServer!

### 1. The Code: (Credited to Skill Demo 1's `StringServer.java` and wavelet's `NumberServer.java` folder downloaded from Week 2's lab)
![Image](ChatServerSS1.png)
![Image](ChatServerSS2.png)
____________________________________________________________________________________________________________________________________________________________________________________________
### 2. `/add-message` Example 1:
![Image](ChatServerMessage1.png)
#### Which methods in your code are called?
In this example, the method `handleRequest` is being called.
#### What are the relevant arguments to those methods, and the values of any relevant fields of the class?
*The Relevant Arguments:* 
1. The URL (specifically the path an query)

*The Relevant Fields:*
1. `URI url`: This is the method’s only parameter, and it contains the URL of the page that we are using.
2. `StringBuilder builder`: An object of `StringBuilder` (a standard class in the `java.lang` package) which allows you to add different pieces of text together, which is used to build the final message.
3. `String[] parameters`: An array of strings used to store the split-up parts of the query part of the URL.
4. `String records`: A string variable which logs the conversations (each `/add-message` that happens) on the server.
#### How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
`StringBuilder builder`, `ArrayList<String> conversations`, and `String records` all change from this request. `StringBuilder builder` is initialized as an empty object, and then it is appended to, so it changes. The ArrayList that is not in the method but within the class, `ArrayList<String> conversations`, stores the messages in parts, so it also changes from being empty to containing the chat that is appended to it. `String records` stores all the messages from `conversations` as a single string, and as of now, it has one chat: 

`Shanu: Hi! This is Shanu's ChatServer!`

So it also changed.
____________________________________________________________________________________________________________________________________________________________________________________________
### 3. `/add-message` Example 2:
![Image](ChatServerMessage2.png)
#### Which methods in your code are called?
In this example, the method `handleRequest` is being called.
#### What are the relevant arguments to those methods, and the values of any relevant fields of the class?
*The Relevant Arguments:* 
1. The URL (specifically the path an query)

*The Relevant Fields:*
1. `URI url`: This is the method’s only parameter, and it contains the URL of the page that we are using.
2. `StringBuilder builder`: An object of `StringBuilder` (a standard class in the `java.lang` package) which allows you to add different pieces of text together, which is used to build the final message.
3. `String[] parameters`: An array of strings used to store the split-up parts of the query part of the URL.
4. `String records`: A string variable which logs the conversations (each `/add-message` that happens) on the server.
#### How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
`StringBuilder builder`, `ArrayList<String> conversations`, and `String records` all change from this request. `StringBuilder builder` is initialized as an empty object, and then it is appended to, so it changes. The ArrayList that is not in the method but within the class, `ArrayList<String> conversations`, stores the messages in parts, so it also changes from containing only the first chat to containing the new one as well. `String records` stores all the messages from `conversations` as a single string, so now it has 2 chats:

`Shanu: Hi! This is Shanu's ChatServer!`\
`Also Shanu: This works!`

So, this also changes.




