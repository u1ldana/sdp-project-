We used a Layered Architecture in our project because it helps organize the code into clearly defined layers, each responsible for a specific functionality. This approach makes the system more flexible, scalable, and easier to maintain.
By applying this architecture with various design patterns, we have separated responsibilities between layers, improved modularity, made the system easier to maintain and scale, and ensured resilience to changes and future extensions.
In my development, I utilized several popular design patterns that helped improve the structure and behavior of the application. One of them is the **State Pattern**. It allows toggling between the "logged-in" and "logged-out" states, which controls how the page elements behave (whether they are shown or hidden). This provides a smooth and logical interface where the behavior of elements changes based on the state.

I also applied the **Observer Pattern**, which is evident in how events, such as clicking the "save" or "logout" buttons, trigger changes in the UI. Thanks to the Observer pattern, all updates occur dynamically in response to user actions.

For the "save" and "logout" buttons, I used the **Command Pattern**. Each click on these buttons can be seen as a command that encapsulates a user action. Handlers execute operations like updating data or ending the session, making the code more understandable and extensible.

The **Singleton Pattern** was applied through the use of localStorage to store user data. This storage acts as a single point of access, perfectly aligning with the Singleton principle — having a single instance of data.

Additionally, I used the **Factory Pattern** to create the userData object based on user input. This pattern allows the creation of objects without explicitly specifying their class, making the code more flexible.

Finally, I employed the **Template Method** to dynamically generate the HTML structure displaying user data. This approach provides a common algorithm with variable details, such as the current user's data, ensuring consistency and flexibility in rendering content.

These design patterns significantly simplified the maintenance and development of the application, making the code more readable and extensible.

